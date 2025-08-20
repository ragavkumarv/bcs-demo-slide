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

addons:
  - fancy-arrow
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


---

<h1 class="!text-orange-400" >Ternary Operator</h1>




###  <logos-javascript /> Javascript

<div data-id="js-box">

```js {all}{class:'!children:text-[1.2rem] !children:leading-6'}
condition ? valueIfTrue : valueIfFalse
```

</div>


<div class="mt-[2rem]" data-id="py-box">

### <logos-python /> Python 

```py {all}{class:'!children:text-[1.2rem] !children:leading-6'}
value_if_true if condition else value_if_false
```

</div>


<div class="mt-[1.5rem]">

<h2 class="!text-red-500">Example</h2>


```py {all}{class:'!children:text-[1.2rem] !children:leading-6'}
age = 18
status = "Adult" if age >= 18 else "Minor"
print(status)
```

</div>

<p v-drag="[779,361,25,40]" text-green text-2xl data-id="one">Hi</p>


<p v-drag="[816,162,59,40]" text-orange text-2xl  data-id="two">Hello</p>


<FancyArrow color="orange" from="[data-id=js-box@(50%,150%)]" to="[data-id=py-box@top]" arc="0.4" />


<FancyArrow color="orange" from="[data-id=one@bottom]" to="[data-id=two@left]" arc="-0.1" />


---


<FancyArrow color="orange" from="[data-id=one@bottom]" to="[data-id=two@left]" arc="-0.1" />

<p v-drag="[247,212,25,40]" text-green text-2xl data-id="one">Hi</p>


<p v-drag="[721,120,59,40]" text-orange text-2xl  data-id="two">Hello</p>

