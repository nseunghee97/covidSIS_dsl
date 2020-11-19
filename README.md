# covidSIS

**Network Modeling on Covid-19**

---

**Data Science Lab**  
**Network Analysis Study**  
[Jinwoo Lee(이진우)](https://github.com/jinwu99), [Jiwoo Kim(김지우)](https://github.com/zioo1004), [Seunghee Nam(남승희)](https://github.com/shd04121)

---


## Study Overview

**[Network Analysis](https://www.notion.so/Network-Analysis-c36b0e2c19ed4e3d865aa8c94a11b88e)**

- [Network Visualization using Gephi](https://www.notion.so/Gephi-cd69959603f9477881a0e68bada90daf)
- Network Modeling
  - [ERGM(Exponential Random Graph Model)](https://www.notion.so/ERGM-Exponential-Random-Graph-Model-d5bdb371c7fa47e9838bcf646a2b2a93)
    - [Hierarchical ERGM](https://docs.google.com/presentation/d/1nJbM5os3KeD4proiX-znSSRXwCY6jqvdsQqvSDmzU48/edit?usp=sharing)
    - MultiLayer ERGM
    - Temporal ERGM
  - [SBM(Stochastic Block Model)](https://www.notion.so/SBM-Stochastic-Block-Model-52cc1201be204a1caa4c6991ce934761)
  - [LSM(Latent Space Model)](https://www.notion.so/LSM-Latent-Space-Model-70f876fdf70546299b7bf1dcd158a760)
  - Multiplex Network
  - [Dynamic Networks](https://www.notion.so/Dynamic-Networks-fdc592a56e1a42fe835611b6b5d351cb)
    - SIS
    - SIR
    
## Networking Modeling on Covid-19

### Code Detail

- **model** : R markdown files regarding each network models
  - `ERGM.Rmd`
  - `SBM.Rmd`
  - `LSM.Rmd`
  
- **project** : python notebook codes
  - **bus**
    - `node_edge_file.ipynb`
      - Preprocess on public dataset. Create node and edge file.
    - `SIS_on_bus_network.ipynb`
      - Create Graph instance using node and edge file from `node_edge_file.ipynb`.
      - Epidemic model simulation using python `EoN` package.
      - Visualize simulation results geographically using python `folium` package.
  - **subway**
  - **publicBike**
    - **data**
      - `public_bike_rental_log.csv` : Rental log of Seoul public bike. *★ Large File. Should be unzipped.*
      - `public_bike_rental_point.csv` : Rental point of Seoul public bike.
    - `public_bike_network_EDA.ipynb`
      - Preprocess on public bike dataset. Create graph instance using node and edge file.
      - EDA on public bike network.
      - Simple visualization using network statistics.
    - `public_bike_network_SIS.ipynb` 
      - Epidemic model simulation using python `EoN` package.
    - `rental_g.pickle` : Graph object of public bike network
    - `public_bike_network_visualization.gephi` : Visualization of public bike network using Gephi.
    
