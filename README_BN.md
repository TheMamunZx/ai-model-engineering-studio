# AI Model Engineering Studio — বাংলা গাইড

Design reproducible model experiments and training/inference pipelines with data governance, measurable evaluation, and realistic compute constraints.

## ব্যবহারের নিয়ম

এই Repository-তে একটি মাত্র Selectable Master Skill আছে: `ai-model-engineering-studio`। বাকি 5টি Specialist Module তার `references/` ফোল্ডারে Internal Playbook হিসেবে থাকবে। প্রতিবার আলাদা আলাদা Skill নির্বাচন করতে হবে না।

## ব্যবহার

Claude Code:
```text
/ai-model-engineering-studio
```

OpenCode:
```text
@ai-model-engineering-studio
```

প্রথমে Project-এর বর্তমান ফাইল, নির্দেশনা, Dependencies ও Tools পরীক্ষা করতে হবে। প্রয়োজনীয় Reference Module নিজে নির্বাচন করে Master Skill সম্পূর্ণ Workflow চালাবে।

## গুরুত্বপূর্ণ

এই Repository AI Model বা API দেয় না। বাইরের Provider, API Key, Tool, Permission, Dependency ও Hardware প্রয়োজন হলে সেগুলো আলাদাভাবে Configure করতে হবে। কাজ সত্যিই Build/Test/Generate না হলে Agent সেটি সম্পন্ন হয়েছে বলে দাবি করতে পারবে না।

বিস্তারিত ইংরেজি নির্দেশনা: [README.md](README.md)।
