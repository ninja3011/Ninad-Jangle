/ [Home](/index) / [Tracker](/gsoc-2021) / [About](pages/gsoc/about) / [TL-Verilog](pages/gsoc/TLV) / [Blogs](pages/blogs/gsoc-final-blog) /

---

### Week 9

---

<div align = "center">
    <a align = "left" href = "./wk8"> < Prev </a> 
      /
    <a  href = "./wk10"> Next > </a>  
  </div>

1. **29/07/2021:** 
   * Switched to chakra-ui from bootstrap + css. 
   * Button clickhandler function names now to format handle button name
   * Defined BlocklyDiv in Main instead of BlocklyComponent so both files have access to it. This will eradicate the need for get and set methods and ill be able to make the BlocklyComponent into functional based component as well.
   * [container not in document error](https://stackoverflow.com/questions/45227309/uncaught-error-container-is-not-in-current-document)
  
2. **30/07/2021:**
   * Ported Panel stylings to chakra-ui from bootstrap 
   * Replaced divs with Boxes
3. **31/07/2021:**
   * Styled the blocklyDiv and buttons
   * Attempted to move blocklyDiv state up to global but facing container not in document error.
4. **1/08/2021:**
   * Did pane management of the interface using grid and flex.
   * Currently moved back stage of blocklyDiv to blocklyComponent to do stylings. 
5. **2/08/2021:**
   * Shortened Div error coming when applying ChakraProvider to the blocklyDiv.
   * Bifurcated Code from Main.js to Panel.js and toolbox.js in Components folder. Integration left.
6. **3/08/2021:**
   * Integrated Panel and toolbox with Main.
   * Attempted to move blocklydiv and toolbox ref upwards. Still facing errors.
7. **4/08/2021:**
   * Moved blocklydiv up, no error. It is the toolbox ref that is giving the error. 
   * This is because the ref is then being defined outside the component
