# Tabs settings

This is a very simple script to implement tabs on your site. You just need to insert the necessary data and everything will work. It can be used for several tabs on one page, different in structure and content.

### HTML structure

    <div class="tab__parent">
        <div class="tab tab__active">1</div>
        <div class="tab">2</div>
        <div class="tab">3</div>
        <div class="tab">4</div>
    </div>

    <div class="tab__content">1</div>
    <div class="tab__content">2</div>
    <div class="tab__content">3</div>
    <div class="tab__content">4</div>
    
Ideal structure of the HTML code (class names can be changed). The style.css file has all the necessary classes + animation (it can be changed to any other).

### JS settings

These settings are suitable for the example given above in the NTTL structure. The name of the classes can be changed, but the structure must be respected.

    <script>
        tabs({
            parentSelector: '.tap__parent',
            tabSelector: '.tab',
            contentSelector: '.tab__content',
            activeClass: 'tab__active',
        });
    </script>
    
1. **parentSelector** is the class selector of the parent of the tabs.
2. **tabSelector** is a class of tabs themselves, after clicking on which the content changes.
3. **contentSelector** is the tab content class.
4. **activeClass** is the class that indicates the activity of a particular tab.
    
