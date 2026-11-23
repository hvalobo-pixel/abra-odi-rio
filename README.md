# abra-odi-rio
<!doctype html>
<html lang="pt-BR"><head><meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Meu Abraço Diário · cartão de cuidado</title>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,500;0,600;1,400&family=Nunito:wght@400;600;700&display=swap">
<style>
:root{--bg:#f4ede4;--card:#fffaf3;--fg:#3b2a20;--mut:#7a6455;--soft:#a8917f;--terra:#b8623f;--sage:#7a8a5a;--tint:#f0e5d6;--bd:rgba(120,80,50,.14);--m1:#b5523b;--m2:#cf8a52;--m3:#d4a24c;--m4:#8f9f62;--m5:#5f7f4a;--ft:'Lora',Georgia,serif;--fb:'Nunito',system-ui,sans-serif;color-scheme:light;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media(prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#1f1612;--card:#2a1f19;--fg:#f1e6d8;--mut:#bfa592;--soft:#8d7767;--terra:#e0865f;--sage:#a2b27c;--tint:#35271f;--bd:rgba(240,200,170,.14);color-scheme:dark}}
:root[data-theme="dark"]{--bg:#1f1612;--card:#2a1f19;--fg:#f1e6d8;--mut:#bfa592;--soft:#8d7767;--terra:#e0865f;--sage:#a2b27c;--tint:#35271f;--bd:rgba(240,200,170,.14);color-scheme:dark}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--fg);font:16px/1.6 var(--fb);padding:0 max(16px,env(safe-area-inset-left,0px))}
.pg{max-width:600px;margin:0 auto;padding:24px 0 40px}
.hd{text-align:center;margin-bottom:14px}
.hd svg{color:var(--terra)}
h1{font:600 1.8rem var(--ft);color:var(--terra);margin:2px 0}
.sub{font-size:.8rem;color:var(--mut);margin:0 0 10px}
.nav{display:flex;align-items:center;justify-content:center;gap:8px;margin-bottom:8px}
.nav button,.nav input{background:var(--card);border:1px solid var(--bd);color:var(--mut);border-radius:10px;padding:6px 12px;font:inherit;font-size:.85rem;cursor:pointer}
.nav button:disabled{opacity:.3}
#dl{font-weight:700;color:var(--fg);text-transform:capitalize;min-width:150px}
.pt{height:5px;width:160px;background:var(--tint);border-radius:9px;margin:0 auto;overflow:hidden}
.pt i{display:block;height:100%;width:0;background:var(--sage);transition:width .4s}
#st{font-size:.72rem;color:var(--soft);height:16px;margin-top:4px}
.sec,.tabs{display:flex;gap:4px;border-radius:14px;padding:4px;margin-bottom:14px}
.sec{background:var(--terra)}
.tabs{background:var(--card);border:1px solid var(--bd)}
.sec button,.tabs button{flex:1;border:0;background:none;border-radius:10px;padding:9px 0;font:700 .86rem var(--fb);cursor:pointer}
.sec button{color:rgba(255,255,255,.7)}.sec button.on{background:rgba(255,255,255,.22);color:#fff}
.tabs button{color:var(--mut)}.tabs button.on{background:var(--sage);color:#fff}
.card{background:var(--card);border:1px solid var(--bd);border-radius:18px;padding:18px;margin-bottom:12px}
.eye{font-size:.68rem;font-weight:700;letter-spacing:.12em;text-transform:uppercase;color:var(--sage);margin:0}
h2{font:600 1.08rem var(--ft);margin:2px 0 12px}
.lb{font-size:.68rem;font-weight:700;letter-spacing:.08em;text-transform:uppercase;color:var(--soft);margin:12px 0 6px}
.hint{font:italic .85rem var(--ft);color:var(--mut);margin:0 0 10px}
.row{display:flex;gap:6px}
.sc{flex:1;border:2px solid var(--bd);background:var(--tint);border-radius:12px;padding:8px 2px;text-align:center;cursor:pointer;font:600 .62rem var(--fb);color:var(--mut)}
.sc b{display:block;font-size:1rem;color:var(--c)}
.sc.on{background:var(--c);border-color:var(--c);color:#fff}.sc.on b{color:#fff}
.ch{display:flex;flex-wrap:wrap;gap:6px}
.c{border:1.5px solid var(--bd);background:var(--tint);color:var(--mut);border-radius:99px;padding:6px 12px;font:600 .8rem var(--fb);cursor:pointer}
.c.on{background:var(--terra);border-color:var(--terra);color:#fff}
.c.g.on{background:var(--sage);border-color:var(--sage)}
textarea,input[type=text]{width:100%;background:var(--tint);border:1.5px solid var(--bd);border-radius:12px;padding:10px 12px;color:var(--fg);font:inherit;font-size:.95rem;resize:vertical;margin-bottom:6px}
textarea{min-height:64px}
input[type=range]{width:100%;accent-color:var(--sage)}
.ln{background:none;border:0;color:var(--terra);font:600 .8rem var(--fb);cursor:pointer;padding:6px 0;text-decoration:underline}
.msg{font:italic .9rem var(--ft);color:var(--terra);margin:10px 0 0}
.cal{display:grid;grid-template-columns:repeat(7,1fr);gap:4px;text-align:center}
.cal span{font-size:.65rem;color:var(--soft);font-weight:700}
.cal button{aspect-ratio:1;border:1.5px solid var(--bd);background:var(--tint);border-radius:10px;color:var(--fg);font:600 .8rem var(--fb);cursor:pointer}
.cal button.dot{background:var(--c);color:#fff;border-color:var(--c)}
.cal button.td{outline:2px solid var(--terra)}
.he{border:1px solid var(--bd);border-radius:14px;margin-bottom:8px;background:var(--card);overflow:hidden}
.hh{display:flex;align-items:center;gap:10px;padding:12px 14px;cursor:pointer;font-weight:700;font-size:.9rem}
.hh i{width:12px;height:12px;border-radius:50%;background:var(--c,var(--bd));margin-left:auto}
.hb{display:none;padding:0 14px 12px;font-size:.88rem;color:var(--mut)}.he.open .hb{display:block}
.hb p{margin:4px 0}.hb b{color:var(--fg)}
.fn{font-size:.75rem;color:var(--soft);text-align:center;margin-top:16px;line-height:1.5}
.th{background:none;border:0;color:var(--soft);font:inherit;font-size:.75rem;cursor:pointer;display:block;margin:10px auto 0}
</style></head><body><div class="pg">
<div class="hd">
<svg width="40" height="40" viewBox="0 0 40 40" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" aria-hidden="true"><path d="M20 35V17"/><path d="M20 20c-7 0-10-5-10-10 7 0 10 4 10 10Z"/><path d="M20 24c6 0 9-4 9-8-6 0-9 3-9 8Z"/></svg>
<h1>Meu Abraço Diário</h1>
<p class="sub">um cantinho seu, no seu ritmo</p>
<div class="nav"><button id="pv" aria-label="Dia anterior">‹</button><span id="dl"></span><button id="nx" aria-label="Próximo dia">›</button><input type="date" id="dp" aria-label="Escolher data"></div>
<div id="st"></div></div>
<div class="sec"><button id="s-rot" class="on">🌿 Rotina do Dia</button><button id="s-reg">📋 Registro de Saúde</button></div>
<div class="tabs"><button id="t-hoje" class="on">Hoje</button><button id="t-cal">Calendário</button><button id="t-hist">Histórico</button><button id="t-crise">🤍 Apoio</button></div>
<main id="app"></main>
<p class="fn">🔒 Suas anotações ficam somente neste aparelho. Ninguém as acompanha, nem sua psicóloga, e você decide o que levar para a sessão.<br><b>Este painel não é monitorado.</b> Se estiver muito difícil, não espere a sessão: use a aba 🤍 Apoio, fale com sua psicóloga ou ligue 188 (CVV, 24h).</p>
<button class="th" id="th">🌙 Tema</button>
</div>
<script>
(function(){
var $=function(q){return document.querySelector(q)};
var MOOD=["Muito difícil","Difícil","Neutro","Bem","Muito bem"],EN=["Exausta","Baixa","Ok","Alta","Agitada"];
var SIGNS={"Emoções":["irritada","ansiosa","triste","vazio","choro fácil","culpa","calma","conectada","eufórica","medo de abandono","pânico","dissociada"],"Corpo":["cólica","inchaço","dor de cabeça","fadiga","tontura","náusea","dor no corpo","seios sensíveis"],"Foco":["sem foco","névoa mental","procrastinação","inquietação","impulsividade"]};
var CARE=["atividade física","banho de sol","meditação","leitura","comi e hidratei bem","usei uma habilidade","pedi ajuda"];
var MORN=["bebi água","tomei café da manhã","alonguei","respirei fundo","saí para a luz do dia"];
var ARR=["calma","cansada","ansiosa","animada","sobrecarregada","triste"];
var URG=["vontade de me machucar","pensamentos de morte","vontade de sumir","compulsão alimentar","gastar sem pensar","beber ou usar substâncias","explodir com alguém","mandar mensagem impulsiva"];
var ACT=["me machuquei","comi em compulsão","gastei sem planejar","bebi ou usei substâncias","explodi com alguém","me isolei","nenhuma dessas"];
var SK=["respiração ou relaxamento","atenção plena","distração agradável","acalmar pelos sentidos","verificar os fatos","ação oposta","validei meu sentimento","pedi ajuda"];
var CYC=["menstruada","pós-menstrual","ovulação","lútea/TPM","n/a"],SQ=["reparador","picotado","insônia","dormiu demais"];
function ymd(d){var m=d.getMonth()+1,x=d.getDate();return d.getFullYear()+"-"+(m<10?"0":"")+m+"-"+(x<10?"0":"")+x}
function pd(k){var a=k.split("-");return new Date(+a[0],+a[1]-1,+a[2])}
var TODAY=ymd(new Date()),date=TODAY,sec="rot",tab="hoje",cm=new Date(),s={},edit=false,tm=null;
function esc(t){return String(t==null?"":t).replace(/[&<>"]/g,function(c){return {"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;"}[c]})}
function load(d){try{return JSON.parse(localStorage.getItem("mad:"+d))||{}}catch(e){return {}}}
function meds(){try{return JSON.parse(localStorage.getItem("mad-meds"))||[]}catch(e){return []}}
function setMeds(a){try{localStorage.setItem("mad-meds",JSON.stringify(a))}catch(e){}}
function save(){try{localStorage.setItem("mad:"+date,JSON.stringify(s));$("#st").textContent="salvo ✓"}catch(e){$("#st").textContent="não foi possível salvar neste navegador"}prog()}
function dsave(){$("#st").textContent="salvando…";clearTimeout(tm);tm=setTimeout(save,500)}
function arr(f){return Array.isArray(s[f])?s[f]:[]}
function prog(){}
function card(e,t,b){return '<div class="card"><p class="eye">'+e+'</p><h2>'+t+'</h2>'+b+'</div>'}
function scale(f,L){var h='<div class="row">';L.forEach(function(l,i){var v=i+1,on=+s[f]===v;h+='<div class="sc'+(on?" on":"")+'" role="button" tabindex="0" data-t="s" data-f="'+f+'" data-v="'+v+'" style="--c:var(--m'+v+')"><b>'+v+'</b>'+l+'</div>'});return h+'</div>'}
function chips(f,L,single,cls){var h='<div class="ch">';L.forEach(function(l){var on=single?s[f]===l:arr(f).indexOf(l)>-1;h+='<span class="c '+(cls||"")+(on?" on":"")+'" role="button" tabindex="0" data-t="'+(single?"o":"m")+'" data-f="'+f+'" data-v="'+esc(l)+'">'+esc(l)+'</span>'});return h+'</div>'}
function ta(f,ph,tag){return (tag==="in"?'<input type="text"':'<textarea')+' data-i="'+f+'" placeholder="'+ph+'"'+(tag==="in"?' value="'+esc(s[f])+'">':'>'+esc(s[f])+'</textarea>')}
function hoje(){var h="";
if(sec==="rot"){
h+=card("Chegada","Como estou chegando hoje?",chips("arr",ARR,true));
h+=card("Intenção","Âncora do dia",'<p class="hint">Uma frase para me lembrar de mim.</p>'+ta("anchor","Hoje eu quero…"));
h+=card("Gratidão","Hoje sou grata por…",ta("grat","Uma ou duas coisas, pequenas servem."));
h+=card("Manhã","Autocuidado do dia",chips("morn",MORN,false,"g"));
h+=card("Pensamentos","Um pensamento que passou por aqui",'<p class="hint">Opcional. Só se estiver com calma e com vontade; pode pular sem culpa.</p><div class="lb">O que aconteceu?</div>'+ta("sit","A situação…","in")+'<div class="lb">O que pensei? E o que senti?</div>'+ta("pen","O pensamento e a emoção…")+'<div class="lb">Que outro olhar também é possível?</div>'+ta("alt","Uma forma mais gentil e realista de ver…"));
h+=card("Conquista","Uma coisa que fiz bem hoje",ta("win","Pode ser pequena."));
h+=card("Noite","Reflexão antes de dormir",ta("night","Como foi o dia? O que posso soltar agora?"));
}else{
h+=card("Bem-estar","Humor geral",scale("mood",MOOD)+'<p class="msg" id="mm">'+(s.mood&&s.mood<=2?"Dia difícil também conta 🤍":"")+'</p>');
h+=card("Vitalidade","Energia",scale("energy",EN));
h+=card("Emoções","Que intensidade cada emoção teve hoje?",'<p class="hint">0 é nenhuma, 5 é a mais forte.</p>'+emo());
h+=card("Impulsos","Vontades que apareceram hoje",chips("urges",URG)+'<p class="msg">'+(urg()?"Obrigada por registrar isso. Você merece apoio agora: abra a aba 🤍 Apoio ou ligue 188 (CVV, 24h).":"")+'</p><div class="lb">O que aconteceu hoje?</div>'+chips("acts",ACT));
h+=card("Habilidades","O que usei para me cuidar?",chips("skills",SK,false,"g")+'<div class="lb">Ajudou?</div>'+chips("helped",["ajudou muito","ajudou um pouco","não ajudou"],true,"g"));
h+=card("Descanso","Sono da noite passada",'<div class="row" style="align-items:center"><input type="range" min="0" max="12" step="0.5" data-sl value="'+(s.sleepH==null?7:s.sleepH)+'"><b id="sv" style="min-width:48px;text-align:right;color:var(--sage)">'+(s.sleepH==null?"—":s.sleepH+"h")+'</b></div><div class="lb">Como foi o sono?</div>'+chips("sleepQ",SQ,true,"g"));
h+=card("Ciclo","Fase do ciclo menstrual",chips("cycle",CYC,true));
var sg="";Object.keys(SIGNS).forEach(function(g){sg+='<div class="lb">'+g+'</div>'+chips("signs",SIGNS[g])});
h+=card("Observação","Sinais do dia",sg);
var m=meds(),mh='';
if(!m.length)mh+='<p class="hint">Cadastre seus remédios abaixo para marcar o que tomou a cada dia.</p>';
else{mh+='<div class="ch">';m.forEach(function(x){var on=arr("meds").indexOf(x)>-1;mh+='<span class="c g'+(on?" on":"")+'" role="button" tabindex="0" data-t="m" data-f="meds" data-v="'+esc(x)+'">'+esc(x)+(edit?' <u data-a="del" data-v="'+esc(x)+'">✕</u>':'')+'</span>'});mh+='</div>'}
mh+='<div class="lb">Adicionar remédio (nome e horário)</div><input type="text" id="nm" placeholder="Ex.: Sertralina 50mg · manhã"><button class="ln" data-a="add">+ adicionar</button> <button class="ln" data-a="edit">'+(edit?"concluir edição":"editar lista")+'</button>';
h+=card("Tratamento","Remédios de hoje",mh);
h+=card("Autocuidado","Cuidados de hoje",chips("care",CARE,false,"g"));
h+=card("Reflexão","Uma linha sobre o dia",ta("line","Em uma frase…","in"));
}return h}
function cal(){var y=cm.getFullYear(),mo=cm.getMonth(),f=new Date(y,mo,1).getDay(),n=new Date(y,mo+1,0).getDate();
var h='<div class="card"><div class="nav"><button data-a="cp">‹</button><span id="dl">'+cm.toLocaleDateString("pt-BR",{month:"long",year:"numeric"})+'</span><button data-a="cn">›</button></div><div class="cal">';
"DSTQQSS".split("").forEach(function(d){h+="<span>"+d+"</span>"});
for(var i=0;i<f;i++)h+="<i></i>";
for(var d=1;d<=n;d++){var k=ymd(new Date(y,mo,d)),e=load(k);h+='<button data-a="day" data-v="'+k+'" class="'+(e.mood?"dot":"")+(k===TODAY?" td":"")+'"'+(e.mood?' style="--c:var(--m'+e.mood+')"':"")+'>'+d+'</button>'}
return h+'</div><p class="hint" style="margin-top:12px">A cor de cada dia mostra o humor registrado.</p></div>'}
function sumr(e){var r=[];function a(l,t){if(t&&t.length)r.push([l,Array.isArray(t)?t.join(", "):t])}
if(e.mood)a("Humor",e.mood+"/5 · "+MOOD[e.mood-1]);if(e.energy)a("Energia",EN[e.energy-1]);
if(e.sleepH!=null||e.sleepQ)a("Sono",(e.sleepH!=null?e.sleepH+"h":"")+(e.sleepQ?" · "+e.sleepQ:""));
if(e.emo&&Object.keys(e.emo).length)a("Emoções",Object.keys(e.emo).map(function(n){return n+" "+e.emo[n]+"/5"}).join(", "));a("Impulsos",e.urges);a("Aconteceu",e.acts);a("Habilidades",e.skills);a("Ajudou",e.helped);a("Ciclo",e.cycle);a("Sinais",e.signs);a("Remédios",e.meds);a("Cuidados",e.care);a("Chegada",e.arr);a("Manhã",e.morn);a("Âncora",e.anchor);a("Gratidão",e.grat);
a("Situação",e.sit);a("Pensamento e emoção",e.pen);a("Outro olhar",e.alt);a("Conquista",e.win);a("Noite",e.night);a("Uma linha",e.line);return r}
function keys(){var k=[];try{for(var i=0;i<localStorage.length;i++){var x=localStorage.key(i);if(x.indexOf("mad:")===0)k.push(x.slice(4))}}catch(e){}return k.sort().reverse()}
function hist(){var k=keys();if(!k.length)return '<div class="card"><p class="hint">Quando você começar a registrar, seus dias aparecem aqui.</p></div>';
var h='';k.forEach(function(d){var e=load(d),r=sumr(e);h+='<div class="he"><div class="hh" data-a="tg"><span>'+pd(d).toLocaleDateString("pt-BR",{weekday:"short",day:"numeric",month:"short",year:"numeric"})+'</span><i'+(e.mood?' style="--c:var(--m'+e.mood+')"':"")+'></i></div><div class="hb">'+(r.length?r.map(function(x){return '<p><b>'+x[0]+':</b> '+esc(x[1])+'</p>'}).join(""):"<p>Entrada vazia</p>")+'</div></div>'});
return '<div class="card"><p class="eye">Para levar à sessão</p><h2>Resumo dos últimos 7 dias</h2><p class="hint">Copie e cole numa mensagem se quiser compartilhar com sua psicóloga. Só vai o que você escolher enviar.</p><button class="c on" data-a="copy">Copiar resumo</button></div>'+h}
function emo(){var E=["tristeza","raiva","medo","vergonha","ansiedade","alegria"],h="";s.emo=s.emo||{};E.forEach(function(n){h+='<div class="lb">'+n+'</div><div class="row">';for(var v=0;v<6;v++){h+='<div class="sc'+(s.emo[n]===v?" on":"")+'" role="button" tabindex="0" data-t="e" data-f="'+n+'" data-v="'+v+'" style="--c:var(--terra)"><b>'+v+'</b></div>'}h+='</div>'});return h}
function urg(){return arr("urges").some(function(x){return x==="vontade de me machucar"||x==="pensamentos de morte"||x==="vontade de sumir"})||arr("acts").indexOf("me machuquei")>-1}
function cr(){try{return JSON.parse(localStorage.getItem("mad-crisis"))||{}}catch(e){return {}}}
function crise(){var c=cr();function f(k,l,ph){return '<div class="lb">'+l+'</div><textarea data-c="'+k+'" placeholder="'+ph+'">'+esc(c[k])+'</textarea>'}
return '<div class="card" style="border-color:var(--terra)"><p class="eye">Agora</p><h2>Se estiver muito difícil</h2><p>Você não precisa passar por isso sozinha.</p><p>📞 <b>188</b>, CVV (24h, gratuito)<br>📞 <b>192</b>, SAMU<br>🏥 Procure a UPA ou o pronto-socorro mais próximo.</p></div>'+card("Meu cartão","Combinado com minha psicóloga",'<p class="hint">Preencha com calma, de preferência junto com ela. Fica salvo só neste aparelho.</p>'+f("sinais","Sinais de que estou entrando em crise","Ex.: não consigo dormir, sinto muito vazio…")+f("fazer","O que posso fazer primeiro","Minhas habilidades, um lugar seguro, uma música…")+f("pessoas","Pessoas que posso chamar","Nome e telefone")+f("psi","Minha psicóloga","Nome e contato combinado")+f("seguro","Deixar o ambiente mais seguro","O que posso afastar de mim e quem pode me ajudar"))}
function copy(){var k=keys().slice(0,7).reverse(),t="Meu Abraço Diário · resumo\n";k.forEach(function(d){t+="\n"+pd(d).toLocaleDateString("pt-BR")+"\n";sumr(load(d)).forEach(function(x){t+="- "+x[0]+": "+x[1]+"\n"})});
try{navigator.clipboard.writeText(t).then(function(){$("#st").textContent="resumo copiado ✓"},function(){$("#st").textContent="não consegui copiar"})}catch(e){$("#st").textContent="não consegui copiar"}}
function render(){var d=pd(date);$("#dl").textContent=d.toLocaleDateString("pt-BR",{weekday:"long",day:"numeric",month:"long"});$("#nx").disabled=date>=TODAY;$("#dp").value=date;$("#dp").max=TODAY;
$("#app").innerHTML=tab==="hoje"?hoje():tab==="cal"?cal():tab==="crise"?crise():hist();prog()}
function go(d){date=d;s=load(d);render()}
function shift(n){var d=pd(date);d.setDate(d.getDate()+n);var k=ymd(d);if(k<=TODAY)go(k)}
function setSec(x){sec=x;$("#s-rot").className=x==="rot"?"on":"";$("#s-reg").className=x==="reg"?"on":"";tab="hoje";tabs();render()}
function tabs(){["hoje","cal","hist","crise"].forEach(function(t){$("#t-"+t).className=t===tab?"on":""})}
$("#s-rot").onclick=function(){setSec("rot")};$("#s-reg").onclick=function(){setSec("reg")};
["hoje","cal","hist","crise"].forEach(function(t){$("#t-"+t).onclick=function(){tab=t;tabs();render()}});
$("#pv").onclick=function(){shift(-1)};$("#nx").onclick=function(){shift(1)};
$("#dp").onchange=function(){if(this.value&&this.value<=TODAY)go(this.value)};
function act(el){var t=el.dataset.t,f=el.dataset.f,v=el.dataset.v;if(!t)return;
if(t==="s"){s[f]=s[f]===+v?0:+v;if(!s[f])delete s[f];if(f==="mood"){render()}else{render()}}
else if(t==="e"){s.emo=s.emo||{};s.emo[f]=+v;render()}
else if(t==="o"){if(s[f]===v)delete s[f];else s[f]=v;render()}
else{var a=arr(f).slice(),i=a.indexOf(v);if(i>-1)a.splice(i,1);else a.push(v);s[f]=a;if(f==="urges"||f==="acts")render();else el.classList.toggle("on")}
save()}
$("#app").addEventListener("click",function(ev){var u=ev.target.closest("[data-a]");
if(u){var a=u.dataset.a,v=u.dataset.v;
if(a==="del"){ev.stopPropagation();setMeds(meds().filter(function(x){return x!==v}));render();return}
if(a==="add"){var i=$("#nm"),n=i.value.trim();if(n){var m=meds();if(m.indexOf(n)<0){m.push(n);setMeds(m)}}render();return}
if(a==="edit"){edit=!edit;render();return}
if(a==="cp"){cm.setMonth(cm.getMonth()-1);render();return}
if(a==="cn"){cm.setMonth(cm.getMonth()+1);render();return}
if(a==="day"){go(v);tab="hoje";sec="reg";$("#s-reg").className="on";$("#s-rot").className="";tabs();render();return}
if(a==="tg"){u.parentNode.classList.toggle("open");return}
if(a==="copy"){copy();return}}
var c=ev.target.closest("[data-t]");if(c)act(c)});
$("#app").addEventListener("keydown",function(ev){if((ev.key==="Enter"||ev.key===" ")&&ev.target.dataset&&ev.target.dataset.t){ev.preventDefault();act(ev.target)}});
$("#app").addEventListener("input",function(ev){var t=ev.target;
if(t.dataset.i){s[t.dataset.i]=t.value;dsave()}
else if(t.dataset.c){var c=cr();c[t.dataset.c]=t.value;try{localStorage.setItem("mad-crisis",JSON.stringify(c));$("#st").textContent="salvo ✓"}catch(e){}}
else if("sl" in t.dataset){s.sleepH=+t.value;$("#sv").textContent=t.value+"h";dsave()}});
var root=document.documentElement;
function tl(){var d=root.getAttribute("data-theme")==="dark"||(!root.getAttribute("data-theme")&&matchMedia("(prefers-color-scheme:dark)").matches);$("#th").textContent=d?"☀️ Tema claro":"🌙 Tema escuro";return d}
$("#th").onclick=function(){var n=tl()?"light":"dark";root.setAttribute("data-theme",n);try{localStorage.setItem("mad-theme",n)}catch(e){}tl()};
try{var th=localStorage.getItem("mad-theme");if(th)root.setAttribute("data-theme",th)}catch(e){}
tl();go(TODAY);
})();
</script></body></html>
