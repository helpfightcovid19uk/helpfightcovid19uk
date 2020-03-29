---
layout: default
title: FAQ
faqs:
  -
    q: "Why are you doing this?"
    a: "We strongly support our amazing NHS staff and know they don’t have all the resources they need to manage what’s happening at the moment. We have also been inspired by the amazing acts of kindness from others during this time and we want to play our part to help front-line workers."
  -
    q: "How can I help?"
    a: "Go to Facebook, ‘Like’ our page, and share it to your network and any groups you’re part of. The more people clicking our links – and using these to buy from Amazon – means the more we can raise for the NHS. If you want to buy something, just click our link and complete your purchase. Simples."
  -
    q: "How will you donate the money to the NHS?"
    a: "Like most things at the moment – they’re happening so fast we don’t have all the answers. We are in the process of contacting NHS Charities Together – a collection of 140+ charities – to start the conversation about how we make sure we get the money where it needs to be. "
  -
    q: "What happens to my data?"
    a: "We do not have access to any of your personal data. The only information we receive is the number of people who click our links and make purchases. It is completely anonymous who has bought what. All of this falls under Amazon’s data protection and GDPR compliance. "
  -
    q: "Are you just trying to make a profit from this situation?"
    a: "There is no intention to profiteer from what’s happening. We’ve seen other sites doing so and we are not like them. We take 10p from every £1 to cover running costs, managing the website, social media support, graphic design etc., and will constantly review this to see if we can reduce costs further."
---

<div id="accordion" class="faqs">

{% for faq in page.faqs %}

<div class="card">
	<div class="card-header" id="heading{{ forloop.index }}">
		<h5 class="mb-0">
			<button class="btn btn-link{% unless forloop.first %} collapsed{% endunless %}" data-toggle="collapse" data-target="#collapse{{ forloop.index }}" aria-expanded="true" aria-controls="collapse{{ forloop.index }}">
{{ faq.q }}
			</button>
		</h5>
	</div>

	<div id="collapse{{ forloop.index }}" class="collapse{% if forloop.first %} show{% endif %}" aria-labelledby="heading{{ forloop.index }}" data-parent="#accordion">
		<div class="card-body">
			<div class="card-text">
{{ faq.a }}
			</div>
		</div>
	</div>
</div>

{% endfor %}

	
</div>