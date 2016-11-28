# Unsupervised Approach To AI Web Development

## Goal
&nbsp;&nbsp;&nbsp;&nbsp; This paper provides a high-level description of a machine learning algorithm that learns to write HTML and CSS code using spatial-temporal recognition and goal-driven behavior. It explains how sensory input from multiple domains (visual, text) is coupled to discover associations, along with the role of motor output in multiple environments at once.

***

## Sensory-Motor Processing
&nbsp;&nbsp;&nbsp;&nbsp; The system outputs HTML tags and CSS elements into a text document and received visual input from the webpage, as well as textual input from the document. The system has a database of preloaded HTML tags and CSS elements that are inserted at selected locations within the document.

***

## Spatial-Temporal Learning
&nbsp;&nbsp;&nbsp;&nbsp; Development occurs across a variety of domains. First, the system must associate HTML and CSS outputs with changes to the webpage. Once there is an adequate understanding of environmental effects of actions, the system turns to the document itself to comprehend the structure of HTML and CSS, particularly the way in which a tag/element has different effects depending on the location it is inserted and the contextual significance of the other tags/elements in the document.

***

## Goal-Oriented Behavior
&nbsp;&nbsp;&nbsp;&nbsp; Having learned visual patterns from the webpage, ordering patterns in the document, and the relationship between document and webpage, the system observes a desired state of the webpage and attempt to construct a desired state of the document based on its past experience with associating webpage-document changes. It can then perform actions that alter the document with the intention of reaching the desired state of the webpage. The system has the ability to detect its own errors by comparing the desired state to the progress it's made, and then makes judgments based on the efficiency of attempted strategies. 

&nbsp;&nbsp;&nbsp;&nbsp; This self-critique determines whether sequences of actions are scrapped due to poor performance, or saved as a solution to similar problems in the future. Sequences of actions are essentially plans to solve problems where the current state must be transformed into a desired state. Naturally, certain plans will fit a task better than others. Thus the plans compete to be the best method of performing transformations to the state in a desirable way, relative to the current and desired states. Solutions are optimized through a competitive, self-organizing process.

&nbsp;&nbsp;&nbsp;&nbsp; A plan is created in response to a desired state transformation for which there is no known solution. The differences between current and desired states are detected by observing both to find which patterns are missing from the current state and which must be removed. 

&nbsp;&nbsp;&nbsp;&nbsp; Pattern changes are correlated with certain document actions that are believed to cause the change. This provides the system with a desired state of the document itself, which is compared to the current state to find the required changes. These requirements, along with knowledge from past experiences regarding the order constraints of tags and elements, are used to construct a plan that attempts to move the current state of the document to the desired state.

***

## Learning
-	Spatial: shapes, colors, and text on the webpage, and orientation of objects. Order constraints of tags and elements within the document.
-	Temporal: changes in the webpage following an action in the document. Cause and effect of actions. Assists in processing multiple bits of input (limited number of sensors) over a period of time to comprehend the scene as a whole (this occurs with visual information from the webpage as it is viewed in sections, as well as textual information from the document as it is viewed line-by-line) even when the environment is not changing.
-	Reinforcement: utilizes knowledge about the effects of actions in the document to reach a desired state of the webpage. Trial and error results in a perceived fitness associated with each plan regarding its ability to solve a certain problem.

***

## Action
-	Webpage: movement of sensors across the webpage. Limited number of vision modules constrains the amount of pixels seen at any given time.
-	Document: movement of sensors across the document. Limited number of textual modules constrains the amount of words processed at any given time. Insertion of tags/elements into the document. Limited textual processing constrains the possible locations to include only the space currently being processed in the document. 
