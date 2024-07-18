---
layout: archive
# title: "Publications"
permalink: /publications/
author_profile: true
---

<style>
.justified-text {
    text-align: justify;
}
</style>

<!-- {% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %} -->


<!-- {% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %} -->


# Articles under Review
<ol reversed>
<li> [Submitted, Manufacturing & Service Operations Management] Sobhanan A, Charkhgard H, Dayarian I. "Equity-Driven Workload Allocation for Crowdsourced Last-Mile Delivery".<span style="display: inline-block; width: 10px;"></span>
    <details style="display: inline-block; font-size: 80%;">
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; cursor: pointer;"><em>abstract</em></summary>
    <br>
    <div class="justified-text">
    To be available soon.
    </div>
    </details>
</li>

</ol>

# Journal Articles

<ol reversed>

<li> [Accepted, Transportation Science] Sobhanan A, Park J, Park J, Kwon C. "Genetic Algorithms with Neural Cost Predictor for Solving Hierarchical Vehicle Routing Problems". arXiv preprint arXiv:2310.14157. 2023 Oct 22.<span style="display: inline-block; width: 10px;"></span>
    <details style="display: inline-block; font-size: 80%;">
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; cursor: pointer;"><em>abstract</em></summary>
    <br>
    <div class="justified-text">
    When vehicle routing decisions are intertwined with higher-level decisions, the resulting optimization problems pose significant challenges for computation. Examples are the multi-depot vehicle routing problem (MDVRP), where customers are assigned to depots before delivery, and the capacitated location routing problem (CLRP), where the locations of depots should be determined first. A simple and straightforward approach for such hierarchical problems would be to separate the higher-level decisions from the complicated vehicle routing decisions. For each higher-level decision candidate, we may evaluate the underlying vehicle routing problems to assess the candidate. As this approach requires solving vehicle routing problems multiple times, it has been regarded as impractical in most cases. We propose a novel deep-learning-based approach called Genetic Algorithm with Neural Cost Predictor (GANCP) to tackle the challenge and simplify algorithm developments. For each higher-level decision candidate, we predict the objective function values of the underlying vehicle routing problems using a pre-trained graph neural network without actually solving the routing problems. In particular, our proposed neural network learns the objective values of the HGS-CVRP open-source package that solves capacitated vehicle routing problems. Our numerical experiments show that this simplified approach is effective and efficient in generating high-quality solutions for both MDVRP and CLRP and has the potential to expedite algorithm developments for complicated hierarchical problems. We provide computational results evaluated in the standard benchmark instances used in the literature.
    </div>
    </details>
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; font-size: 80%"> 
    <a href="https://arxiv.org/abs/2310.14157" style="text-decoration: none; color: inherit;">
    arXiv:2310.14157
    </a> 
    </summary>
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; font-size: 80%"> 
    <a href="https://github.com/abhaysobhanan/GANCP" style="text-decoration: none; color: inherit;">
    code
    </a> 
    </summary>
</li>


<li> Golui S, Pal C, Manikandan R, Sobhanan A. "Optimal control of a dynamic production-inventory system with various cost criteria". Annals of Operations Research. 2023 Nov 27:1-29. <span style="display: inline-block; width: 10px;"></span>
    <details style="display: inline-block; font-size: 80%;">
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; cursor: pointer;"><em>abstract</em></summary>
    <br>
    <div class="justified-text">
    In this article, we investigate the dynamic control problem of a production-inventory system. Here, demands arrive at the production unit according to a Poisson process and are processed in an FCFS manner. The processing time of the customer’s demand is exponentially distributed. Production manufacturers produce items on a make-to-order basis to meet customer demands. The production is run until the inventory level becomes sufficiently large. We assume that the production time of an item follows an exponential distribution and that the amount of time for the produced item to reach the retail shop is negligible. In addition, we assume that no new customer joins the queue when there is void inventory. Moreover, when a customer is waiting in an infinite FIFO queue for service, he/she does not leave the queue even if the inventory is exhausted. This yields an explicit product-form solution for the steady-state probability vector of the system. The optimal policy that minimizes the discounted/average/pathwise average total cost per production is derived using a Markov decision process approach. We find an optimal policy using value/policy iteration algorithms. Numerical examples are discussed to verify the proposed algorithms.
    </div>
    </details>
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; font-size: 80%"> 
    <a href="https://doi.org/10.1007/s10479-023-05716-5" style="text-decoration: none; color: inherit;">
    https://doi.org/10.1007/s10479-023-05716-5
    </a> 
    </summary>
</li>

</ol>


# Refereed Conference Proceedings
<ol reversed>

<li> Sobhanan A, Mahmoudinazlou S, Charkhgard H, Kwon C. "A branch-and-price algorithm for emergency humanitarian logistics with a mixed truck-drone fleet". Proceedings of the IISE Annual Conference & Expo 2024. [<b>Best Paper Award Finalist</b>, Operations Research Division] <span style="display: inline-block; width: 10px;"></span>
    <details style="display: inline-block; font-size: 80%;">
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; cursor: pointer;"><em>abstract</em></summary>
    <br>
    <div class="justified-text">
    Humanitarian aid distribution often prioritizes rapid relief operations or emergency services under time constraints, as opposed to commercial transportation problems, where the primary objective is to minimize operational costs. 
    Drones can offer immense potential to achieve this goal by leveraging their aerial mobility. 
    Specifically, drones can surpass ground transportation and navigate directly through disrupted or inaccessible roads, ensuring the quickest path to deliver aid where the ground vehicle may face obstacles. 
    However, drones have limitations in terms of flying range and load capacity. To effectively provide time-sensitive emergency services, combining a ground vehicle with one or more aerial vehicles enhances coverage. 
    Our approach integrates a truck as a mobile depot for multiple drones, where a drone battery is replenished on landing after a flight, and the fleet operates in tandem to serve the locations visited. 
    We formulate a mixed-integer linear programming (MILP) model to maximize the weighted sum of locations served by this mixed truck-drone fleet under time constraints. 
    We further develop a branch-and-price algorithm to solve this problem, where the pricing subproblem is solved using dynamic programming recursions with dominance rules. 
    Our results demonstrate the computational superiority of this method compared to a commercial optimization solver and its potential for expediting aid distribution during an emergency.
    </div>
</li>

</ol>