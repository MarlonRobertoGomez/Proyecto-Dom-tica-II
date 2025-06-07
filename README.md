 public class MainActivity extends AppCompatActivity implements 
View.OnClickListener, View.OnLongClickListener

rivate void botones_accion() 
{ 
    foco_pp.setOnClickListener(this); 
    foco_sp.setOnClickListener(this); 
    foco_tp.setOnClickListener(this); 
    foco_ext.setOnClickListener(this); 
    enchufe_pp.setOnClickListener(this); 
    enchufe_sp.setOnClickListener(this); 
    enchufe_tp.setOnClickListener(this); 
    enchufe_ext.setOnClickListener(this); 
    boton_focos.setOnClickListener(this); 
    boton_enchufes.setOnClickListener(this); 
     
    //click largo 
    foco_pp.setOnLongClickListener(this); 
    foco_sp.setOnLongClickListener(this); 
    foco_tp.setOnLongClickListener(this); 
    foco_ext.setOnLongClickListener(this); 
} 

/Metodo para detectar los botones con click largo 
@Override 
public boolean onLongClick(View v) 
{ 
    if (v == foco_pp) 
    { 
        popup(foco_pp); 
        return true; 
    } 
 
    if (v == foco_sp) 
    { 
        popup(foco_sp); 
        return true; 
    } 
 
    if (v == foco_tp) 
    { 
        popup(foco_tp); 
        return true; 
    } 
 
    if (v == foco_ext) 
    { 
        popup(foco_ext); 
        return true; 
    } 

     return false; 
}
