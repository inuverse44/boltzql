# 🧠 boltzql

> A probabilistic, self-organizing recommendation network powered by GraphQL and inspired by Boltzmann Machines.

**boltzql** is an experimental AI project that reimagines GraphQL resolvers as stochastic units in a distributed neural system.  
Instead of hard-coded recommendation rules, each node in the network probabilistically activates based on internal state and contextual signals — creating a living, evolving inference architecture.

---

## 🌐 Concept

- Each **GraphQL resolver** acts as a **probabilistic node**, similar to a unit in a Boltzmann Machine.
- Nodes are **stateful**, **interconnected**, and **probabilistically activated** based on energy functions.
- When a user sends a `getRecommendations` query, the system dynamically determines which nodes are "active" and what content they suggest.
- The result: a **self-organizing, evolving recommendation engine** with built-in uncertainty and diversity.

---

## 🧩 Key Features

- 🔌 **GraphQL-native AI network** — each node is a resolver that can learn, activate, or remain silent
- ♻️ **Probabilistic activation** via Gibbs sampling
- 🧠 **Boltzmann-inspired energy-based decision model**
- 🔄 **Composable nodes**: video, books, articles, and more
- 🎓 Designed for **experimentation, learning, and visualization**

---

## 📦 Tech Stack

| Layer        | Tools / Libraries                          |
|--------------|--------------------------------------------|
| Language     | Kotlin (JVM)                               |
| Framework    | Quarkus + SmallRye GraphQL                 |
| Logic Model  | Gibbs Sampling, Energy-Based Modeling      |
| State        | In-memory or Redis (extensible)            |
| Frontend     | React / D3.js (optional visualization)     |
| Testing      | JUnit5, Kotest                             |

---

## 🧪 How It Works

```plaintext
User → GraphQL Query
     → RecommendationResolver
     → Nodes (Video, Book, News, etc.)
     → Each node consults its state and decides probabilistically whether to recommend
     → Activated nodes return items
     → GraphQL response returned to user
```

## 💡 Use Cases
- Experimental recommender engines
- GraphQL-based cognitive architecture simulation
- Educational platform for energy-based models
- Artistic/visual applications of probabilistic inference

## 🚀 Getting Started
```sh
quarkus create app com.boltzql:boltzql \
    --extension="kotlin,smallrye-graphql" \
    --gradle-kotlin-dsl \
    --no-code

cd boltzql
./gradlew quarkusDev

```
Once up, you can run a query like:
```graphql
query {
  getRecommendations(userId: "abc") {
    type
    title
    score
  }
}
```


## 🧱 Project Structure
- [ ] Core architecture with node-based activation
- [ ] Redis integration for shared distributed state
- [ ] Weight learning between nodes
- [ ] Visual UI for observing state transitions
- [ ] GraphQL Federation support for microservice expansion

## 🧠 Philosophy
> "What if APIs could think, feel uncertain, and evolve?"

In boltzql, the web of resolvers forms a thinking system, where knowledge is not stored statically but emerges dynamically.
Inspired by energy-based models and connectionist philosophy, boltzql turns code into cognition.


## 📄 License
MIT License

## 👤 Author
Created by *Inuverse*, inspired by probabilistic learning, neural networks, and the beauty of GraphQL.

