# emeli

EMELI (Experimental Modeling Environment for Linking and Interoperability) is a model coupling framework written in Python that was designed to explore the possibility of "smart modeling frameworks." As defined here, a smart modeling framework is one that makes it easy for users to couple reusable component models to create new, composite models through the use of a standardized model interface and standardized model metadata. Users make selections from a repository of component models that each provide a CSDMS Basic Model Interface (BMI) for self-description and model control. EMELI then (1) creates a framework object that serves as a container for the component models, (2) instantiates the selected component models as objects in the framework, (3) checks whether the chosen component models are compatible and together provide a complete composite model (i.e. whether every component model can get the variables it needs from one of the other models in the selected set) and then (4) runs the model, automatically passing required variables (or references) between the coupled components as necessary and automatically adjusting for differences between the component models, such as time-stepping scheme and units. EMELI demonstrates an attractive mechanism for coupling heterogeneous models after they have undergone a relatively small amount of additional preparation while also helping to prevent inappropriate couplings.

In order to use EMELI, you need a collection of BMI-enabled model components either written in Python or with Python bindings.  Because of this, the source code for EMELI is included in the <b>framework</b> folder of the <b>topoflow36</b> repository.  This can be found at:
https://github.com/peckhams/topoflow36/tree/master/topoflow/framework.

You can learn how EMELI works by reading the paper by Peckham (2014) in the <b>docs</b> folder.



