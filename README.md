#  Learning Heat Capacity with AI : 

**Merging Physics and Data from Shulman Equation to PINNs and Beyond**

---

##  Overview

This project explores the modeling of heat capacity \( Cp \) as a function of temperature \( T \) for a variety of materials using both physics-based equations and modern AI techniques. The goal is to analyze, generalize, and compare different approaches including:

- Fitting **Shulman's empirical model**

- **Neural Network (NN)** smoothing

- **Physics-Informed Neural Networks (PINNs)** enforcing physical laws (Debye and Dulong--Petit)

- **Symbolic regression** via PySR

- Specialized **NASA polynomial fitting** for gaseous substances

Each approach is applied on real material datasets to investigate their effectiveness in accuracy, extrapolation, and physical plausibility.

---

##  Project Structure

```bash

 heat-capacity-ai

├── README.md

├── datasets/

     ├── CO2.csv

     ├── bronzite.csv

     ├── ice.csv

     ...

     ├── metadata.txt # Physical properties & notes per material



├── notebooks/

    ├── co2.ipynb # Notebook analysis for CO₂

    ├── ice.ipynb # Analysis for ice using all approaches

     ...

```


-   **`datasets/`**: Contains `.csv` files where each dataset corresponds to a specific material.\
    Each file has two columns:

    -   `T` --- Temperature (in Kelvin)

    -   `Cp` --- Heat Capacity (in J/mol-K)

    The `metadata.txt` file contains complementary physical information for each material (phase, references, notes).

-   **`notebooks/`**: For each material, there's a dedicated Jupyter notebook. It includes:

    -   Data loading and visualization

    -   Shulman equation fitting using LM algorithm

    -   Neural network smoothing

    -   PINN with physical loss enforcement

    -   Symbolic regression using PySR

    -   Optional NASA polynomial fitting (for gases)

* * * * *

 How to Use
-------------

###  Installation

1.  Clone the repository:


```bash



git clone https://github.com/your-username/heat-capacity-ai.git
cd heat-capacity-ai

```

2.  Install dependencies (recommended: Python 3.9+):



```bash

pip install -r requirements.txt

```

3.  Explore notebooks 




* * * * *

 Contribute and Collaborate
-----------------------------

This project is a work in progress, and collaboration is welcome!

If you:

-   have a **new dataset** for any material (solid, liquid, gas),

-   know **alternative modeling techniques**,

-   want to improve fitting, modeling, or visualization,

please **open a Pull Request (PR)**. Let's cooperate and grow the **largest open-source dataset and analysis hub** for heat capacity estimation of all known materials.

* * * * *

 License
----------

MIT License. Free to use, modify, and distribute --- with attribution.

* * * * *

 Acknowledgments
------------------

Special thanks to **CRAAG Institute** and **Dr. Naceur Bouziani** for the valuable guidance, and to **ENSIA** --- the National School of Artificial Intelligence --- for the scientific formation and academic support.

* * * * *

 Let's model the thermal universe --- one dataset at a time!
-----------------------------------------------------------
