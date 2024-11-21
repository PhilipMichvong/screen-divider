# **Screen Divider - PowerShell Workflow Generator**

**Screen Divider** is a powerful tool that allows you to easily manage and organize your workspace by automating the placement of applications across multiple monitors in a specified layout. This tool generates a custom PowerShell script that positions your applications on the screen based on your chosen configuration.

---

## **Features**
- **Multi-Monitor Support:** Automatically detects and manages multiple monitors.
- **Flexible Layouts:** Choose between horizontal or vertical screen divisions.
- **App Assignment:** Choose executable applications and assign them to specific regions on your screen.
- **PowerShell Script Generation:** Generates a PowerShell script that launches your apps and positions them on the screen exactly where you need them.

---

## **Installation**

### **Requirements**
Before you get started, make sure you have the following installed:
- **Python 3.x**: You can download Python from [here](https://www.python.org/downloads/).
- **Pip**: The Python package manager should be installed along with Python.
- **PowerShell**: PowerShell is needed to execute the generated scripts.
  
### **Dependencies**
You will also need to install the following Python libraries:

```bash
pip install -r requirements.txt
```

## **How to Use**

### **Step 1: Clone or Download the Repository**

Clone the repository to your local machine using Git:




```
git clone https://github.com/PhilipMichvong/screen-divider
```
Alternatively, you can download the project as a `.zip` file directly from GitHub and extract it to your desired location.

### **Step 2: Run the Application**

Navigate to the project folder and launch the app:



`python app.py`

This will open a graphical user interface (GUI) where you can select your monitor(s), layout, and applications.

### **Step 3: Select Monitor and Layout**

- **Monitor Selection**: Choose which monitor you want the apps to be displayed on.
- **Layout Selection**: Choose whether you want a **horizontal** or **vertical** layout for your apps.

### **Step 4: Choose Applications**

Click the **Choose App** buttons to select up to 5 executable (.exe) applications from your computer. These applications will be assigned to the regions you defined in the layout.

### **Step 5: Generate PowerShell Script**

Once all apps are selected, click **Generate PowerShell Script**. You will be prompted to save a `.ps1` PowerShell script. This script can then be run on your machine to open and position the applications automatically.

---

## **How It Works**

1. **Monitor Detection:** The app automatically detects all connected monitors.
2. **Layout Calculation:** Based on the selected layout (horizontal or vertical), the application divides the screen into regions and assigns each region to one application.
3. **Script Generation:** The app generates a PowerShell script that:
    - Launches the selected applications.
    - Positions them on the screen at the specified regions using `SetBounds` for window management.

---

## **Example Usage**

### **Example 1: Horizontal Layout with 3 Applications**

1. Select the monitor where you want to place the applications.
2. Choose a **horizontal** layout with 3 regions.
3. Pick 3 applications (e.g., a browser, a text editor, and a terminal).
4. The generated PowerShell script will launch the applications and position them from left to right across the screen.

### **Example 2: Vertical Layout with 2 Applications**

1. Select the monitor.
2. Choose a **vertical** layout with 2 regions.
3. Choose 2 applications (e.g., a media player and a PDF viewer).
4. The PowerShell script will launch the applications and place them one on top of the other.

---

## **Additional Notes**

- **Customization**: You can always edit the generated PowerShell script to further customize the positions or modify which applications are opened.
- **Multi-Monitor Support**: If you have multiple monitors connected, simply select the one you wish to use in the app.

---

## **Contributing**

If you would like to contribute to this project, feel free to fork the repository and submit a pull request. Make sure to follow the existing code style and add any necessary documentation or tests.

---

## **License**

This project is licensed under the MIT License - see the LICENSE file for details.

---

## **Acknowledgements**

- **customtkinter** for providing the simple and customizable GUI components.
- **screeninfo** for detecting monitor details.

---

## **Screenshots**
![screen1](/assets/1.png)
![screen2](/assets/2.png)
![screen3](/assets/3.png)

---

## **FAQ**

**Q1: Can I use this tool on Mac or Linux?**

- Currently, this tool is designed for Windows systems, as it uses PowerShell to position the windows. The script generation is tailored to Windows environments.

**Q2: What happens if I have more than 5 apps?**

- The app currently supports up to 5 applications. If you need more, you can manually edit the PowerShell script to add extra windows.

**Q3: Can I edit the generated PowerShell script?**

- Yes! You can always modify the PowerShell script to better fit your needs, such as adjusting window positions or adding new applications.