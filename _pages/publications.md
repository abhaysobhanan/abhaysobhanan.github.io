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

<li> Sobhanan A, Charkhgard H, Kwon C. "Arc Routing Problems with Multiple Trucks and Drones: A Hybrid Genetic Algorithm". arXiv preprint arXiv:2508.18105. 2025 August 25.<span style="display: inline-block; width: 10px;"></span>
    <details style="display: inline-block; font-size: 80%;">
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; cursor: pointer;"><em>abstract</em></summary>
    <br>
    <div class="justified-text">
    Arc-routing problems underpin numerous critical field operations, including power-line inspection, urban police patrolling, and traffic monitoring. In this domain, the Rural Postman Problem (RPP) is a fundamental variant in which a prescribed subset of edges or arcs in a network must be traversed. This paper investigates a generalized form of the RPP, called RPP-mTD, which involves a fleet of multiple trucks, each carrying multiple drones. The trucks act as mobile depots traversing a road network, from which drones are launched to execute simultaneous service, with the objective of minimizing the overall makespan. Given the combinatorial complexity of RPP-mTD, we propose a Hybrid Genetic Algorithm (HGA) that combines population-based exploration with targeted neighborhood searches. Solutions are encoded using a two-layer chromosome that represents: (i) an ordered, directed sequence of required edges, and (ii) their assignment to vehicles. A tailored segment-preserving crossover operator is introduced, along with multiple local search techniques to intensify the optimization. We benchmark the proposed HGA against established single truck-and-drone instances, demonstrating competitive performance. Additionally, we conduct extensive evaluations on new, larger-scale instances to demonstrate scalability. Our findings highlight the operational benefits of closely integrated truck-drone fleets, affirming the HGA's practical effectiveness as a decision-support tool in advanced mixed-fleet logistics.
    </div>
    </details>
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; font-size: 80%"> 
    <a href="https://arxiv.org/abs/2508.18105" style="text-decoration: none; color: inherit;">
    arXiv:2508.18105
    </a> 
    </summary>
</li>

</ol>

# Journal Articles

<ol reversed>

<li> Sobhanan A, Charkhgard H, Dayarian I. "Equity-Driven Workload Allocation for Crowdsourced Last-Mile Delivery". Production and Operations Management, forthcoming.<span style="display: inline-block; width: 10px;"></span>
    <details style="display: inline-block; font-size: 80%;">
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; cursor: pointer;"><em>abstract</em></summary>
    <br>
    <div class="justified-text">
    Crowdshipping, a rapidly growing approach in Last-Mile Delivery (LMD), relies on independent crowdworkers for delivery orders. Building a sustainable network of crowdshippers is essential for the survival and growth of such systems, while their participation is primarily motivated by fair pay. Additionally, the financial well-being of crowdworkers is sensitive to fair compensation, especially for those who depend on crowdwork as their main source of income. Therefore, equitable workload allocation and compensation mechanisms in crowdsourcing platforms will benefit both platforms and crowdworkers. We aim to answer several questions gig-economy platforms interested in fair pay may ask: How to measure equity, assess the cost benefits, and manage potential drawbacks? Our main contribution is the proposal of a practical equity-oriented framework tailored to crowdshipping within an LMD environment. This framework draws inspiration from the real-world operations of a group of crowdshipping platforms and operates in real-time. At its core is a bi-objective optimization process that balances equity and cost, aiming to address the study's main research questions. Built on a theoretical foundation, it enables the use of various equity measures and allows us to identify the equity measure that most reliably explores the trade-offs between cost and equity. We show that even a marginal sacrifice in cost efficiency (e.g., 2.5%) can significantly improve equity, potentially up to 39%. We provide actionable recommendations for practitioners, offering insights into selecting equity measures. We demonstrate that significant improvements in pay equity can be achieved with minimal increases in company's operational costs. Our experiments reveal that the best level of equity is achieved when the pool of employed crowdshippers is kept as small as possible. We quantify the loss of high and low-performing crowdshippers as the crowdshipper pool size increases, offering further insights for workforce management.
    </div>
    </details>
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; font-size: 80%"> 
    <a href="https://optimization-online.org/?p=27199" style="text-decoration: none; color: inherit;">
    preprint
    </a> 
    </summary>
</li>

<li> Mahmoudinazlou S, Sobhanan A, Charkhgard H, Eshragh A, Dunn G. (2025). "Deep Reinforcement Learning for Dynamic Order Picking in Warehouse Operations". Computers & Operations Research, 107112. <span style="display: inline-block; width: 10px;"></span>
    <details style="display: inline-block; font-size: 80%;">
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; cursor: pointer;"><em>abstract</em></summary>
    <br>
    <div class="justified-text">
    Order picking is a pivotal operation in warehouses that directly impacts overall efficiency and profitability. This study addresses the dynamic order picking problem, a significant concern in modern warehouse management, where real-time adaptation to fluctuating order arrivals and efficient picker routing are crucial. Traditional methods, which often depend on static optimization algorithms designed around fixed order sets for the picker routing, fall short in addressing the challenges of this dynamic environment. To overcome these challenges, we propose a Deep Reinforcement Learning (DRL) framework tailored for single-block warehouses equipped with an autonomous picking device. By dynamically optimizing picker routes, our approach significantly reduces order throughput times and unfulfilled orders, particularly under high order arrival rates. We benchmark our DRL model against established algorithms, utilizing instances generated based on standard practices in the order picking literature. Experimental results demonstrate the superiority of our DRL model over benchmark algorithms. For example, at a high order arrival rate of 0.09 (i.e., 9 orders per 100 units of time on average), our approach achieves an order fulfillment rate of approximately 98%, compared to the 82% fulfillment rate observed with benchmarking algorithms. We further investigate the integration of a hyperparameter in the reward function that allows for flexible balancing between distance traveled and order completion time. Finally, we demonstrate the robustness of our DRL model on out-of-sample test instances.
    </div>
    </details>
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; font-size: 80%"> 
    <a href="https://arxiv.org/abs/2408.01656" style="text-decoration: none; color: inherit;">
    arXiv:2408.01656
    </a> 
    </summary>
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; font-size: 80%"> 
    <a href="https://github.com/Sasanm88/DRL-Order-Picking" style="text-decoration: none; color: inherit;">
    code
    </a> 
    </summary>
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; font-size: 80%"> 
    <a href="https://doi.org/10.1016/j.cor.2025.107112" style="text-decoration: none; color: inherit;">
    https://doi.org/10.1016/j.cor.2025.107112
    </a> 
    </summary>
</li>


<li> Sobhanan A, Park J, Park J, Kwon C. (2025). "Genetic Algorithms with Neural Cost Predictor for Solving Hierarchical Vehicle Routing Problems". Transportation Science, 59(2), 322-339. <span style="display: inline-block; width: 10px;"></span>
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
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; font-size: 80%"> 
    <a href="https://doi.org/10.1287/trsc.2023.0369" style="text-decoration: none; color: inherit;">
    https://doi.org/10.1287/trsc.2023.0369
    </a> 
    </summary>
</li>


<li> Golui S, Pal C, Manikandan R, Sobhanan A. (2024). "Optimal control of a dynamic production-inventory system with various cost criteria". Annals of Operations Research, 337(1), 75-103. <span style="display: inline-block; width: 10px;"></span>
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
    </details>
    <summary style="display: inline-block; border: 1px solid #ccc; padding: 3px 8px; border-radius: 5px; font-size: 80%"> 
    <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4915810" style="text-decoration: none; color: inherit;">
    preprint
    </a> 
    </summary>
</li>

</ol>