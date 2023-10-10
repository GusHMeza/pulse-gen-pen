# pulse-gen-pen
Digital probe project. Winter 2023
Este proyecto es una pluma generadora de pulsos. 

Experiencia de usuario: 
1. Presiona uno de tres botones para que la pluma entregue un tren de pulsos continuo a la frecuencia seleccionada. 

Notas de diseño: 
1. Si se presionan dos botones a la vez, se habilitan dos fuentes de corriente al mismo nodo, con lo cual se pueden crear frecuencias adicionales a las determinadas. 
2. Para la frecuencia de 1Hz se necesitan 10 MOhms; para la de 1kHz, alrededor de 10 kOhms; para la de 10 kHz, 1 kOhms.
3. El datasheet de U5 SE555DR establece en los diagramas de circuitos de aplicacion que para una operacion astable hay que colocar una resistencia entre DISCH y THRESH, para que el capacitor se descargue hasta el valor en THRESH, que es 1/3 VCC. ¿Está bien colocado y es R35 de suficiente buen tamaño? 
4. El layout debe ser idealmente de 16mm * 100mm
