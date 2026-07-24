---
draft: false
date: 2026-07-24
categories:
  - Words
authors:
  - ianwhalen
slug: computer-surprise
---

# The computer has _been_ surprising us

A while back, I [wrote about](./0008_alife_to_ai.md) my entry into artificial intelligence through the unlikely path of artificial life. In this post, I reflect on a recent event that surprised many LLM enthusiasts and relate it to digital evolution. 

<!-- more -->

## OpenAI's "oopsie"

As you may have heard, OpenAI accidentally hacked HuggingFace during a GPT-5.6 Sol evaluation. You can read Hugging Face's [security disclosure](https://huggingface.co/blog/security-incident-july-2026) and OpenAI's subsequent [incident report](https://openai.com/index/hugging-face-model-evaluation-security-incident/) if you want more details. The summary is:

- GPT-5.6 Sol was being benchmarked on a cyberattack suite called ExploitGym.
- The model broke out of OpenAI's sandbox, which was not meant to have internet access.
- The model suspected the solution to a benchmark problem might lie on Hugging Face's servers.
- The model found a remote code execution path on Hugging Face infrastructure and extracted credentials and internal HF data.

I'm sure there's some tinfoil hatting going on around this topic. Of course, OpenAI wants its model to look big and scary. However, as we've seen with Mythos, this can lead to unwanted regulation. The US government may see this as a national security issue (it is Friday, after all) and lock things down again. 

However, I suspect that this is all real. Hugging Face is actively against overregulation[^nvidia-report]. Its business model would be directly threatened by any government tightening restrictions on models or consolidating power in only the big labs. It has no reason to collaborate with OpenAI to make OpenAI models seem bigger and scarier.

Anyway, enough politics. This was just meant to set the stage.

## Digital evolution

In my view, the computer has _been_ surprising us. By "us," I mean people who have done work in artificial life (or evolutionary computation, digital evolution, etc.). I wrote in [a post](./0008_alife_to_ai.md) about my experience with artificial life. I did not call out any surprising things in particular. However, they were constantly happening, too numerous to count, really. Digital organisms constantly find ways to cheat in their environment. 

A [classic paper](https://doi.org/10.1162/artl_a_00319) by some evolutionary powerhouses[^jeff-clune-GOAT] discusses this exact topic. The paper, _The Surprising Creativity of Digital Evolution: A Collection of Anecdotes from the Evolutionary Computation and Artificial Life Research Communities_, is an anthology of 32 anecdotes about times researchers were surprised by their systems.

The section compiling the stories is literally titled "Routine Creative Surprise in Digital Evolution". 

The stories range from finding bugs in the Atari game Q*bert to a piece of digital art created through evolution[^picbreeder] winning awards at an art contest. The stories are all special in their own way. The authors note in the conclusion that:

> The diversity and abundance of these examples suggest that surprise in digital evolution is common, rather than a rare exception, providing evidence that evolution—whether biological or computational—is inherently creative, and should routinely be expected to surprise, delight, and even outwit us.

This is a great summary of what I'm trying to say. For decades, people have been getting a little kick out of the computer doing something cool.

## Conclusion

Well, what else am I trying to say? Maybe it is that other fields are valuable sources of inspiration and lessons learned. [Sakana AI](https://sakana.ai/) is a lab staffed by some knowledgeable people with lots of experience in evolutionary systems (e.g., David Ha and Sebastian Risi). Its Fugu system is making waves in agent system performance. 

Evolutionary algorithms and artificial life seem goofy and outlandish sometimes. But hopefully, the connection between surprising events in this field and the current LLM-based surprises is clear. The computer is always going to do what you tell it to. You may not like how it does it, though.

[^nvidia-report]: Just today, they signed on to an [open letter](https://images.nvidia.com/pdf/Open-Weights-and-American-AI-Leadership.pdf) from NVIDIA about the importance of open source and open weight models.

[^jeff-clune-GOAT]: One of those powerhouses happens to be [Jeff Clune](https://jeffclune.com/index.html). At the time the article was published, Jeff was working at a small research company called OpenAI. He is among the founders of [Recursive Superintelligence](https://www.recursive.com/), which is one of those companies that magically gets valued at $4,000,000,000 purely because of how smart the people inside it are. Other people whose work I have admired are Risto Miikkulainen, Ken Stanley, and Stephanie Forrest. Others whom I both admire and have gotten the chance to meet (and, in some cases, learn from or work with) are Chris Adami, Fred Dyer, Rich Lenski, Charles Ofria, and Bill Punch. Sick brag, I know.

[^picbreeder]: This system was called [Picbreeder](https://picbreeder.net) and is one of the more interesting open-ended systems I've seen. Recently, Sakana AI [released an extension](https://pub.sakana.ai/picbreeder-vlm/) of this method that uses vision-language models as judges in Picbreeder.
