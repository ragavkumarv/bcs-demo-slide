---
# You can also start simply with 'default'
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://cover.sli.dev
# some information about your slides (markdown enabled)
title: Welcome to Slidev
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# open graph
seoMeta:
  # By default, Slidev will use ./og-image.png if it exists,
  # or generate one from the first slide if not found.
  ogImage: auto
  # ogImage: https://cover.sli.dev
---

# Python

---

# Safe Access


````md magic-move {lines:true, class:'!children:text-[1.1rem] !children:leading-6'}

```py {13}
# Dictionary with Solo Leveling character info
sung_jinwoo = {
    "name": "Sung Jinwoo",
    "title": "Shadow Monarch",
    "level": 110,
    "skills": {
        "stealth": True,
        "shadow_extraction": True,
    }
}

# ✅ Safe access with .get()
print(sung_jinwoo.get("name"))   #?        
```



```py {13}
# Dictionary with Solo Leveling character info
sung_jinwoo = {
    "name": "Sung Jinwoo",
    "title": "Shadow Monarch",
    "level": 110,
    "skills": {
        "stealth": True,
        "shadow_extraction": True,
    }
}

# ✅ Safe access with .get()
print(sung_jinwoo.get("name"))   # "Sung Jinwoo"       
```


```py
# Dictionary with Solo Leveling character info
sung_jinwoo = {
    "name": "Sung Jinwoo",
    "title": "Shadow Monarch",
    "level": 110,
    "skills": {
        "stealth": True,
        "shadow_extraction": True,
    }
}

# ✅ Safe access with .get()
print(sung_jinwoo.get("title"))  #?
```

```py
# Dictionary with Solo Leveling character info
sung_jinwoo = {
    "name": "Sung Jinwoo",
    "title": "Shadow Monarch",
    "level": 110,
    "skills": {
        "stealth": True,
        "shadow_extraction": True,
    }
}

# ✅ Safe access with .get()
print(sung_jinwoo.get("title"))  # Shadow Monarch
```





```py
# Dictionary with Solo Leveling character info
sung_jinwoo = {
    "name": "Sung Jinwoo",
    "title": "Shadow Monarch",
    "level": 110,
    "skills": {
        "stealth": True,
        "shadow_extraction": True,
    }
}

# ✅ Safe access with .get() 
print(sung_jinwoo.get("guild"))  #?
```



```py
# Dictionary with Solo Leveling character info
sung_jinwoo = {
    "name": "Sung Jinwoo",
    "title": "Shadow Monarch",
    "level": 110,
    "skills": {
        "stealth": True,
        "shadow_extraction": True,
    }
}

# ✅ Safe access with .get() 
print(sung_jinwoo.get("guild"))  # None (missing key)
```

````

## Output


<div v-click="[1,2]" v-if="$clicks < 2">

```py {all}{class:'!children:text-[1.1rem] !children:leading-6'}
"Sung Jinwoo"
```

</div>


<div v-click="[3,4]" v-if="$clicks < 4">

```py {all}{class:'!children:text-[1.1rem] !children:leading-6'}
"Shadow Monarch"
```

</div>



<div v-click="[5,6]" v-if="$clicks < 6">

```py {all}{class:'!children:text-[1.1rem] !children:leading-6'}
None
```

</div>



---


# Safe Access


<div flex="~ gap-[2rem] justify-center items-center">

<div>

````md magic-move {lines:true, class:'!children:text-[1.1rem] !children:leading-6'}

```py 
# Dictionary with Solo Leveling character info
sung_jinwoo = {
    "name": "Sung Jinwoo",
    "title": "Shadow Monarch",
    "level": 110,
    "skills": {
        "stealth": True,
        "shadow_extraction": True,
    }
}

# ✅ Safe access with .get()
print(sung_jinwoo.get("name"))   #?        
```



```py 
# Dictionary with Solo Leveling character info
sung_jinwoo = {
    "name": "Sung Jinwoo",
    "title": "Shadow Monarch",
    "level": 110,
    "skills": {
        "stealth": True,
        "shadow_extraction": True,
    }
}

# ✅ Safe access with .get()
print(sung_jinwoo.get("name"))   # "Sung Jinwoo"       
```


```py
# Dictionary with Solo Leveling character info
sung_jinwoo = {
    "name": "Sung Jinwoo",
    "title": "Shadow Monarch",
    "level": 110,
    "skills": {
        "stealth": True,
        "shadow_extraction": True,
    }
}

# ✅ Safe access with .get()
print(sung_jinwoo.get("title"))  #?
```

```py
# Dictionary with Solo Leveling character info
sung_jinwoo = {
    "name": "Sung Jinwoo",
    "title": "Shadow Monarch",
    "level": 110,
    "skills": {
        "stealth": True,
        "shadow_extraction": True,
    }
}

# ✅ Safe access with .get()
print(sung_jinwoo.get("title"))  # Shadow Monarch
```





```py
# Dictionary with Solo Leveling character info
sung_jinwoo = {
    "name": "Sung Jinwoo",
    "title": "Shadow Monarch",
    "level": 110,
    "skills": {
        "stealth": True,
        "shadow_extraction": True,
    }
}

# ✅ Safe access with .get() 
print(sung_jinwoo.get("guild"))  #?
```



```py
# Dictionary with Solo Leveling character info
sung_jinwoo = {
    "name": "Sung Jinwoo",
    "title": "Shadow Monarch",
    "level": 110,
    "skills": {
        "stealth": True,
        "shadow_extraction": True,
    }
}

# ✅ Safe access with .get() 
print(sung_jinwoo.get("guild"))  # None (missing key)
```

````

</div>

<div>

## Output


<div v-click="[1,2]" v-if="$clicks < 2">

```py {all}{class:'!children:text-[1.1rem] !children:leading-6'}
"Sung Jinwoo"
```

</div>


<div v-click="[3,4]" v-if="$clicks < 4">

```py {all}{class:'!children:text-[1.1rem] !children:leading-6'}
"Shadow Monarch"
```

</div>



<div v-click="[5,6]" v-if="$clicks < 6">

```py {all}{class:'!children:text-[1.1rem] !children:leading-6'}
None
```

</div>

</div>

</div>