#1 Установка и настройка Babel

//initializing npm (-y means accept all by default) - package.json
>> npm init -y

// install babel - node_modules
>> npm i babel-cli babel-core babel-preset-es2015 --save-dev

src - source code           //исходный код
dist- distribute code     //конечный код

package.json ->"test"..... заменить на  -> "scripts":{
                        "build": "babel src -d dist --presets es2015"
                        }
                        
>> npm run build

package.json -> "watch": " babel src -d dist --presets es2015 -w"

>> npm run watch