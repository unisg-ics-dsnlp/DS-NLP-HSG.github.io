---
layout: post
title: "2022-10-23: FOD-QA Benchmark Challenge Invitation"
date: 2022-10-23
categories: post
tags: datasetfodqa
is_series: true
series_title: "datasetfodqa"
---
## Abstract

FOD-QA provides a benchmark for open-domain question answering for the financial domain.

Existing natural language processing benchmarks in the financial domain often on sentiment analysis. Question answering is not yet covered.

We constructed a benchmark that consists purely of questions from the financial domain. The questions chosen are relevant to the financial industry, as indicated by their frequency of use in real-corps corpora. 

## Motivation

Open-domain question answering methods advanced significantly in recent years, mainly due to contextualized word embeddings \parencite{KarpukhinOguzMinLewisWuEdunovChenYih_DensePassageRetrievalForOpenDomainQuestionAnsweringDPR_2020}.

\cite{YangUyHuang_FinbertAPretrainedLanguageModelForFinancialCommunications_2020} demonstrate with the scale of their financial data collection that the domain produces vast amounts of text. This textual information is unstructured and often factual, making it a candidate for open-domain question answering.

Natural language processing research in the financial domain frequently analyzes the sentiment of financial texts  \parencite{GuKurov_InformationalRoleOfSocialMediaEvidenceFromTwitterSentiment_2020} as well as on numerical reasoning and text from tables \parencite{ZhuLeiHuangWangZhanLvFengChua_TAT-QA_AQuestionAnsweringBenchmarkOnAHybridOfTabularAndTextualContentInFinance_2021}. 

FOD-QA is a dataset that bridges the gap between a missing open benchmark for financial open-domain question answering the extensive use of

## Benchmark Description

The benchmark contains $4,000$ question-answer pairs. Those stem from $200$ annual reports, with $20$ answered questions per annual report. The annual reports were authored by $100$ different S\&P 500 corporations, one for the financial year 2020 and one for the financial year 2021 each.

## Evaluation Metrics

\textbf{Taken from here:} \href{https://www.deepset.ai/blog/metrics-to-evaluate-a-question-answering-system}{https://www.deepset.ai/blog/metrics-to-evaluate-a-question-answering-system}

\textbf{TODO: NEEDS TO BE REWORDED}

Recall measures how many times the correct document was among the retrieved documents. For a single query, the output is binary: either a document is contained in the selection, or it is not. Over the entire dataset, the recall score amounts to a number between zero (no query retrieved the right document) and one (all queries retrieved the right documents).

In contrast to the recall metric, mean reciprocal rank takes the position of an answer (the “rank”) into account. It does this to account for the fact that a query elicits multiple responses of varying relevance. Like recall, MRR can be a value between zero (no matches) and one (the system retrieved the correct document as the top result for all queries).
\section{Evaluation Results}

\textbf{TODO}

## Acknowledgments

\textbf{TODO}

{% if page.is_series == true %}
    {% assign posts = site.posts | where: "is_series", true | where: "series_title", page.series_title | sort: 'date' %}
    {% if posts.size > 1 %}
        
<h3 class="text-success p-3 pb-0">Read More From the {{ page.series_title }} Series</h3>
        {% for post in posts %}
                {% if post.title == page.title %}
<p class="nav-link bullet-pointer mb-0">{{ post.title }}</p>
                {% else %}
<a class="nav-link bullet-hash" href="{{ post.url }}">{{ post.title }}</a>
                {% endif %}
        {% endfor %}
    {% endif %}
{% endif %}