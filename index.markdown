---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
image: "/assets/images/logo.jpg"
---

<div class="warning" style='background-color:#E9D8FD; color: #69337A; border-left: solid #805AD5 4px; border-radius: 4px; padding:0.7em;'>
    <span>
        <p style='margin-top:1em; text-align:center'>
            <b>Site content not yet finalized.</b>
        </p>
        <p style='margin-left:1em;'>
            Please note that the content of this page is still under construction.
            <br><br>
            More info will follow.
        </p>
    </span>
</div>

![Institute of Computer Science at the University of St. Gallen]({{ page.image }}){: style="float: right; padding-top: 10px; padding: 40px; max-width: 200px"}

## The Challenge

Measure your performance using our provided script:

```
evaluate_fod_qa
```

This script will apply your model on the test data.

## How This Dataset Advances Research in Financial Text Processing

## Structure of and Access to the Dataset

## Collaboration on the Dataset

We welcome everybody to directly participate in improving `FOD-QA` by contributing their competency and time by the following means:

1) Finding new questions to be added to the set of questions (currently 20).
2) Engaging in discussions about new questions to be added.
3) Annotating data.

You can suggest a new question to be added by opening an issue in our [GitHub repository](https://github.com/DS-NLP-HSG/DS-NLP-HSG.github.io).

For all of these tasks, we require you to participate in a short 20-minute vetting call with one of our core team members. We will provide you with a short 5-question task that tests whether you can find information from an annual report based on simple question such as "What is the revenue of company X in the year Y?"

If you would like to participate and get to know us, contact us using the contact information in the website footer.

## Ensuring Data Quality

Data quality is our first priority. 

1) We vet all data annotators. We do not use Amazon Mechanical Turk or other providers. Our annotators have sufficient domain knowledge to perform their tasks and are not only financially motivated.
2) We employ a quadruple-annotation scheme to detect inter-annotator disagreement. Any disagreement among annotators leads to a manual review by the core team, and the resulting final annotation will be documented with several sentences of explanation of why a certain annotation was favored over the competing alternatives. One annotator can perform an annotation only once.