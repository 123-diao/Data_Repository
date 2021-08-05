我将我的所有数据都放在此仓库中，并会一一分好类（即建立好相应的文件夹，并在此有说明）
```
if(F){
  
  t_l=transcriptLengths(txdb)
  head(t_l)
  t_l=na.omit(t_l)
  head(t_l)
  t_l=t_l[order(t_l$gene_id,t_l$tx_len,decreasing = T),]
  head(t_l)
  str(t_l)
  t_l=t_l[!duplicated(t_l$gene_id),]
  head(t_l)
  g_l=t_l[,c(3,5)]
  
}
```
