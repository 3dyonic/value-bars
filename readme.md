# Value bar
job interview assignment by Yonatan Lev Ari  
[demo](https://3dyonic.github.io/value-bars/.)

## Specification
1. Each bar can have a value between 0 to 100  
  - Bar design is changing based on it’s value:
    - Left bar: value is above 80
    - Right bar: value is below or equal to 80  
    - Vertical arrows are pointing down  
    - Top indicator is red and pointing down
2. Build 
  - Gap between the border and the content should be transparent  
  - Be accurate as you can  
  - Don’t use images except for the black arrow  
  - Try to build with a few elements as you can  
  - Use class for the low state (red)

## Development dependencies:
simple npm configuration with node sass


### Highlights
A simple html component with scss setup.  
This exercise demonstrate a progress value var with low and high values switch. 

#### Expected beheviour: 
1. value bars with class toggle for low and high
1. only arrow images.

## Styling methods: 
- scss with sass-lint configuration
- role based architecture
  - seperation between global and component scope.
  - configuration based for global and component scope.
  - style guide as a global definition layer
- BEM ,OOCSS.
- Component selectors are self containted and isolated.  
  - using global tokens for configuration
  - using global mixins and functions
- Utilized mixins and functions for selector indipendent future re-use.
- Rule based linting


### Styling dependencies: 
- Since i wanted to simulate a real use case i chose the seperate between the component to external layers.
- external layers for this example are:
  - global config (containing the style guide and semantic tokens, very minimalistic for this component example)
  - base layer (reset)

### Notes:
For this example css folder contains the final output in styles.css but also contains:  
- global.css  
- value-bar.css  
i did it so we can also bench mark standalone output. 
therfore these files are not prefixed with '_" (against the common practise).

#### Performance statistics:
External requests: 0  
Global Size: 90 bytes  
Component Size: 1.61 kb  
Total: 1.79 bytes    
Lint Errors: 0
