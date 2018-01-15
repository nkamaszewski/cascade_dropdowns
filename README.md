# cascade_dropdowns
Cascade Dropdowns (with unlimited nesting) Component written in Angular JS.
There is a example of use cascade_dropdown_component with fake data.
To avoid errors Your JS object (or JSON) data file should be in format like that:
data = [
            {label: "BMW", value: 0, level: 0, description: "The car brand", child: null},
            {label: "Audi", value: 1, level: 0, description: "The car brand", child: [
                {label: "A3", value: "1a",level: 1, description: "Model",child: [
                    {label: "1.9 TDi", value: "1aa",level: 2, description: "Engine",child: null},
                    {label: "1.4 TFSI", value: "1ab",level: 2, description: "Engine",child: null},
                    {label: "2.0 TFSI", value: "1ac",level: 2, description: "Engine",child: null}   
                ]},
                {label: "A4", value: "1b",level: 1, description: "Model",child: null},
                {label: "RS6", value: "1c",level: 1, description: "Model",child: [
                    {label: "4.2 TFSI", value: "1ad",level: 2, description: "Engine",child: [
                        {label: "560 KM", value: "2ada",level: 3, description: "Power",child: null}
                    ]},
                ]},
                {label: "R8", value: "1d",level: 1, description: "Model",child: null}
            ]},
            {label: "Honda", value: 2, level: 0, description: "The car brand",child: [
                {label: "Civic", value: "2a",level: 1, description: "Model",child: [
                    {label: "2.2 C-TDI", value: "2aa",level: 2, description: "Engine",child:[
                        {label: "100 KM", value: "2aaa",level: 3, description: "Power",child: null},
                        {label: "120 KM", value: "2bbb",level: 3, description: "Power",child: null},
                        {label: "140 KM", value: "2bcc",level: 3, description: "Power",child: null}
            ]},
                    {label: "1.8 V-TEC", value: "2bb",level: 2, description: "Engine",child: null},
                    {label: "1.4 V-TEC", value: "2bc",level: 2, description: "Engine",child: null}
            ]},
                {label: "CR-V", value: "2b",level: 1, description: "Model",child: null}
            ]},
            {label: "Suzuki", value: 3, level: 0, description: "The car brand",child: null},
            {label: "Opel", value: 4, level: 0, description: "The car brand",child: [
                {label: "Astra", value: "4a",level: 1, description: "Model",child: null},
                {label: "Insignia", value: "4b",level: 1, description: "Model",child: null}
            ]}
        ]
       
       
Where nesting child is no limited, and adding another fieds in object does not affect the operation in component.

Enjoy!
