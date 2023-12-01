> _Fork_ deze leertaak en ga aan de slag. Onderstaande outline ga je gedurende deze taak in jouw eigen GitHub omgeving uitwerken. De instructie vind je, zoals altijd, in: [docs/INSTRUCTIONS.md](docs/INSTRUCTIONS.md)

# Titel
<!-- Geef je project een titel en schrijf in één zin wat het is -->

## Inhoudsopgave

  * [Beschrijving](#beschrijving)
  * [Kenmerken](#kenmerken)
  * [Bronnen](#bronnen)
  * [Licentie](#licentie)

## Beschrijving
Hier laat ik zien dat wat ik voor thema heb.
home:

![image](https://github.com/Seijno/the-client-website/assets/104066080/a2dea808-4a2e-451a-b899-838161e95d71)

filter:

![image](https://github.com/Seijno/the-client-website/assets/104066080/e170364c-0eea-48ad-8379-c3051d7b68b7)

site zelf: https://seijno.github.io/the-client-website/#

## Kenmerken
het beste aan de site vind ik de hammburger menu hier de code:
HTML:
```
<nav>
        <section class="filterMenu">
            <div id="sideMenu" class="sideMenu">
                <a class="closebtn material-symbols-outlined" id="closeMenu">close</a>
                <form>
                    <label><h3>Filters:</h3></label>
                    <p>Events(): <span><input type="checkbox" ></span></p>
                    <p>hulp gezocht(): <span><input type="checkbox" ></span></p>
                    <p>hulp aanbieder(): <span><input type="checkbox" ></span></p>
                    <p>muziek(): <span><input type="checkbox" ></span></p>
                    <p>museum(): <span><input type="checkbox" ></span></p>
                </form>
              </div>
              <a href="#"><span class="material-symbols-outlined" id="openMenu">
                filter_list
                </span></a>
          </section>
    </nav>`
```
JS:
```
document.getElementById("openMenu").addEventListener("click", openMenu);
document.getElementById("closeMenu").addEventListener("click", closeMenu);

function openMenu() {
document.getElementById("sideMenu").style.width = "50vw";
}

function closeMenu() {
document.getElementById("sideMenu").style.width = "0";}
```
CSS:
```
.menu-item{
  margin: 0 1em 0 0;
  vertical-align: middle;
  text-decoration: var(--decoratie-uit);
  
}
.menu-item:hover{
  text-decoration: var(--decoratie-line);
}


.navmenu{
  padding-left: 1em;
  display: flex;
  flex-direction: row;
  justify-content: center;
  list-style: var(--decoratie-uit);
}
```



## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).
