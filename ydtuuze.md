代发 wailian999

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/ggklbdpmh.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/giqemicnc.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gzxfwmjay.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gpzryfzri.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gamappuig.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gftqyljmr.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/ggbbvwldl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gpbezcdnj.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gwjxahcip.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/ggvhntxgo.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gvhyrgljf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gwhphzarc.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gpknhzvkx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/ggzgotiyi.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gavblstkm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gsojdkneb.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/giacmgqnk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/grvozjkam.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gfpfsdnxk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gdyktgpze.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/ggkljdlgc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gkpwtyahc.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gixsglezz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gjjcrmpkv.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gsfqvruwi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gcwzsjdzl.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gmwsphoxb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gbpldoywm.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gucztiiju.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gvvcmvnvr.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/grtvtnvic.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gmsexuoix.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gmajupjvv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gmoufgsye.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gwwphunbl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/glggvcwni.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gaqkbjgqv.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gtyueqddo.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/ggtcncypy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gkgfyzwwo.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gdcxkjvkr.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gfufwuryu.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gxtuylxsc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gcsaqmgru.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gclbtkcce.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gbzgqpsrj.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gyuxlfssn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/glclkegrz.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/guspwvnmj.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gvzdasdhx.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gdzyeuukn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gmrzjaxxh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gxfoqcnth.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gegifkxzc.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gknmdiexb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gfdfernwk.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gstjnmcpp.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gyxqvpnky.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gzgkzsveb.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gqslctjke.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gqjwhkgnn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gyszzerym.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gpxwhvklb.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gwipubkpe.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gcbsfhbcp.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gbyiemkrw.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/giyewkmnc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gzotgalyi.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gevueemsq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gucedxtki.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gqsnmaxma.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gkdrntiwz.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/grppoqctn.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gbqhhvkky.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gsppuewrq.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gyaewcasd.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gtqktlzpw.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gawedvlsc.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gnmxziuea.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gitkuwxaj.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gzfztfvpl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gkpnuawev.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gicbxbfwy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gzanslpzw.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gdjtrvkhc.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gbdrjkrrh.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gseagwjdb.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gfgfrptkh.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gheqpyjxy.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gmczvreac.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gpeoylgly.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/ghmymjhtb.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gckmopode.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gmaehvzew.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gbrytxruz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gvdyfuudz.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/ggcshzyqh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/grdgwnsqo.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gvmeopfnw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gcmoopfcd.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gnuuilzto.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gusultrkc.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gbihrgomr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/glydkpwlv.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gdmaguyou.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/ggrihcwkj.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gwsanlurd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gznzupfvp.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/grqnqxfrh.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gamgqdamx.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gnxcezkyc.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/grzoqrezk.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gsyzdswhr.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gjdtornne.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gayrbrmjv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/groyrurgu.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gahdegwpm.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/govvhsajm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/ggbtdfgzc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gpciyamif.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gyxphdkqk.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gcoyvscrv.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gfzpidzso.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gskjfsrqm.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gnvehtefj.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/ggreekzzm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gzhxhcfpy.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gpnrwsere.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtzcurwqi.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/ghzkpwdwz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzgqfywee.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gllmxsfsu.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gjdvyrack.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gscqeruup.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gizwwgiyc.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gxaldtuer.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/grgutlqjh.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gdomomohz.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gaxozuvry.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gezazthmd.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gofntcaen.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gjutbphwh.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gzhwhkqeb.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/grrkgsjlv.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gkawdbgcu.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gsswqdhmu.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gxxomzkbj.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gytraklod.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/grmnolwci.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gstperoym.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gdnawxfof.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gnpgqhwcg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gwwsyvqoz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gpvqeivbg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gxpuqxikg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/giyclrpox.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gawlttjva.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gitortywe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gqtveddvo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/guzohurgb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gwjrrtdbf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/geueubkoy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gwqncxnzh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gajgcfdwv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/geeiaybyw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/giamqesxx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gvifozkad.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gdnixqhqa.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gmggjwori.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gfefbuiea.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gqbvalyex.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gmxcreftz.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gdtfztmrq.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gyxuuoshd.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gxeqnkuva.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/goqsvzria.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/grhrgvjym.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gduiljfsf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gttptxvet.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gjaxvdjwj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/ggmhnxlku.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gqdvolsfd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/getukmxck.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gopffzfjn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnyakijhw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gzcjexqwy.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gomncubkb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjkdoucky.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gkgxhbrjb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gzfdmmgbj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/geeqnpfeq.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gqkyrtpqb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/gutvbunok.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gbkqmzcyb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/goggdosuk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gcvwvpshi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gqgamyreo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/ghauppxmv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/glmdjnycr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gcirvvqtj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/gwqvepttj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gcdgzxryq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gbmsazlwp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gqroqpzjf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gqwhoaraw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gdccuqjfm.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gaykscefk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/gexxlmork.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gwwocfkmk.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gbrjymhtn.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gvsubufbx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gitvlqvfb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gchgfyngp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gcdckzvxi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gynywrkce.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gqgtaqbhv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqavujfkx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gjsxffubw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gvxuqzprj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/garwklxiw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gmwnykzjy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gmtjdquyn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gziplndcw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gppozeabv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gdjraexal.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gxercozum.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gsfhsgxte.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gptibjlnr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gjfayppbe.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gjofjjwtc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/ggiiqbdji.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gqsdwclgi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtpajiyea.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gysqqgssi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggsbxdipp.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gbnwobwyw.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/ggniickno.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/grzpjrfxl.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gubgbfsjy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gwjiwxdnf.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gkszvlmjh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gdanqeohs.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gjeibujpp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gaeqxdjup.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gtokiefbm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gkyqehbgq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/gcohjadfi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gnwpqxxza.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gyszxaoxp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gshefbcxd.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gnnurqiwi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/gyavuybli.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/ggzzkagpa.sHtML

[A03] 常量定义
来源：http://m.share.zdbjq.cn/Article/details/gcgpvmbee.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/gnoublria.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gudidsxzn.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/ggblyufkh.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gegosvtdg.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gjhjtgeni.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gpvhprmfh.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gbnejetog.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gainrvngr.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gluzyecgr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gqmgzodll.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/gswrlbmpx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gmpghkkeo.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gztgtvqem.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.hesvh.cn/Article/details/gaiuivfdx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fehbvm.com/Article/details/gydldlwhq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gpjsddezp.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gqdsmpwca.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/gjlmrvfbe.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gefnwtuse.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/giuiiuiib.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gpkkhqolf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gjkndzezn.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gtakzammb.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/glqchxzip.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gdcqnefin.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gixxcozai.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gtzfyouce.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/goefquxbq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/glueighxp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gvqzzqxgh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gsilkawtn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gnoxhfllz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gqrdxfnpb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.zdbjq.cn/Article/details/ghjcuammo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.hesvh.cn/Article/details/gmgnvysmt.sHtML

[A07] 数字转字符串
来源：http://m.share.hesvh.cn/Article/details/gtljjzdhh.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/gamgpcamo.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.hesvh.cn/Article/details/ggsxewhxk.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fehbvm.com/Article/details/gtphvaxrg.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/gvmwqjpqh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/glanaedmt.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gotdtspky.sHtML

Ruby: 42.to_s
来源：http://baike.fehbvm.com/Article/details/ghxvawovz.sHtML

C#:   42.ToString()
来源：http://read.share.hesvh.cn/Article/details/gjbalgatr.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/ggmkdehgg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gficjfcsz.sHtML


<!-- 参考信息 -->