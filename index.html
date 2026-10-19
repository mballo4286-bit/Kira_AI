<!doctype html><html lang="fr"><head><meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<meta name="theme-color" content="#0b72e7"><link rel="manifest" href="manifest.json">
<link rel="icon" type="image/png" sizes="192x192" href="icon-192.png"><link rel="apple-touch-icon" sizes="192x192" href="icon-192.png"><meta name="description" content="Kira, assistante IA"><title>Kira</title>
<style>
:root{--bg:#fff;--fg:#1b1f24;--c:#f1f3f6;--me:#d9ecff;--a:#0b72e7}
@media(prefers-color-scheme:dark){:root{--bg:#0e1621;--fg:#e8edf2;--c:#1b2735;--me:#12395f;--a:#4aa3ff}}
*{box-sizing:border-box}body{margin:0;background:var(--bg);color:var(--fg);font:16px system-ui,sans-serif;display:flex;flex-direction:column;height:100dvh}
header{display:flex;align-items:center;justify-content:space-between;padding:10px 14px;color:var(--a);font-weight:700;font-size:22px}
header button{background:none;border:0;font-size:22px}
#log{flex:1;overflow-y:auto;padding:6px 12px}
.m{max-width:92%;margin:8px 0;padding:10px 12px;border-radius:14px;white-space:pre-wrap;word-wrap:break-word;background:var(--c)}
.me{margin-left:auto;background:var(--me)}.m img{max-width:100%;border-radius:10px}
form{display:flex;gap:6px;padding:10px;padding-bottom:max(10px,env(safe-area-inset-bottom))}
#q{flex:1;min-width:0;font-size:16px;padding:12px 14px;border-radius:24px;border:1px solid var(--a);background:var(--bg);color:var(--fg)}
.go{border:0;border-radius:24px;background:var(--a);color:#fff;padding:0 12px;font-size:16px}
#v{position:fixed;inset:0;background:#0e1621;color:#e8edf2;display:none;flex-direction:column;align-items:center;justify-content:space-between;padding:18px;text-align:center;font-size:18px}
#v.on{display:flex}#vt{flex:1;display:flex;flex-direction:column;justify-content:center;gap:14px;max-width:560px;overflow-y:auto}
#orbe{width:150px;height:150px;border-radius:50%;border:0;background:#4aa3ff;color:#fff;font-size:56px}
.ecoute{animation:p 1.2s infinite}.reflechit{background:#8a94a3!important;animation:p 2s infinite}.parle{background:#2ecc71!important;animation:p .8s infinite}
@keyframes p{0%{box-shadow:0 0 0 0 rgba(74,163,255,.55)}100%{box-shadow:0 0 0 42px rgba(74,163,255,0)}}
form{display:block;margin:8px 10px;padding:10px 12px;border:1px solid var(--a);border-radius:22px;background:var(--bg)}
#q{width:100%;border:0;border-radius:0;padding:4px;resize:none;outline:0;background:transparent;max-height:140px}
.cr{display:flex;gap:8px;align-items:center;margin-top:6px}.ic{border:0;border-radius:50%;width:40px;height:40px;background:var(--c);color:var(--fg);font-size:18px}.ic.dk{background:var(--fg);color:var(--bg)}
#dr{position:fixed;top:0;bottom:0;left:0;width:82%;max-width:340px;background:var(--bg);border-right:1px solid var(--c);transform:translateX(-100%);transition:.2s;z-index:5;padding:14px;overflow-y:auto}#dr.on{transform:none}
.dh{display:flex;justify-content:space-between;align-items:center;margin-bottom:10px}.dh button{background:none;border:0;color:inherit;font-size:20px}
.it{padding:12px 6px;border-radius:10px;display:flex;justify-content:space-between}.it.sel{background:var(--c)}.it b{opacity:.5}
#av{position:fixed;inset:0;background:var(--bg);display:none;flex-direction:column;z-index:6;padding:12px}#av.on{display:flex}#ab{flex:1;overflow:auto}#ab iframe{width:100%;height:100%;border:0;background:#fff}
pre{background:var(--c);padding:10px;border-radius:10px;overflow-x:auto;font-size:13px;margin:6px 0;white-space:pre}.bt button{margin:0 6px 6px 0;padding:6px 10px;border-radius:14px;border:1px solid var(--a);background:none;color:var(--a)}
</style></head><body>
<header><button id="bmenu">☰</button><span>Kira</span><span><button id="bspk">🔇</button><button id="bnew">💬</button><button id="bset">⚙️</button></span></header>
<div id="log"></div>
<form id="f"><textarea id="q" rows="1" placeholder="Répondre à Kira…"></textarea><div class="cr"><button type="button" class="ic" id="bfile">＋</button><span style="flex:1"></span><button type="button" class="ic" id="bmic">🎤</button><button type="button" class="ic dk" id="bwave">🎙️</button><button class="ic dk" id="bsend" hidden>➜</button></div></form>
<input id="file" type="file" hidden accept="image/*,.txt,.md,.csv,.json,.py,.js,.html">
<div id="dr"><div class="dh"><b>Kira</b><button id="dx">✕</button></div><div class="it" data-m="c">💬 Conversations</div><div class="it" data-m="p">📁 Projets</div><div class="it" data-m="k">&lt;/&gt; Code</div><div class="it" data-m="a">📦 Artéfacts</div><hr><div id="dl"></div></div>
<div id="av"><div class="dh"><b id="at"></b><span><button id="acp">Copier</button><button id="adl">⬇</button><button id="ax">✕</button></span></div><div id="ab"></div></div>
<div id="v"><a href="#" id="vx" style="color:#4aa3ff">✕ Fermer</a><div id="vt"><div id="toi" style="opacity:.65"></div><div id="kv" style="font-size:20px"></div></div><div id="etat" style="margin:10px 0 16px"></div><button id="orbe">🎙️</button></div>
<script>
const $=id=>document.getElementById(id),CREATEUR='Abddoulaye Mballo',S=localStorage,log=$('log'),q=$('q');
let hist=[],vocal=false,oral=false;
const fmt=s=>s.replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/\*\*(.+?)\*\*/g,'<b>$1</b>');
function add(t,me,html){const d=document.createElement('div');d.className='m'+(me?' me':'');d.innerHTML=html||fmt(t);log.appendChild(d);log.scrollTop=log.scrollHeight;return d}
const modele=()=>S.kira_model||'openai/gpt-oss-120b';
const sys=()=>`Tu es Kira, une assistante amicale et polyvalente créée par ${CREATEUR}. Réponds en français, de façon courte et utile, et tutoie l'utilisateur. Il écrit vite, avec des fautes : comprends son intention sans le reprendre ; si c'est ambigu, choisis le sens le plus probable, reformule brièvement puis réponds. Si on te demande le modèle, dis que tu utilises ${modele()} via Groq. Les questions sur l'argent, l'entrepreneuriat, les études et la carrière sont légitimes : réponds concrètement, sans promettre de gains. Ne refuse que le vraiment dangereux ou illégal. Pour une info qui peut avoir changé et sans source fournie, dis honnêtement que tu n'es pas sûre.`+(oral?' Tu parles à voix haute : 1 à 3 phrases courtes, sans liste ni markdown ni emoji, avec une relance si utile.':'')+ext();
async function groq(messages,model){
 const k=S.kira_key;if(!k)throw new Error('Clé Groq manquante : touche ⚙️.');
 const m=model||modele(),p={model:m,messages,temperature:.4,max_tokens:2000};
 if(m.includes('gpt-oss'))p.reasoning_effort='low';
 const r=await fetch('https://api.groq.com/openai/v1/chat/completions',{method:'POST',headers:{Authorization:'Bearer '+k,'Content-Type':'application/json'},body:JSON.stringify(p)});
 const j=await r.json();if(!r.ok)throw new Error((j.error&&j.error.message)||('Erreur '+r.status));
 return(j.choices[0].message.content||'').replace(/<think>[\s\S]*?<\/think>/g,'').trim()||'(réponse vide)'}
async function prix(){const n={bitcoin:'BTC',ethereum:'ETH',solana:'SOL',binancecoin:'BNB',ripple:'XRP'};
 const d=await(await fetch('https://api.coingecko.com/api/v3/simple/price?ids='+Object.keys(n)+'&vs_currencies=usd&include_24hr_change=true')).json();
 return Object.keys(n).filter(c=>d[c]).map(c=>`${n[c]} : ${d[c].usd} $ (${d[c].usd_24h_change>=0?'+':''}${d[c].usd_24h_change.toFixed(2)}% 24h)`).join('\n')}
async function wiki(t){try{const s=await(await fetch('https://fr.wikipedia.org/w/api.php?action=query&list=search&srsearch='+encodeURIComponent(t)+'&format=json&srlimit=1&origin=*')).json();
 const e=await(await fetch('https://fr.wikipedia.org/w/api.php?action=query&prop=extracts&exintro=1&explaintext=1&titles='+encodeURIComponent(s.query.search[0].title)+'&format=json&origin=*')).json();
 return Object.values(e.query.pages)[0].extract.slice(0,1000)}catch(e){return''}}
async function kira(t){
 const l=t.toLowerCase();
 if(l==='/reset'){hist.length=0;return'Mémoire effacée.'}
 if(l==='/aide')return'Je discute, écris, corrige, traduis, explique, code, lis une image ou un fichier texte (📎), donne le prix des cryptos, fais des photos ("photo de ...") et parle avec toi (🎙️). /reset efface la mémoire.';
 if(/\b(crypto|cryptos|btc|bitcoin|eth|ethereum|solana)\b/.test(l)&&/\b(prix|cours|combien|vaut|valeur|analyse|tendance|avis)\b/.test(l)){
  const d=await prix();if(/analys|tendance|avis/.test(l)){const a=await groq([{role:'system',content:"Tu es analyste crypto. Analyse uniquement ces données, brièvement. Rappelle que ce n'est pas un conseil financier."},{role:'user',content:d+'\n'+t}]);return d+'\n\n'+a}
  return'💰 Prix en direct :\n'+d}
 const ph=l.match(/(?:photo|image)s?\s+(?:de |du |des |d')\s*(.+)/);
 if(ph&&(/^(photo|image)/.test(l)||/envoi|génère|genere|crée|cree|fais|donne|montre/.test(l)))
  {const p=await groq([{role:'system',content:"Tu transformes une demande d'image en prompt ANGLAIS de photographie réaliste : sujet précis, lieu, lumière naturelle, objectif 35mm, f/1.8, haute résolution, détails nets, aucun texte. Réponds uniquement avec le prompt. Si la demande désigne une personne réelle ou précise par son nom (célébrité, footballeur, connaissance), un mineur, ou du contenu sexuel ou nu, réponds exactement REFUS."},{role:'user',content:ph[1]}]);
   if(/^REFUS/i.test(p))return"Je ne peux pas créer la photo d'une personne réelle ou précise (ni de contenu inapproprié) : une image IA serait inventée et ne lui ressemblerait pas. Décris plutôt un paysage, un objet, un animal, un lieu ou un personnage imaginaire (ex. « photo d'une femme africaine souriante au marché »).";
   return{html:'<img alt="photo" src="https://image.pollinations.ai/prompt/'+encodeURIComponent(p+', ultra realistic photo, sharp focus, natural light')+'?model=flux&width=1024&height=1024&nologo=1&seed='+(Date.now()%100000)+'">'}}
 const info=t.split(/\s+/).length>=3?await wiki(t):'';
 const u=info?'INFO WEB (ignore-la si elle ne correspond pas à la question) :\n'+info+'\n\nQuestion : '+t:t;
 const r=await groq([{role:'system',content:sys()},...hist.slice(-12),{role:'user',content:u}]);
 hist.push({role:'user',content:t},{role:'assistant',content:r});sauve();return r}
async function repondre(t,o){oral=!!o;try{return await kira(t)}finally{oral=false}}
const synth=window.speechSynthesis,SR=window.SpeechRecognition||window.webkitSpeechRecognition;
let actif=false,rec=null,sil=0,tour=0,wl=null,voixFr=null;
function cv(){voixFr=synth.getVoices().find(x=>/^fr/i.test(x.lang))||null}if(synth){cv();synth.onvoiceschanged=cv}
const propre=t=>t.replace(/\*\*/g,'').replace(/[#*_`]/g,'').replace(/https?:\/\/\S+/g,'').replace(/\s+/g,' ').trim();
function dire(t,fin){const mon=++tour,ms=(propre(t).match(/[^.!?…]+[.!?…]*/g)||[]).map(s=>s.trim()).filter(Boolean);
 if(!synth||!ms.length){if(fin)fin();return}synth.cancel();const suite=()=>{if(mon===tour&&fin)fin()};
 setTimeout(()=>ms.forEach((m,i)=>{const u=new SpeechSynthesisUtterance(m);u.lang='fr-FR';if(voixFr)u.voice=voixFr;if(i===ms.length-1){u.onend=suite;u.onerror=suite}synth.speak(u)}),60)}
const etat=(c,m,i)=>{$('orbe').className=c;$('etat').textContent=m;$('orbe').textContent=i};
function arreter(m){actif=false;tour++;try{if(rec)rec.abort()}catch(e){}if(stopper)stopper();if(synth)synth.cancel();etat('',m||'Appuie pour parler','🎙️');if(wl){try{wl.release()}catch(e){}wl=null}}
let stopper=null;
async function enregistrer(){
 if(!navigator.mediaDevices)throw new Error("Adresse non sécurisée : ouvre Kira avec http://localhost:8080 (pas [::]) ou avec le lien https.");
 const st=await navigator.mediaDevices.getUserMedia({audio:true});
 const AC=window.AudioContext||window.webkitAudioContext,ac=new AC(),an=ac.createAnalyser();an.fftSize=1024;ac.createMediaStreamSource(st).connect(an);
 const mr=new MediaRecorder(st),ch=[],buf=new Uint8Array(an.fftSize);mr.ondataavailable=e=>ch.push(e.data);
 return new Promise(ok=>{let parle=false,der=Date.now();const t0=Date.now();
  const fin=()=>{clearInterval(iv);stopper=null;if(mr.state!=='inactive')mr.stop()};stopper=fin;
  mr.onstop=()=>{st.getTracks().forEach(t=>t.stop());ac.close();ok(parle?new Blob(ch,{type:mr.mimeType}):null)};
  mr.start();
  const iv=setInterval(()=>{an.getByteTimeDomainData(buf);let m=0;for(const v of buf)m=Math.max(m,Math.abs(v-128));
   const t=Date.now();if(m>12){parle=true;der=t}
   if((parle&&t-der>1300)||(!parle&&t-t0>8000)||t-t0>30000)fin()},100)})}
async function transcrire(b){
 for(const m of['whisper-large-v3-turbo','whisper-large-v3']){
  const fd=new FormData();fd.append('file',b,'voix.webm');fd.append('model',m);fd.append('language','fr');fd.append('response_format','text');
  const r=await fetch('https://api.groq.com/openai/v1/audio/transcriptions',{method:'POST',headers:{Authorization:'Bearer '+S.kira_key},body:fd});
  if(r.ok)return(await r.text()).trim();if(r.status===401)throw new Error('Clé Groq refusée (⚙️).')}
 throw new Error('Transcription impossible (modèle Whisper indisponible ?).')}
const errMic=e=>e.name==='NotAllowedError'?'Micro bloqué : dans Chrome, ⋮ › Paramètres › Paramètres du site › Micro, autorise ce site.':'Micro indisponible : '+(e.message||e.name);
async function ecouter(){if(!actif)return;etat('ecoute',"Je t'écoute…",'🎙️');$('toi').textContent='';
 let b;try{b=await enregistrer()}catch(e){arreter(errMic(e));return}
 if(!actif)return;
 if(!b){if(++sil>=4){arreter("Je ne t'entends plus.");return}setTimeout(ecouter,200);return}
 sil=0;etat('reflechit','Je transcris…','✍️');
 try{const t=await transcrire(b);if(!actif)return;if(!t){setTimeout(ecouter,200);return}$('toi').textContent=t;parler(t)}
 catch(e){$('kv').textContent='Erreur : '+e.message;arreter('Erreur de transcription.')}}
async function parler(t){
 if(/(^|\s)(stop|arr[êe]te|au revoir)([\s.!?]|$)/i.test(t)){actif=false;try{if(rec)rec.abort()}catch(e){}etat('parle','Au revoir !','🔊');dire("D'accord, à bientôt !",()=>arreter('Conversation terminée.'));return}
 etat('reflechit','Je réfléchis…','💭');
 try{const r=await repondre(t,true);if(!actif)return;let txt=r;if(typeof r==='object'){add(t,true);add('',false,r.html);txt='Voilà ta photo, elle est dans le chat.'}
  $('kv').textContent=txt;etat('parle',"Je parle… (touche le rond pour m'interrompre)",'🔊');dire(txt,()=>{if(actif)setTimeout(ecouter,250)})}
 catch(x){$('kv').textContent='Erreur : '+x.message;arreter('Erreur.')}}
$('orbe').onclick=()=>{if(!navigator.mediaDevices){etat('','Adresse non sécurisée : ouvre http://localhost:8080 ou le lien https.','⚠️');return}if(!actif){actif=true;sil=0;try{navigator.wakeLock.request('screen').then(l=>wl=l)}catch(e){}ecouter();return}
 if($('orbe').className==='parle'){tour++;synth.cancel();ecouter();return}arreter('Conversation arrêtée.')};
$('bwave').onclick=()=>{$('v').classList.add('on');etat('','Appuie sur le rond pour parler','🎙️')};
$('vx').onclick=e=>{e.preventDefault();arreter();$('v').classList.remove('on')};
$('bspk').onclick=()=>{vocal=!vocal;$('bspk').textContent=vocal?'🔊':'🔇';if(!vocal&&synth)synth.cancel()};
$('bset').onclick=()=>{const k=prompt('Ta clé Groq (gsk_...) :',S.kira_key||'');if(k&&k.trim())S.kira_key=k.trim();const m=prompt('Modèle (openai/gpt-oss-120b ou openai/gpt-oss-20b) :',modele());if(m&&m.trim())S.kira_model=m.trim()};
$('f').onsubmit=async e=>{e.preventDefault();const t=q.value.trim();if(!t)return;q.value='';q.oninput();add(t,true);const w=add('…');
 try{const r=await repondre(t);if(typeof r==='object')w.innerHTML=r.html;else{rend(w,r);if(vocal)dire(r.slice(0,800))}}catch(x){w.textContent='Erreur : '+x.message}log.scrollTop=log.scrollHeight};
$('bfile').onclick=()=>$('file').click();
$('file').onchange=async e=>{const f=e.target.files[0];e.target.value='';if(!f)return;const t=q.value.trim();q.value='';add('📎 '+f.name+(t?' — '+t:''),true);const w=add('…');
 try{let r;if(f.type.startsWith('image/')){const b=await new Promise(ok=>{const x=new FileReader();x.onload=()=>ok(x.result);x.readAsDataURL(f)});
   if(b.length>5e6)throw new Error('Image trop lourde (max ~3 Mo).');
   r=await groq([{role:'system',content:'Tu analyses des images avec précision. Réponds en français.'},{role:'user',content:[{type:'text',text:t||"Décris cette image et analyse ce qu'elle contient."},{type:'image_url',image_url:{url:b}}]}],'qwen/qwen3.8-27b')}
  else r=await groq([{role:'system',content:sys()},{role:'user',content:'DOCUMENT :\n'+(await f.text()).slice(0,15000)+'\n\nTÂCHE : '+(t||'Fais un résumé clair et structuré.')}]);
  rend(w,r);if(vocal)dire(r.slice(0,800))}catch(x){w.textContent='Erreur : '+x.message}};
const J=k=>JSON.parse(S[k]||'[]'),W=(k,v)=>{S[k]=JSON.stringify(v)},esc=s=>s.replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;'),uid=()=>Date.now().toString(36)+Math.random().toString(36).slice(2,5);
let P=J('kp'),A=J('ka'),CV=J('kc'),C=null,vue='c',blocs=[],cur=null;
function ext(){const p=P.find(x=>C&&x.id===C.p);return' Mets tout code dans des blocs ```langage.'+(p?` Projet « ${p.n} », instructions de l'utilisateur : ${p.i}.`:'')+(C&&C.code?' Mode Code : tu es développeur senior ; donne le code complet puis explique brièvement ; pour une page web, un seul fichier HTML autonome.':'')}
function nouvelle(code){C={id:uid(),t:'Nouvelle conversation',m:[],p:S.kproj||'',code:!!code};hist=C.m;log.innerHTML='';
 add(code?'Mode Code : décris le programme à créer ou colle ton code.':S.kira_key?'Salut ! Pose-moi une question ou touche 🎙️ pour parler.':'Bienvenue ! Touche ⚙️ pour mettre ta clé Groq (gratuite sur console.groq.com), puis pose-moi une question.')}
function sauve(){if(!C)return;if(C.t==='Nouvelle conversation'&&C.m.length)C.t=C.m[0].content.slice(0,40);if(!CV.includes(C))CV.unshift(C);W('kc',CV.slice(0,40))}
function rend(el,t){const p=t.split(/```(\w*)\n?([\s\S]*?)```/g);let h='';
 for(let i=0;i<p.length;i+=3){h+=fmt(p[i]);if(i+2<p.length){const n=blocs.push({l:p[i+1],c:p[i+2]})-1;
  h+=`<pre><code>${esc(p[i+2])}</code></pre><div class="bt"><button data-a="cp" data-n="${n}">Copier</button><button data-a="ar" data-n="${n}">📦 Garder</button>${/html/i.test(p[i+1])?`<button data-a="ap" data-n="${n}">▶ Aperçu</button>`:''}</div>`}}
 el.innerHTML=h}
function voir(a){cur=a;$('at').textContent=a.t;const b=$('ab');b.innerHTML='';
 if(/html/i.test(a.l)||/^\s*<(!doctype|html)/i.test(a.c)){const f=document.createElement('iframe');f.setAttribute('sandbox','allow-scripts');f.srcdoc=a.c;b.appendChild(f)}
 else{const p=document.createElement('pre');p.textContent=a.c;b.appendChild(p)}$('av').classList.add('on')}
log.onclick=e=>{const b=e.target.closest('button[data-a]');if(!b)return;const x=blocs[+b.dataset.n],a=b.dataset.a;
 if(a==='cp'){navigator.clipboard.writeText(x.c);b.textContent='✓ Copié'}
 if(a==='ar'){A.unshift({id:uid(),t:(x.l||'code')+' '+new Date().toLocaleDateString('fr-FR'),l:x.l,c:x.c});W('ka',A);b.textContent='✓ Gardé'}
 if(a==='ap')voir({t:'Aperçu',l:'html',c:x.c})};
$('ax').onclick=()=>$('av').classList.remove('on');
$('acp').onclick=()=>{navigator.clipboard.writeText(cur.c);$('acp').textContent='✓'};
$('adl').onclick=()=>{const a=document.createElement('a');a.href=URL.createObjectURL(new Blob([cur.c],{type:'text/plain'}));a.download=(cur.l==='html'?'page':'code')+'.'+(cur.l||'txt');a.click()};
const dr=$('dr'),ferme=()=>dr.classList.remove('on');
function liste(){let h='';
 if(vue==='c')h=CV.map(c=>`<div class="it" data-o="${c.id}">${esc(c.t)}<b data-x="${c.id}">✕</b></div>`).join('')||'<i>Aucune conversation</i>';
 if(vue==='p')h='<div class="it" data-np="1">＋ Nouveau projet</div>'+P.map(p=>`<div class="it ${S.kproj===p.id?'sel':''}" data-p="${p.id}">📁 ${esc(p.n)}<b data-xp="${p.id}">✕</b></div>`).join('')+"<i>Touche un projet pour l'activer.</i>";
 if(vue==='a')h=A.map(a=>`<div class="it" data-v="${a.id}">📦 ${esc(a.t)}<b data-xa="${a.id}">✕</b></div>`).join('')||'<i>Aucun artéfact : garde un bloc de code avec 📦.</i>';
 $('dl').innerHTML=h}
dr.onclick=e=>{const d=k=>e.target.closest('['+k+']');let x;
 if(x=d('data-x')){CV=CV.filter(c=>c.id!==x.dataset.x);W('kc',CV);liste();return}
 if(x=d('data-xp')){P=P.filter(p=>p.id!==x.dataset.xp);W('kp',P);liste();return}
 if(x=d('data-xa')){A=A.filter(a=>a.id!==x.dataset.xa);W('ka',A);liste();return}
 if(x=d('data-m')){const m=x.dataset.m;if(m==='k'){nouvelle(true);ferme()}else{vue=m;liste()}return}
 if(x=d('data-o')){C=CV.find(c=>c.id===x.dataset.o);hist=C.m;log.innerHTML='';C.m.forEach(m=>{const el=add('',m.role==='user');if(m.role==='user')el.innerHTML=fmt(m.content);else rend(el,m.content)});ferme();return}
 if(d('data-np')){const n=prompt('Nom du projet :');if(!n)return;const i=prompt("Instructions pour Kira dans ce projet (ex. « tu m'aides à réviser le BAC ») :")||'';const p={id:uid(),n:n.trim(),i};P.push(p);S.kproj=p.id;W('kp',P);liste();return}
 if(x=d('data-p')){S.kproj=S.kproj===x.dataset.p?'':x.dataset.p;if(C)C.p=S.kproj;liste();return}
 if(x=d('data-v')){voir(A.find(a=>a.id===x.dataset.v));ferme()}};
$('bmenu').onclick=()=>{vue='c';liste();dr.classList.add('on')};$('dx').onclick=ferme;$('bnew').onclick=()=>nouvelle();
q.oninput=()=>{q.style.height='auto';q.style.height=Math.min(q.scrollHeight,140)+'px';const t=!!q.value.trim();$('bsend').hidden=!t;$('bwave').hidden=t};
$('bmic').onclick=async()=>{const b=$('bmic');b.textContent='⏺';try{const a=await enregistrer();if(a){q.value+=(q.value?' ':'')+await transcrire(a);q.oninput()}}catch(e){alert(errMic(e))}b.textContent='🎤'};
nouvelle();
if('serviceWorker'in navigator)navigator.serviceWorker.register('sw.js');
</script></body></html>
