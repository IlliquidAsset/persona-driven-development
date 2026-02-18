# System Persona-Driven Development (SPDD) - Twitter Thread v2

1/
I'm a finance guy who builds with AI. Your AI writes code the way a junior analyst builds a pro forma — it assumes nothing goes wrong. I built a framework called SPDD to fix that. Here's what I found. 🧵

2/
Your AI reads API docs the way a fresh MBA reads a pitch deck — it believes every word. No downside scenarios. No stress tests. I call this "Behavioral Debt." Code that looks perfect on paper and falls apart the second it hits production.

3/
Most devs treat APIs like math. Input A → Output B. But legacy systems have trauma. They lie. They have triggers. Treating a 20-year-old ERP like a clean REST API? That's a failure of due diligence.

4/
When your AI reads a Swagger doc, it sees a promise. A senior dev looks at the same system and sees a minefield. We've been trying to make AI "smarter." We should be making it more cynical.

5/
So I stopped handing my AI spec sheets. I give it a personality profile of the system instead — like a CIA dossier for your API. I call it a "System Legend." #AI #SoftwareEngineering

6/
A System Legend covers 5 dimensions:
1. Habits — what it actually does
2. Lies — where the docs are wrong
3. Triggers — what breaks it
4. Trauma — legacy scars
5. Incentives — what it "wants" to do

7/
Don't tell your AI "the API returns a 404." Tell it "this system is an overworked clerk who says 'I don't know' when it's really just too busy to look." Sounds weird? The AI handles it better. Theory of Mind kicks in.

8/
This turns integration into negotiation. Your AI stops blindly pushing data and starts navigating the friction. Like a VC working a messy cap table — you don't force it, you work it.

9/
I tested this on a legacy ledger.

Standard docs → 15% data corruption under load.
System Legend → 0%.

Same AI. It didn't write better code — it just stopped trusting the docs and started anticipating the system's mood swings. #LLM

10/
Here's why it works: LLMs are way better at reasoning about "characters" than following abstract logic. Give it a persona to negotiate with and it thinks about intent, not just syntax. That's the core of SPDD.

11/
I call this "Simulated Seniority." Junior devs follow the manual. Senior devs know where the bodies are buried. A System Legend downloads that institutional memory straight into the AI's context window.

12/
In finance, we price in tail risk. In SPDD, I prompt for it. If your model doesn't account for the chaos of interconnected systems, you're just building another pro forma with no downside scenario.

13/
This evolved from my work on Persona-Driven Development. First I gave the AI a persona. Then I realized — give the TARGET SYSTEM a persona too. Now the AI knows every actor's secrets before it writes a single line of code.

14/
If your AI doesn't understand the personality of your stack, you're not automating development. You're automating the creation of technical debt. That's an expensive mistake. #PromptEngineering

15/
Where this gets interesting: imagine your CI/CD pipeline auto-generating System Legends from error logs and incidents. A living dossier that evolves as your system ages. That's where I'm taking this next.

16/
Stop treating your APIs like math problems. They're counterparties in a negotiation. The results speak for themselves — 15% data corruption down to 0%. Same AI. Same complexity. Different approach.

17/
I wrote up the full SPDD framework, the Legacy Ledger results, and System Legend templates you can use today. If you're done watching your AI trust documentation it shouldn't, start here:

https://github.com/IlliquidAsset/persona-driven-development

18/
What's the worst "lie" your API tells? What's the trauma in your legacy stack that your AI keeps tripping over? I want to hear the horror stories. 👇 #AIdev
