# Mechanical Ventilator 
## Background
A mechanical ventilator is a machine that enables a patient to breathe when the patient cannot breath sufficiently on their own. The purpose of a ventilator is to:
- deliver high concentrations of oxygen into the lungs. 
- help get rid of carbon dioxide. 
- decrease the amount of energy a patient uses on breathing so their body can concentrate on fighting infection or recovering

### Respiratory Mechanics
1. Peak airway pressure:
        
        Represents the total pressure needed to push a volume of gas into the lung and is calculated as:

                Peak Airway Pressure = Resistive Pressure + Elastic Pressure + PEEP
        
2. Resistive pressure

        The product of circuit resistance and airflow.

3. Elastic pressure

        The product of the elastic recoil of the lungs and chest wall (elastance) and the volume of gas delivered.

4. Positve End-expiratory pressure

        The positive pressure that will remain in the airways at the end of the respiratory cycle (end of exhalation) that is greater than the atmospheric pressure in mechanically ventilated patients.

5. Intrinsic PEEP

        Occurs when the expiratory time is shorter than the time needed to fully deflate the lungs, preventing the lung and chest wall from reaching an elastic equilibrium point. It is also know as autoPEEP.



### Parameters
The parameters measured include:

- Respiratory rate
- Tidal volume
- Trigger sensitivity
- Flow rate
- Inspiratory/expiratory (I/E) ratio


### Operation Modes
A mechanical ventilator operates in the following modes:

- Volume cycled: Delivering a constant volume with each breath (pressures may vary)

- Pressure cycled: Delivering constant pressure during each breath (volume delivered may vary)

- A combination of volume and pressure cycled


Volume-cycled ventilation delivers a set tidal volume. This mode includes:

1. Volume-control (V/C)
2. Synchronized intermittent mandatory ventilation (SIMV) 

Pressure-cycled ventilation delivers a set inspiratory pressure. This mode includes:

1. Pressure control ventilation (PCV)
2. Pressure support ventilation (PSV)
3. Noninvasive modalities applied via a tight-fitting face mask (several types available)


### References
1. [Oxford Medicine](https://oxfordmedicine.com/view/10.1093/med/9780199600830.001.0001/med-9780199600830-chapter-92)

2. [MSD Manuals](https://www.msdmanuals.com/professional/critical-care-medicine/respiratory-failure-and-mechanical-ventilation/overview-of-mechanical-ventilation)

3. [NCBI](https://www.ncbi.nlm.nih.gov/books/NBK441904/)



## Project Structure
This project is divided into the following modules:
1. Mechanical
2. Electrical/eletronics
3. Software and control
4. Resources
Each of the modules/directories has a README.md file at the root of the directory

### Scope
This project will focus on the following modes of operation:

1. AC mode of ventilation

        - Tidal Volume (TV)- normally between 500-600ml (Set 500ml as default)
        - Frequency of Breathing/Breaths per Minute(BPM)/Respiratory Rate (RR) ---
                * Adult (12-60 Breaths Per Minute (BPM) (set default at 12 BPM)
                * Child (18-60 BPM) (set default at 18 BPM)
        - Fractional Inspiration of Oxygen (FiO2) – Between 35- 100% (set default at 35)
        - PEEP – Normally around 5cm H2O (Set 5 cm H2O as the default)

2. Synchronized Intermittent Mandatory Ventilation (SIMV)

        - Tidal Volume (TV)- normally between 500-600ml (Set 500 as default)
        - Frequency of Breathing/Breaths per Minute(BPM)/Respiratory Rate (RR) (set default at 12)
        - Fractional Inspiration of Oxygen (FiO2) – Between 35- 100% (set default at 35)
        - PEEP – Normally around 5cm H2O (Set 5 as the default)
        - Pressure Support (PS) (Between 5 – 15 cm H2O) (Set 5 as the default)
3. Pressure Support

        - FiO2 (Set 35 as the default)
        - PEEP (Set 5 as the default)
        - PS (PS) (Between 5 – 15 cm H2O) (Set default as 5 cm H2O)


### Version control
#### Branches 
- master:
        Production branch
- staging:
        Testing branch
- mechanical:
        Development branch for mechanical features
- electrical_electronics:
        Development branch for electircal and electronics
- software:
        All Devcode goes here
- resource

Convention for pushing items to a particular branch:
        
        feature-X-name: Feature implementation branch. Branched from the dev branches
        hotfix-x-name: Fix errors on production branch

Commit messages convention:

        <type>[optional scope]: <description>

        [optional body]

        [optional footer(s)]

        Examples:

                - feat(ac mode): alert when pressure goes below ...
                - docs: correct spelling of VENTILATOR
                - feat(ac mode): add tidal parameter
                - fix: prevent skipping of breaths
                - resources: add pcb schematic 



## Contribution
Contributions to this project are welcomed and encouraged.

### Issues
Feel free to submit issues and enhancement requests.

### Contributing
Please refer to our project's style and contribution guidelines for submitting patches and additions. Follow the "fork-and-pull" Git workflow.

1. Fork the repo on GitHub
2. Clone the project to your own machine
3. Commit changes to your own branch
4. Push your work back up to your fork
5. Submit a Pull request so that we can review your changes

NOTE: Be sure to merge the latest from "upstream" before making a pull request!

### License
        MIT License

        Copyright (c) 2022 Smith Jilks

        Permission is hereby granted, free of charge, to any person obtaining a copy
        of this software and associated documentation files (the "Software"), to deal
        in the Software without restriction, including without limitation the rights
        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
        copies of the Software, and to permit persons to whom the Software is
        furnished to do so, subject to the following conditions:


        The above copyright notice and this permission notice shall be included in all
        copies or substantial portions of the Software.

        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
        SOFTWARE.


## Authors
- [Smith Jilks](https://www.linkedin.com/in/jilks-smith-56ba74173/)
<a href="https://github.com/QUALIS-LABS/IBM-Call-for-code-2021-zero-hunger-solution/graphs/contributors">

  <img src="https://contrib.rocks/image?repo=smithjilks/JKUAT-mechanical_ventilator_v1" />
</a>

Made with [contributors-img](https://contrib.rocks).



