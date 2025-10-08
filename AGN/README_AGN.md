## **AGN Spectral Decomposition and Black Hole Mass Estimation**

This project teaches students how to use **Python** (via **Google Colab**) to analyze **AGN spectra from SDSS**.
The workflow guides users from raw data retrieval to calculations of black hole mass and accretion.

---

### **Overview**

Students will learn how to:

1. **Download a spectrum** from SDSS using `astroquery` and an AGN list (CSV provided).
2. **Perform PCA decomposition** to separate AGN and host galaxy components using eigen-spectra.
3. **Subtract the galaxy contribution** to isolate the pure AGN spectrum.
4. **Fit the H-β emission line** (broad and narrow) using multi-component Gaussian fitting.
5. **Measure spectral properties** — line flux, FWHM (km s⁻¹), and luminosity at 5100 Å.
6. **Compute physical parameters** — SMBH mass, bolometric luminosity, Eddington luminosity, Eddington ratio, and growth time.

---

### **Requirements**

Install the following Python packages (Colab-ready):

```bash
pip install numpy scipy astropy matplotlib lmfit astroquery specutils
```

---

### **Repository Structure**

```
ThaiPASS2025/AGN/
|── how_giants_grow_workbook.ipynb
|── data/
│   └── table_dr16_qso_krc213.csv
│   └── eigSpec_qso_0.dat
│   └── ...
│   └── galaxyKL_eigSpec_10.dat
└── README.md
```

---

### **Quick Start (Colab)**

```python
from google.colab import drive
drive.mount('/content/drive')
%cd /content/drive/MyDrive/ThaiPASS2025/AGN
```

Run the provided notebook and follow the step-by-step exercises.


### **You can clone directly from Google Colab here:**
https://colab.research.google.com/drive/19QCVNpoflF9AWl-vkIZHGR4USchH3Q9D?usp=sharing

### **Here is the answer to the above workbook:**
https://colab.research.google.com/drive/1Gm6OktBr5pysdGzmfzTYovxZjK2DuJSc?usp=sharing

---

### **References**

* Chanchaiworawit & Sarajedini (2024), *AGN host galaxy decomposition and SMBH growth studies*
* Vestergaard & Peterson (2006), *ApJ, 641, 689* – Single-epoch black hole mass relations
* Shen et al. (2011), *ApJS, 194, 45* – SDSS quasar catalog
* Netzer (2019), *MNRAS, 488, 5185* – Accretion physics

---

### **Acknowledgments**

Developed at **NARIT (Thailand)** for educational and research use.
Based on SDSS public data and open-source Python tools.
