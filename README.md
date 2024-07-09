# JAVASCRIPT-Destructuring

#### Destructuring, or Destructuring assignment
#### A JavaScript feature to extract data from arrays and objects.
#### It's (syntactic sugar) an easier, shorter, and clearer way to write expressions than other forms.

### Destructuring Arrays

    let cars = ['ferrari', 'tesla', 'cadillac'];
    let [car1, car2, car3] = cars;
    console.log(car1, car2, car3); // Prints: ferrari tesla cadillac

##### We created a new array `3 variables (car1, car2, car3)` corresponding to the `3 elements` in the cars array and their `3 values`.

### Destructuring Objects

    let destinations = { x: 'LA', y: 'NYC', z: 'MIA' };
    let { x, y, z } = destinations;
    console.log(x, y, z); // Prints LA NYC MIA

##### Create new variables (x,y,z) directly from an object’s properties.
    
### Destructuring Function Parameters

    let truck = {
      model: '1977 Mustang convertible',
      maker: 'Ford',
      city: 'Detroit',
      year: '1977',
      convertible: true
    };
                         //Funciton uses object destructuring to create three parameter variables:
    const printCarInfo = ({model, maker, city}) => {              
      console.log(`The ${model}, or ${maker}, is in the city ${city}.`);
    };

    printCarInfo(truck);
    // Prints: The 1977 Mustang convertible, or Ford, is in the city Detroit.

#####  The function printCarInfo is invoked with the truck object, these parameters are assigned the corresponding values from that object.
