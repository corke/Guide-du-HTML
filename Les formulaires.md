#Formulaires

##Disposition des champs :

####Pas de `<br/>` !  

Ex :   
`<label for="comment">Pour laisser un commentaire libre à propos d'O'clock, c'est par ici :</label>`    
`<textarea placeholder="" name="comment" rows="8" cols="40"></textarea>`  
`<br/>`   
`<input type="checkbox" name="certification" value="">`  
`<label for="certification">Je certifie la véracité de ces informations.</label>`  

Devient :  
`<p>`  
    `<label for="comment">Pour laisser un commentaire libre à propos d'O'clock, c'est par ici :</label>`  
`    <textarea placeholder="" name="comment" rows="8" cols="40"></textarea>`  
`</p>`  
`<p>`  
    `<input type="checkbox" name="certification" value="">`  
     `<label for="certification">Je certifie la véracité de ces informations.</label>`  
`</p>`  
Ou :  
`<label>
  <input type="radio" name="civilite" value="2" checked />
  Mme
</label>`

##Les labels 
&lt;label&gt; : Représentent le titre / désignation d'un élément du formulaire
Fonctionnement / mécanisme : Permet lors du clic sur le label de prendre la main sur le champ lié comme si le clic 
avait été fait sur l'élément du formulaire
2 manière d'écrire les labels

`<label>
Titre de mon élément 
<input type="text" name="mon_element" value="un element" id="id_du_champ"/>
</label>`  
Ici la méthode consiste a insérer le titre (le label) et le champ dans la balise <label> le parametre id n'est pas utilisé 

`<label for="id_du_champ2">Titre de mon élément2</label>
<input type="text" name="mon_element2" value="un element2" id="id_du_champ2"/>`  

Ici la méthode sépare le label du champs, on utilise donc for="id" dans le label afin de lier le champs au label, l'id doit être
le même que l'id du champs
