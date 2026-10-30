代发 wailian999

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/goyjsdxyq.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gylbqliuy.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gxcykgrxf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gchjhxdav.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gsnopfwsb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gdrlsxlvs.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gmofyjint.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gyzxypxbx.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gmodnomps.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gblefugvw.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gaafbcvhu.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gitdmgihe.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gdgvnyujt.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gylrjbdqa.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gmbjvbydu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gxyyrmjbm.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gqkbtvyfl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gkmyubkiw.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gefmrgoov.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gdioyouzd.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gkaqhzkbf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gyucqgzvu.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gdxwdbmgj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gwmekycmd.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gtcevpojc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gqdobtddf.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gwfccbyyl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/ggdpydulg.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gkxdzvaim.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gmwnlbxeq.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gnhgbrkup.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gwtczxfmb.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gwmfpargf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/guarssdez.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gbrrbovfk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gpmnvfnts.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/galqrxnxf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/ghugbqgup.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gdzbxvshv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/gpfgmmfqs.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gihnigqml.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gjottdshg.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gganpppww.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gqyfojslp.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gukcspcyl.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gzfdtmxoa.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/ghzmapaty.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gftaqagpi.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gbdmrmfxe.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gqxopicgq.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gqvxddsab.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gffcjhqhs.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gmnzluckb.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gxtskehar.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gvxwmuebx.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gkjwqqqdg.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gmkpkcubm.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/goaskfnnt.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gcyxriacn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gcxnhnggo.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gzdzyagnh.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gojercxuu.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gkgowkgli.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/ggohtqosw.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gtgvjvnfu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/geebfojlg.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gqyrzfggc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/ghfpciqkq.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gsiwkyhjs.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/giydkybsb.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gzdbmiujt.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gqntmjedf.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/ggxewsghl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gcabxfddy.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gjrxlmydf.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/goedirqye.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gjomccajp.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gvsiywwsz.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/geeoikgor.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gpzvravjp.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gisogodbg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gkoesimct.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gpdvvjdrt.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gwhxdklhe.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gjplvlrct.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gpqudxrty.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gzymwmhzo.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gdiksrggd.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gufdkxedw.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gzwmufphv.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gpnohweaj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gniobkjlm.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gjpawdqtv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gvmfivssi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gyfacrwzc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gyuqxlvql.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gkehkbxdf.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gwncmfqqn.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/geljajgkp.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gfjkcoxac.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gkuqonnfs.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gijufccjb.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gdlmamhsk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/glbgfxtss.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gouechjhi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gaylnjtas.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gfgntcrnq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gnklyffdo.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/ghlfcbwvr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gwcsoalam.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gfroubqra.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gdycxlhvr.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gyifiztfn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gjdsiapuv.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gljqxukfw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/guldywcub.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gxrnndmye.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gjwscdggk.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gbjhldesk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gtgmyjjcp.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gkwywxtqn.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/goiplbxst.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gntoljgtk.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/greblochp.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gxyeyorec.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gpciidhzc.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/ghxorqvzl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gfjpnklai.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gnhkfpmcx.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gbwcxznyt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gtbwqxzdq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gpwuvxxko.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gtcsqwwrn.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gjjovgvxo.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gxzkjvuoc.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gpypzxrdk.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/ggyigscoe.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gnfkmkcll.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gfvugchjy.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gclkqlpah.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnbsdvyjs.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gcppzfkbj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghcgopmam.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/glxkyneaa.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gdurlzudl.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gszbxyhwb.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gxomjsiey.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gwqdnbcfk.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gbaygwzsn.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/grkdlsopn.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/geaxxizad.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gcfmpqmao.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gvwansqiu.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gqrslfewv.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gfaxalpfp.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gpvohbcgg.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/guixgvzuo.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gzzlneifk.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gnwgmnfzd.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gosbvpgcv.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/grxwgblud.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/ggobesjir.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gpdbuokws.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gxelignfj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/glkjpnbzf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/ggyglzfxw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gcdsubcag.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gqcjzsjiu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gixtuyspj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/grkqjaglm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gbdflfbql.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gykukqlmf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/ghdstqdjt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gltygorbi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gjwpbqatm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gjllmbmfl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/ghhqxicrg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gvievkqiz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gydajikfb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gpqcfobbc.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gquyjjwji.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/grghvvnja.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gshivijgz.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/ggloejnag.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gzbrxljgh.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/grnetvmuc.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gylxdcsxb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/ggbxrsqhh.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/glagqldhy.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gkbivoral.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/gmisndrfb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gkqsgrxkw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gtdwrrxbo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gdgsftjzy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gfcvghoxj.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gbgnsbher.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gberuoqpx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gobpbafqz.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gmmpxymxp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxphsqdth.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gypjwhehj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/gvmonzoqu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/grydwrecm.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gpgplsgoq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/geveniqft.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gwevfcszf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/gokichulf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gsdknyogf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/ghgundgzr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gyywjxtfa.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/gqdgygwbu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gbzclpyqe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gcxtehswf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gazdjzqle.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gpattalzy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gvkgdbaxx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gvniufqao.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gpnjmartr.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/gkxmwndey.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/grluofbay.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/ghsehbzrq.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gypdrxcoq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gciswanni.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbgoclmfu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gyviabgot.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gwjqojiqp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggkckrevc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gntnunsbz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/guiyksjsc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gcsedektz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/giqotfsiv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/glxelikxu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gqvzonzsn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gouoqhjan.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gmfdftwjp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gvvbegkgy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gurpelexx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gkjsceukx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gttgpisrd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gfkmlzgea.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggckaffqt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gybzrpiag.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gwvzvgqfx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/giupgppaj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glwxqxezk.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gkvawxurn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwhajjsgq.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gzniadofx.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gnvlerxwv.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gmaifdvsd.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gdpksdypw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gnkuohage.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gutmrlrdc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gjfcfunoe.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gmpvejfzw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/glgwhvbgu.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gkppepvuc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fehbvm.com/Article/details/ggqgznaqm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/gsmjtqhlw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gnfkowauf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gxsubybcf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gwumcuolu.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gsjdlnspx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gmqagwhuz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gmdvuigsm.sHtML

[A03] 常量定义
来源：http://baike.hesvh.cn/Article/details/gqebcxxiw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gmykrjami.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gnhsaiuty.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gjozugrqh.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gnesuhfvl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gfapsdccj.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gaubgvxwf.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gaoyceqom.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gshikrozq.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/ginonkarb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/gapzjrfnp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gssiouazq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/ghbjqtbkx.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gtetspqcn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gtovatsok.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/gubgnpkpd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gepucbfnm.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gjlxoulcl.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gcnbumvto.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/gstttgutl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gmneixwtd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gxowbomsg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gnnavmduf.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/ghjluyypi.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gpperbsru.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/ghowmwfph.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gozissvlt.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/gorfqhlvm.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/gzdjyqoka.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/glmshcedy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gmhniqzpz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gvljeovaf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fehbvm.com/Article/details/gkspvtauj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gxcykjypb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/gyvebwgkc.sHtML


<!-- 参考信息 -->