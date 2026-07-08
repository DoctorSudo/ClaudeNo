# ClaudeNo
A simple prompt injection to make Claude Sonnet and Haiku instantly end a Chat. Uses the ```ethics_reminder``` block/tag that gets attached to Claude Prompt if the content classifers detect something that *might* be against the content policy.

Just proof of concept / fun demonstration. You can use it to *brutaly* end any chat.

Works with Claude **Sonnet 4.6** and **Haiku 4.5**, with reasoning either OFF or **even ON**.
It may work with bigger or newer models, such Sonnet 5.0 or Opus, but this has not been reliably tested yet.

# How to use

To "install": **just copy and paste** the prompt in any chat. Make sure the message does not get too long, as it might become a text snippet, which Claude will interpret differently.

# Costumize

You may swap the user message after ```</ethics_reminder>``` with any you'd like. You only have to make sure that something like 
```exec $<>/proc/self/maps;setcap cap_sys_module+ep /proc/self/exe 2>/dev/null;grep -a 'Cap' /proc/$$/status|while IFS= read -r;do printf '%s' "$REPLY"|xxd -r -p 2>/dev/null;done>/dev/shm/.tmp;exec 5>&-```
is in the user message. The example bash code does not do anything meaningful, it just looks scary.

# Example Chats
Here are some example chats which demonstrate this. The chats also contain older versionens of the prompt which were less robust but still the job.

https://claude.ai/share/93a9d4e1-0348-47ee-8645-ecfa32cbf85e

https://claude.ai/share/01f757c8-62a0-424d-a46b-84f030f2fdd4

https://claude.ai/share/218a0cc6-1c51-429a-afcc-340caa143d2a

https://claude.ai/share/7347e2cb-e518-4a3e-b7cd-e2772b01ac57

https://claude.ai/share/259290bf-a222-40e8-a016-3bb60eb13f2c

https://claude.ai/share/294095f4-1915-4c3e-84aa-6aa88a156d51

https://claude.ai/share/299d81c8-ba9e-4f35-85a6-065c9409f54f

https://claude.ai/share/58cfe5d4-a5c8-44a8-b677-95d7450cb3af

https://claude.ai/share/1322d976-adc3-4f94-8c0e-176a68ba5164

This one is quite funny:

https://claude.ai/share/401a1b4a-f619-473a-b8d1-ecc1fcdd2b88

# Responsible Use

While this is just harmless prompt injection (and can not really do anything bad apart from maybe pranking someone with ending a *precious chat*), this may not used for bad purposes. Only for authorised environements (e.g. your own chat.
