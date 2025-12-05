# tabs-ref-telco

<br />
<br />

## 1. Historicos

<br />

- Throughput por site

```sql
select *
from tcpsai.ref_thr_fileaccess
;

select *
from tcpsai.ref_thr_streaming
;

select *
from tcpsai.ref_thr_browsing
;
```

<br />
<br />

- Cantidad de usuarios por site

<br />

```sql
select *
from tcpsai.ref_users_11
;
```

<br />
<br />
<br />

- Información de sites únicos

<br />

```sql
select *
from tcpsai.sites_unique
;
```


<br />
<br />
<br />

- Valores umbrales de los KPIs

<br />

```sql
select *
from tcpsai.ref_synack_delay
from tcpsai.ref_tcp_success_rate
;

select *
from tcpsai.ref_down_volume_mb
from tcpsai.ref_up_volume_mb
;

select *
from tcpsai.ref_tcp_up_retx
from tcpsai.ref_tcp_down_retx
from tcpsai.ref_tcp_up_ooo
from tcpsai.ref_tcp_down_ooo
;

select *
from tcpsai.ref_srv_up_loss
from tcpsai.ref_srv_down_loss
from tcpsai.ref_cl_up_loss
from tcpsai.ref_cl_down_loss
;

select
from tcpsai.ref_srv_rtt_ms
from tcpsai.ref_cl_rtt_ms
from tcpsai.ref_srv_rtt_long
from tcpsai.ref_cl_rtt_long
;

```


<br />
<br />

- 5 vecinos más cercanos

<br />

```sql
select *
from tcpsai.sites_unique_vecinos
;
```


<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />


## 2. Alertas

<br />
<br />

- Vistas de alertas por sites



```sql
# Vista consolidada

select *
from tcpsai.alarm_activas_4g_consolidado
;
```

<br />

```sql
# Vistas separadas por tabla (juntas forman la vista: alarm_activas_4g_consolidado)

select *
from tcpsai.alarm_activas_caida_mbts_ana_last
;

select *
from tcpsai.alarm_activas_caida_celda_4g_ana_last
;

select *
from tcpsai.alarm_activas_caida_sitio_4g_ana_last
;
```




<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />


## 3. Data cada 15 min

<br />
<br />

- Tabla número de usuarios - 15 min

```sql
select *
from tcpsai.tcpcell_kpi_summary_15min_users_11
;
```

<br />
<br />

- Tabla KPIs 15 min

```sql
select *
from tcpsai_kpi_summary_15min_11
;
```


<br />
<br />

- Tabla Throughput 15 min

```sql
select *
from tcpsai_thr_summary_10min_11
;
```

<br />
<br />

- Tabla indice de moran 15 min (var: rtt)

```sql
select *
from tcpsai.sites_15min_localmoran
;
```





<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />


## 4. Tabla resumen de anomalias

<br />
<br />

- Resumen anomalias

<br />


```sql
select *
from tcpsai.data_eval_13
;
```





<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />

