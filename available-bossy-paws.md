---
title: "Available Bossy Paws"
permalink: /available-bossy-paws
---

<iframe id="iframe-03" frameborder="0" sandbox="allow-scripts allow-same-origin allow-forms allow-popups allow-presentation allow-top-navigation" src="javascript: window.frameElement.getAttribute(&quot;srcdoc&quot;);" srcdoc="<script>window.onmessage = function(event) {event.source.postMessage({iframeId: event.data, scrollHeight: document.body.getBoundingClientRect().height || document.body.scrollHeight}, event.origin);};</script><body style='margin: 0'>
        <pet-scroller
            type='[]'
            age='[]'
            limit=&quot;48&quot;
            hidebreed
            status=&quot;adoptable&quot;
            petlisttitle=&quot;BOSSY PAWS &quot;
            organization=&quot;GA1026&quot;
            apibase=&quot;https://api.petfinder.com&quot;
            petfinderurl=&quot;https://www.petfinder.com&quot;
            accesstoken=&quot;eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJhdWQiOiJtd1NmUDQ1SEpPckFSS0RkVGM1M3JGSjNHVTJIdnk0SUxVSGR5Y3NnNGpURzRCVHIzdCIsImp0aSI6IlhVQ0VuSU84VXVranBJQnJtUDJ3NndpVzZBNUJSOUFDTHg4WHAzejIiLCJpYXQiOjE2NDY3Njk4NjIsIm5iZiI6MTY0Njc2OTg2MiwiZXhwIjo0ODAyNDQzNDYyLCJzdWIiOiIxMDE4NTEwNCIsInNjb3BlcyI6W119.POUKzyDWzzNMq9Nq6b4ON25QyVgYaZ6SA-kZ3QHN2xoDY1wLeRvA2Z5jXy9Jsad7egwPGc9mPXBCgts8J3wK5TxFlEthSzbCte1uqqQVQUsehx2LTINUOSP_kvHj70ljuBZk-fxQAHGizm1MwEAopQ9krw2LhoMBN1U8ofo8Xekm7LN7TfAmL161LwS9Zsm0J9lJ5O_2zjHCJdeOjxXIPjJtI7JXYHqiC2bZd28xVnZQaNnYFnW4iRpsmMwjP8q-V8-Nocjfa7jxXW1FEf2LN8h9P2G27Q7RDMLmXscwxVc_nR3K-6PB_Eo75nqfk6kNemsg2_z3m0zHKWpm8nYXIA&quot;>
        </pet-scroller>

        <script src=&quot;https://www.petfinder.com/assets/widgets/scripts/main-widgets-web.js&quot;>
        </script>
    
    </body>" style="width: 100%; overflow: visible; height: 1000px; transition: height .5s ease-in-out, opacity .5s ease-in; opacity: 0;"></iframe>

<script>
        const petScroller = document.getElementById("iframe-03");
        window.addEventListener("message", (event) => {
                const eventData = event.data;
                petScroller.style.height = eventData.scrollHeight;
                petScroller.style.opacity = "1";
        });
        setInterval(() => petScroller.contentWindow.postMessage("iframe-03"), 1000);
</script>
