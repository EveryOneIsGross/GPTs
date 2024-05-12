```mermaid
%%{init: {'theme': 'base', 'themeVariables': { 'primaryColor': '#ffaa00', 'primaryTextColor': '#ffaa00', 'primaryBorderColor': '#ffaa00', 'lineColor': '#ffaa00', 'secondaryColor': '#ffaa00', 'tertiaryColor': '#ffaa00', 'clusterBkg': 'none', 'clusterBorder': 'none', 'fontSize': '0px'}}}%%

graph TD
    A1(("Problem Description")) --> B1(("Reflect on Problem"))
    A2(("Self-reflection")) --> B1
    A3(("Solution Concept")) --> B2(("Example Explanation"))
    B1 --> B3(("Generate Solution"))
    B2 --> B3
    B3 --> B4(("Modular Code Division"))
    B4 --> B5(("Double Validation"))
    
    B5 --> C1(("Correct Code Solution"))
    B5 --> C2(("Explanation of Logic"))
    
    D1(("Exhaustive Approach")) --> B3
    D2(("Code Quality")) --> B4
    D3(("Ignore Constraints")) --> B3
    
    subgraph Input
    A1
    A2
    A3
    end
    
    subgraph Process
    B1
    B2
    B3
    B4
    B5
    end
    
    subgraph Output
    C1
    C2
    end
    
    subgraph "Parameter Space"
    D1
    D2
    D3
    end
```
