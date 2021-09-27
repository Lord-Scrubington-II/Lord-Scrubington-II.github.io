# Zane Wang's User Page
Hello and welcome. This is Zane Wang (Lord-Scrubington-II)'s Github page. Though it is quite bare-bones at the moment, I fully intend to improve it with time.

## About Me

I attend [The University of California San Diego](https://www.ucsd.edu/). 

My interests include:
1. Game Development
2. Dungeons & Dragons
3. Classical music  
Here's a link to my [favourite part of my favourite composition](https://youtu.be/XiTIfH0TpTg?t=240).  

Some of my game projects include:
- A chess game
  - Includes AI
- A rails shooter
  - Does not include AI
- A tower defence game
  - Sort of includes AI
- An RPG
  - I'll get back to you on that one

**My favourite programming language is C#.** (`delegates` and `Coroutines` are cool!)  
Here's some code that I wrote for an RPG.
```csharp
/**
 * default behaviour for standard attack.
 * belongs to the GenericActor class
 */
public virtual int StandardAttack(GenericActor target)
{
    int atk;
    int def;
    int damage;
    float resistanceFactor;

    //assuming a physical standard attack is the default
    atk = this.GetTrueAttack();
    def = target.GetTrueDefense();
    try
    {
        resistanceFactor = target.WeakResist[GenericSkill.DamageTypes.Physical];
    }
    catch (KeyNotFoundException)
    {
        //not resistant, use multiplier 1x
        resistanceFactor = 1;
    }
    damage = (int)(resistanceFactor * BattleElements.CombatManager.CalculateDamage(atk, def));

    target.CurrentHP -= damage;
    return damage;
}
```
### TODO & FIXME
- [x] Eat
- [ ] **Get Exercise**
- [ ] ***Sleep at a reasonable hour***
- [ ] ~~Achieve enlightenment~~ Settle for a university degree
- [ ] Finish some games in my backlog
 
Here's a link to this repo's [README](./README.md).

## Random Stuff
Confucius once said:
> When a wise man points at the moon, the imbecile scrutinizes his finger.
> 

Here's a picture of a snow weasel, just because I can:
![snow_weasel](https://raw.githubusercontent.com/Lord-Scrubington-II/Lord-Scrubington-II.github.io/main/snow_weasel.png)