<script>
  (function() {
    // Function to append parameters to the URL
    function appendParams() {
      const paramsToAdd = {
        font-family: "system-ui,sans-serif",
        font-size: ".875",
        link-color: "cc000"
      };

      const url = new URL(window.location.href);
      Object.entries(paramsToAdd).forEach(([key, value]) => {
        url.searchParams.set(key, value);
      });
      window.history.replaceState({}, document.title, url);
    }

    // Create a MutationObserver to monitor for Docsify content changes
    const observer = new MutationObserver(function(mutationsList, observer) {
      // Check if Docsify has rendered the body content
      const docsifyRendered = document.querySelector('.content');
      
      // If Docsify content is detected and the URL hasn't been modified yet
      if (docsifyRendered && !window.location.search.includes('param1')) {
        appendParams();
        observer.disconnect();  // Stop observing once params are added
      }
    });

    // Start observing the document for changes (looking for Docsify content)
    observer.observe(document.body, { childList: true, subtree: true });
  })();
</script>
  
# Schedule

## :fas fa-calendar fa-pull-left: [Week 1 (May 9 - 15)](module-01)
**What is usability and user experience design?**  
:fas fa-desktop fa-fw: [Introduction to UX Design](https://docs.google.com/presentation/d/e/2PACX-1vRnnRFelgw1ksq_p8Eryg3dnyLCRRLPf5fBgdwdv9p-tCIwcxqWvzDGrGbjxGHL7HqEJVpmV26ntk3a/pub?start=false&loop=false&delayms=3000)   
:fas fa-book fa-fw: [Usability 101: Introduction to Usability](https://www.nngroup.com/articles/usability-101-introduction-to-usability/) 

## :fas fa-calendar fa-pull-left: [Week 2 (May 16 - 22)](module-02)
**What does a holistic user experience design process look like?**  
:fas fa-keyboard fa-fw: [Course Reflection Log](https://sso.canvaslms.com/courses/1924881/assignments/14377752) <span class='badge'> Fri Aug 3rd 11:59pm PDT</span>  
:fas fa-desktop fa-fw: [The Process of UX Design](https://docs.google.com/presentation/d/e/2PACX-1vRnnRFelgw1ksq_p8Eryg3dnyLCRRLPf5fBgdwdv9p-tCIwcxqWvzDGrGbjxGHL7HqEJVpmV26ntk3a/pub?start=false&loop=false&delayms=3000)   
:fas fa-book fa-fw: [The Evolution of UX Process Methodology](https://uxplanet.org/the-evolution-of-ux-process-methodology-47f52557178b)  

## :fas fa-calendar fa-pull-left: [Week 3 (May 23 - 29)](module-03)
**How to make more strategic design decisions?**  
:fas fa-keyboard fa-fw: [Journey Map](https://sso.canvaslms.com/courses/1924881/assignments/14377756) <span class='badge'> Tue Jun 12th 11:59pm PDT</span>  
:fas fa-folder fa-fw: [Informed Consent Materials](https://sso.canvaslms.com/courses/1924881/files/folder/Downloads/Informed%20Consent)  
:fas fa-desktop fa-fw: [Strategic UX Design](https://docs.google.com/presentation/d/e/2PACX-1vRnnRFelgw1ksq_p8Eryg3dnyLCRRLPf5fBgdwdv9p-tCIwcxqWvzDGrGbjxGHL7HqEJVpmV26ntk3a/pub?start=false&loop=false&delayms=3000)   
:fas fa-book fa-fw: [What is a User Journey Map?](https://www.aytech.ca/blog/user-journey-map/)  

## :fas fa-calendar fa-pull-left: [Week 4 (May 30 - Jun 5)](module-04)
**How to explore the problem space?**  
:fas fa-desktop fa-fw: [Prototyping](https://docs.google.com/presentation/d/e/2PACX-1vRnnRFelgw1ksq_p8Eryg3dnyLCRRLPf5fBgdwdv9p-tCIwcxqWvzDGrGbjxGHL7HqEJVpmV26ntk3a/pub?start=false&loop=false&delayms=3000)   
:fas fa-book fa-fw: [The Skeptic’s Guide To Low-Fidelity Prototyping](https://www.smashingmagazine.com/2014/10/the-skeptics-guide-to-low-fidelity-prototyping/)  
:fas fa-users fa-fw: In-class office hours (tentative)  

## :fas fa-calendar fa-pull-left: [Week 5 (Jun 6 - 12)](module-05)
**How to plan, conduct, and summarize usability tests?**  
:fas fa-desktop fa-fw: [Usability Testing](https://docs.google.com/presentation/d/e/2PACX-1vRnnRFelgw1ksq_p8Eryg3dnyLCRRLPf5fBgdwdv9p-tCIwcxqWvzDGrGbjxGHL7HqEJVpmV26ntk3a/pub?start=false&loop=false&delayms=3000)   
:fas fa-book fa-fw: [The Art of Guerrilla Usability Testing](http://www.uxbooth.com/articles/the-art-of-guerrilla-usability-testing/)  
:fas fa-users fa-fw: In-class office hours (tentative)
