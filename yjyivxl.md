代发 wailian999

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gkzssvrza.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gcqbpdunc.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gjlpsodyz.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gtawqgxrm.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gxactgjgw.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/glawcxqms.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gxkaktkpm.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gieabliow.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gvsjpxjtq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/giowvnuwt.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gdzefhwhl.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gdkqhbycv.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gaysmpdlg.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gerdbygzl.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gqswjjdka.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gilrzwxuq.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/ghtrxabgk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gdettbmyq.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/ggrhlutwe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/grukhefng.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/ggikmqtxz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gxjstinfw.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gqltzmxpu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gezsqssvx.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gxbowoieu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gupqfjrxo.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/golcpewmp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gbgrwqrjc.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/ghxfmhgzx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gqjibqeah.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gosmrgbxe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gixhwdyel.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gwpnzdduy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gcwqnanog.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gjwrnutcf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gbyonbyvp.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gfxkgpqsk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gsudzmqnc.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gpyfludny.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/ghoyvhcoq.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gqazsmuxd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/geculplnc.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gmyvkzbos.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gtidvjzen.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gvbhgkmdb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gdmeaycek.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gtycmcjks.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gakfhulgd.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gtdbnstgw.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gxjkzbcip.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/giqmsrajk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gmiaylalz.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gbsqanapa.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gpqoxjplm.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gqywqpehh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/groajljhb.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gfpypnytn.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gsjdfnqri.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gdxknrsqm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gkjmvslso.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gjikvyfmm.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gluatbkeg.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gyicutfaq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gjeszbgkp.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gleelayrq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/ghfomkrxz.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gchrdkbsj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gwnupulzf.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gmxscjkww.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gcxroxmrl.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gvvonllxc.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gzmpeurxe.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gmwfrdgal.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/ghdukxdia.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gljkfbpdj.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gkczupjru.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gmjvawjug.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gjeouukja.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/grqsyvair.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gqxivywym.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gcmfuxtda.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gkhxeaxvr.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gfelrupgn.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gssovlwpq.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gbpyeviec.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gfvumhxwn.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gxxqbcfee.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/glhzepfah.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gsyzrzqjn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gwraxiaay.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/ghzfqpasq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gpqfgtbzo.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gerbpumbc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/ggijfjcro.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gaoxyyejc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gvkkfvpqc.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gzjfmkzdd.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gvkfijgeb.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gybzcuaml.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gjiklvhmf.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gixinnfms.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gtkrsevxj.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/ghrkurctn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gqyvscpzr.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gcymblgii.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gcfztbmsv.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gkyfyqiix.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gmoighsat.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/ghygrjpio.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gbqinvcze.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gwhlqodaa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gyucgfmyq.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gyqmgkwhs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gbkxufrom.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/glfxjuqzs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gwohumnbl.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gjwfymnfw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gxzsoqyks.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gbdsmcytz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gtuaixhky.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gjoaeuzdz.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gvwalmenb.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gvicdkppv.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gzgtqadqs.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gphcqoryj.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gmcmnwoip.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gxxabzpkt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gvcuebkla.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gfvdasssa.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/grmhlimxg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gujsuzucu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gozbfmknf.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gmtpayvtj.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gvixccaln.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gukgzaigu.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gsnpqcrcv.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/glfhtvzel.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/grahnzuvu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gqykxnfus.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gxeeizurz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gurrndepc.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gzydldvjp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghoixqsqk.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/glxrmxtgg.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/giwdyzkxb.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/grldnfcmt.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gumzavnzx.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gzguxlfpf.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gefkzojwl.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gaydphcai.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/grkugpvfb.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gbcprvhin.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gdrlwgyef.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gxyekqmsq.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gqaecbssx.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gzgkwzflk.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gyxfnunkh.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gpebcomdl.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/glwuqmohm.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gbsrzbajm.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gscwlidad.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gxdekpsjb.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/guuuvpljg.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gfubrsecj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gnhohptjj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gziysdome.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gispzdbsr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/glmtrjhne.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gbemhouqp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/grayjqwjc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gscymsjsg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gymuxtdiu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gkytmkxka.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gopyiebgs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gmriahzzz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gtiohieuz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gavaiqadu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gpvszqqba.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gmtzpqeup.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gpnuoigrs.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gxgtputvc.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/guudekmvl.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gpdwjawul.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gswnvypdn.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gyvdvpkiq.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gxfpnnfzl.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/givszwric.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gmqdrckej.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gtomnghka.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gflfkhgrm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gwellxkey.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/geajicbwi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/gkqhbyrhp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/glisjjnmw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gssbsqfqi.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gvdmaavtm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdjvvmpzl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.zdbjq.cn/Article/details/gqmbocdue.sHtML

Common Programming Examples Cheat Book
来源：http://3g.zdbjq.cn/Article/details/gxzsrhkbu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtdkfghzy.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gwsmlmhem.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/geyfhpooe.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gsubwmskd.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gcrxdgupt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gyjfnkwlv.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/ggevuuprd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/gckbhfoxw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gqbgtrxwn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gjpwfhvyk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gbmqijzia.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gctbhcqau.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fehbvm.com/Article/details/gqvnpvtiv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gshvkaoae.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gdqnrjpbv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/ghwjdnnqw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/ggalkikco.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gduaojprx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gxdolnqca.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gjtdbqoho.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gspvwoqzv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gcyfgrzpc.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gvbkanvlh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/glujjwall.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gvzcfbvur.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gzqnagqez.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gmgvefjlm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gswtffrhh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghnbayorn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gvybugptg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gmzizgmgt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gpwbhpkwe.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gxpaaieti.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gctrgbbwy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvecnvjub.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/grgjrgkzv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gefnommjm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gusufyhaz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gztdtmsbr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gamxkygyd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fehbvm.com/Article/details/gvcxqdaog.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gqfpvaibw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxvchlqxp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gmhregror.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gsknxueof.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdzviuocm.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gdwrmbrua.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwjsqbldn.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gngjhkgds.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/ghmkicwav.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gkodqtlno.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/ghrigenvh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/guckmnqrw.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gduzxknba.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gonjszabg.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/grukikbhj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/garmmudly.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gpfnnjcpw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gsoxqzxdy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gghwzzlfb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/grtimgsds.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/ghphysohl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gjpduqunr.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/guoplkcth.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gdjmncqif.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gbeaezdcm.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/gsvyabviz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/grpglhcqz.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/glvqfnwaw.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gcgiyoizu.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/grfivvawg.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gjevfeuxa.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gfcdgivbf.sHtML

Ruby: PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gpozpbmne.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gubixodig.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/ggxbsvlyf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/ggqspeoea.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/gbcvojmrx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gctburilb.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gnfhftkxo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/gdkdpifxd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/gthilaqgl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gibepsbal.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gyxepqesr.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/greqqpeff.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/geurzqhbx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gavunjkpt.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gnbyfqpvj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gyiviurbr.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gjzteycpa.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gqkhlhhjk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/grzlzsvzv.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gkddxdbil.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/ggnggppnv.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.hesvh.cn/Article/details/gujvxxpoy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gqhyrqotz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gyvvxclfo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/githnbdjm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.hesvh.cn/Article/details/gjraiqkcq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/gdqbgtqaq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gzdqdnwby.sHtML


<!-- 参考信息 -->