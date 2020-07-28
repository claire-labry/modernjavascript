# what's the DOM?

    NOTE: DOM stands for document object model
    NOTE: Tree of nodes/elements created by the browser
    NOTE: JavaScript can be used to read/write/manipulate to the DOM
    NOTE: Object Oriented Representation

# Traversing the DOM
    NOTE: traversing basically means moving up & down the DOM. 
    NOTE: nodeType gives types of a node: 1 - Element, 2 - Attribute (deprecated), 3 - Text node, 8 - Comment, 9 - Document itself, 10 - Doctype 

# creating elements

    NOTE: method is document.createElement() 
        ie:
        
        <!-- create element -->
            const li = document.createElement('li');

        <!--add class to element  -->
            li.className = 'collection-item';
        
        <!-- add id to element -->
            li.id = 'new-item';
        
        <!-- add attribute -->
            li.setAttribute('title', 'New Item');
        
        <!-- create text node & append -->
            li.appendChild(document.createTextNode('Hello World'));
        
        <!-- create new link element -->
            const link = document.createElement('a');
        
        <!-- add classes -->
            link.className = 'delete-item secondary-content';

        <!-- add icon html -->
            link.innerHTML = '<i class='fa fa-remove'></i>'
        
        <!-- append link to li -->
            li.appendChild(link);
        
        <!-- append li ad child to ul -->
            document.querySelector('ul-collection').appendChild('li')
    
    NOTE: this will create a new li element called Hello World and append it to the list shown in the folder of js_sandbox1, a link element has been appended to the li element

