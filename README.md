# Essential Variables Sankey Diagram

This project visualizes the relationships between **Essential Variables (EVs)** using an interactive [D3.js](https://d3js.org/) Sankey diagram. The diagram helps to explore how EVs are linked across categories, such as Climate, Biodiversity and Ocean.

🔗 **Live Demo:**  
[https://biodiversity-aq.github.io/essential-variables-sankey-diagram/](https://biodiversity-aq.github.io/essential-variables-sankey-diagram/)

---

## 📊 About the Visualization

This Sankey diagram shows the **hierarchical and thematic relationships** between Essential Variables. It allows you to:

- Hover over any node to highlight its **upstream and downstream** connections.
- See how various EVs flow across domains and subdomains.
- Easily identify central variables with many dependencies.

The relationships are defined in a simple JSON file (`data/ev.json`) which you can edit to modify the diagram.


## 📁 Project Structure

```
essential-variables-sankey-diagram/ 
├── index.html # Main visualization (D3 + Sankey) 
├── data/ 
│   └── ev.json # Source data: relationships between variables 
└── README.md # This file
```

## 🚀 Getting Started Locally

To test it locally before publishing:

```bash
git clone https://github.com/biodiversity-aq/essential-variables-sankey-diagram.git
cd essential-variables-sankey-diagram
python3 -m http.server
```

Then, open your browser and navigate to `http://localhost:8000/`.

## 📦 Data Format (ev.json)

Each entry in ev.json represents a connection:

```json
{
  "from": "Biodiversity",
  "to": "Species distribution"
}
```

## 📜 License

This project is open source under the [MIT License](https://github.com/biodiversity-aq/essential-variables-sankey-diagram?tab=MIT-1-ov-file#readme).