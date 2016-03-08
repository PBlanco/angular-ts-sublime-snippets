# Angular 1.5 Typescript Snippets for Sublime Text

###Usage
1. Place the snippet files in your sublime `User` folder
2. Create a new typescript file (.ts), then type in `ng1controller` or `ng1module` or `ng1service` and press tab. The option to use the snippet should appear as you type

The `User` folder should be in the same location as the user settings file (from sublime menu `Sublime Text > Preferences > Settings - User` on OSX)

###Snippets
Controller (`ng1controller`)
````javascript
namespace Module {
    'use strict';

    export class className {
        static $inject: Array<string> = [dependency1];

        constructor(private dependency1: dependency1Type) {
        }
    }

    angular
        .module('Module')
        .controller('className', className);
}
````

Service (`ng1service`)
````javascript
namespace Module {
    'use strict';
    
    export interface IService {
    }
    export class Service implements IService {
        static $inject: Array<string> = [dependency1];

        constructor(private dependency1: dependency1Type) {
        }
    }

    angular
        .module('Module')
        .Service('Service', Service);
}
````

Module (`ng1module`)
````javascript
namespace Module {
    'use strict';

    angular
        .module('Module',[
            
        ]);
}
````

## License
The MIT License (MIT)
