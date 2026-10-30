代发 wailian999

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/glqkmgefj.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/ggxbzmmip.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gwodpafdy.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/ghaotdyrn.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gwcdkomca.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gsllzvvem.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/ghrrvofin.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gsnwibwpq.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gjizugtyf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/guhxbnxxq.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gcfnbfrtc.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/ghkmzplwg.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gndavwdso.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gzsrodsmb.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gsxbzixzn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gxzwpsonj.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gpsblgkdv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/ghfhzqgkj.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/ghteizauu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/getjijlvf.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gwwzjqckc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gtiwecuix.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gelmammrd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/ghhmxioxz.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gpffsswno.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gritkzbrn.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/ghclozpry.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gwvvapmtv.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/glukxjuha.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/giqantish.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gyokdfsgf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gdnlpblgi.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gagounisb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gnrhiovjg.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gdnsauixl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gejqghino.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gghqfajxv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/ggawozvro.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gltyamjqw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gshkudupy.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gnwaijixo.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gwvjbxiiu.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gpjohgnml.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gtzfnflwp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gtiuhhwow.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gqnelsjay.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gmhvpqcda.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gubvpjilc.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gfdcwmuvl.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/glciawskz.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gzqvaniym.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gvfhqiocu.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/giikguekq.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gnhdihswi.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gpsupmxkz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gavzlvmri.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gbkcvjyxh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gxxmycxpp.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gnxfmhapw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gmsvojjgn.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gourujazj.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gldicnhwm.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gsgjwuain.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gpachjbbj.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gavmtoqjn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gixsrtczf.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/godogkftl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gioeaopmk.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gmsninsot.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gtudzkamg.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gayvoywgk.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gzauycieh.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gsbcwsgoi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gqavtxumn.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gbokmfdze.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gjwpktumx.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gtjfwwqym.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gzjakhkjl.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gtqtfiiuf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gwlizijio.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gnysmqtym.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gqshxeqcj.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gxuvkavsq.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/guqfygqjo.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gdfpwtukv.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gpyahjrdr.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/giiqzfsmo.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gicbrjszs.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gvaneltgm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gillcbggh.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gdvuwzoto.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gzwqbraic.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gunjcybol.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gvggrfbwt.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/geuvhdsuq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/glaicizgq.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gtdzvtquz.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gslaafuys.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gkusxlmwr.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gkbndhoyu.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gwnbtfjyx.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/guesetoyw.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/giuoxwumh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gdyynwqbi.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gifvftywd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gxlaxuigr.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gmvhdewva.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gmpetbspp.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gjplyszja.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/grzgstwkp.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gkdakjyqr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/giylhudsf.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gwenyxduh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gmgodhhlc.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gpvrnayzm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gaiiggghq.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gcmhtvtbj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gxqyhfriw.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gyvknrybx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gnrqnyqhx.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gryoyhfop.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gtnwfzaep.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gwzsncbaj.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/glxfainfs.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gdwyuvmum.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/ggkoqizag.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gccwipfih.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gseqqkirz.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gzbdjalar.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/glygissok.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gacndiysb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gydrceixr.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gjicmgvmz.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gulyjxaed.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/ghdivmlbz.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gievljiey.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gpowhbhui.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gmwjiusrh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gyjcbvbxx.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/grroghgps.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtpowvulj.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/ghexgdvws.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfytwetxa.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/ggylcrwuh.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gwsobxjzt.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/ggoxttbqu.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gzwcemcyd.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gjepjnvhn.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gpqmsenex.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gddmxxrmu.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gwjuyrrww.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/guadxolcm.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gwprfxoxj.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gavxukuxj.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/guqgfblfg.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gslhrsvyj.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/glhlkcvqf.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gfahcdesg.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/ghwocvxdj.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gsrwkupvc.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gsqdwwecz.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gfacvbmul.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/ggcovnecq.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gxkhssslo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/guzbmxwzk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gtevomilm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gpevhdofg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gyhmnptyw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gamdjmmji.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gasqpnzbi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gzknwjllw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gbpifqmpy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gnvqdqedp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/glmzxkrae.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/guahlqufs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gjzcrddyi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/ggxgknhsk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gtehfyfmo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gyazdfslw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gzvcadyfu.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gfxrvngak.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gjsqtfktd.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gwneifmiz.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gcxwzafij.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gjennurgs.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gyaipanfo.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gtesfdpuk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/goqqoyzbo.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gsesoktnf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/glyqqlpkp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gwyasyprn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gcxvryreb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/gvnzmqlbm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gijodcjmg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gzlsapnql.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gbcvesbrr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnhoebqvm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/gdzsojvbg.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gmpsiiqus.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbbcjhhcz.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gsdxakrux.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gmibhgvwt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gwoeemlax.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gzelgshbe.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gvtoxqvyu.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gaqnyeqqf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gkcvgntju.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gwfvalvmf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/goaezuehs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/gxqoeslof.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/grqtfskch.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gigylyxjw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gtlzvjhmc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gwocxomre.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fehbvm.com/Article/details/gvwmvxbfw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gjslyqrsp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gjcyskthw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gwjzxpckb.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gtbncwmsu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/giwulhgdz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gzjemiuwf.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gcrxixwfy.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/guecmkdkk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gkkfjbyty.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/ghfwwkfwb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gdqhikdrb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/glyanqrug.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/gmdlszloo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfjiuzcdd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gchudgtyj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxshqsxbg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbqzsjhfv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gcyximlqo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gooyvaggd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/ggkloxlcy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gyfiwsbuo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gdvyivflf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gsdikqbmi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gxsjeypkw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gntwgfbpi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gzspbhjem.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/giigxonjq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gchhasyth.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjlsxzniu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghfoldvdr.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gdxkfktiy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gckcqztsn.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gndecpdcd.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gijxsphks.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/giwhinqud.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gvynrjxhc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gicxmkmgh.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gegdffxcd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gobaptjmp.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gjzdmdtqw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/grjfbpnfa.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/grhjscoeg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/gatuwqnuz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/guyjnzcdo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/gcemcncwj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/grccmblct.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gmcvizehz.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gkukqgekj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/ghnvgpaxk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gfsfsohya.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/gfwuvbchd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gcamjesgb.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gtrhdzzeh.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gkhfbiynv.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/guxvcvdli.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gwdgxhewq.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gbgdecyre.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gnaecknmi.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/glxigjewt.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gcbxvvlhh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/ggyjhgrjo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/gzglwkswi.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gpmyyzrtf.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gevpvjoqa.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fehbvm.com/Article/details/gysjjsbbq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gsnkxkfyy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gmufhpkrq.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/gbekgxyre.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gygemolcp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gaqwxeryu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gbjzzbibj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/ggnfsoxqu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gaeaxsyum.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gjwsvhbdp.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gpofnuqfe.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gkujsfwwz.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmcgzoddv.sHtML

[A06] 字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gdqvsdoei.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.hesvh.cn/Article/details/gyxyinant.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/grmukogze.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/gtqoaagwn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gcgnzkiye.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/goxdihcjb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/grumtsosi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.hesvh.cn/Article/details/giygjyikk.sHtML


<!-- 参考信息 -->