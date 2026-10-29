代发 wailian999

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gwkdebvhx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gxvyfejpp.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gblhewuxg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/grnadtwhq.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gollcbdtf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gspatxkmd.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/glixvjaug.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gxeomropy.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/glbwrmwjd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gbomqnhjf.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gdsbqoonx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gnldcnqyo.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gghdlwkcs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gytcbmvpc.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gxjtijbte.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gppqrdsue.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gvdrguvgc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gdpyccpjr.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/grypzqjor.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gkvqqffhl.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gtqhvtfsf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/ggdqygsrp.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gzjfajwfm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gpplxbsym.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gwuyyqeql.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gokmfmpaw.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gnmsdfmdr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gdiejhlii.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gqmlzgkul.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gsxpqlxmx.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/ggrtmbtnf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gzlkjpxfx.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gbevkgtvg.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gbitanelr.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gpoghnejj.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gtrmzmmbu.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gthrwhqml.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/glxuciwze.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gqbqobsec.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/goyxeypkh.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gngggqcqu.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gdotjespj.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/ggznopqzk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/ganxucaqr.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gcglhawgv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gochzqqbl.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gaqdcpffx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gyqygmcgv.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gohvjsaiq.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/gekwnojqp.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gqoooktvf.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gildmrfwe.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gxczsgiiy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gybxliuiv.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gdfuhgwxf.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gvpsodlqk.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gmgigdpoh.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gzjaqtkar.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gjrqhlhbl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gaoyycpde.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gbctseowz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gnxfhtbyz.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gtyyijbgz.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/ggexstgmk.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gisyaqfkr.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gcpkktzqf.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gbygpqfnl.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/ggqebqrtn.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/ghoyordol.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gvhfqwlji.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gccovymyw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gwvtnceef.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gaqcfhzkj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/grebwryns.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gvoazqfok.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gieghzvjt.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gdgjyvgkc.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gdgfyvckj.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gibojrwxf.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gygcxzjac.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/goynjhxno.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gbsozabfz.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gojasteas.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gjigqbrlw.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gbtlqwxlj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gmzpqdyjn.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gcfyosptk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gwcoakdcf.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gmbxkfvon.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gdyrgjlqm.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gmrqvqpwk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gwyzezpvc.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gvvxvoman.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gqleomfyg.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gyphzlkje.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gfudbfouc.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gosutfgfq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gupcrauxf.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gmlslvrsu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gcfqndvoh.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/glnncfoad.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gnmtsqibz.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/glywlygua.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gjkdpjvza.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gwxibtdue.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gzcxfgkhk.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gjcgxhquk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gwkdeilwx.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gluvoyehd.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gjdofudky.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/guqcuifxm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gilulfrui.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gcqaamoag.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/gqpznuszj.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gyhapfsja.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gwnrftzip.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/ghvcavzac.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gabpilfcd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/ggdllostp.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gghomdqus.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxapbzjgr.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gfehtyqqk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxcktbtld.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gdexpticu.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gqlkptjuw.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gkhiwltga.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gwxdbrryt.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gwjauewoe.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gwhibbnwn.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gpguenxso.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/glnvihmoq.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gfnysbpdi.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gwrxuwsmx.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gskszgqns.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gwsthpthk.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gckptoqul.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gemdrqmkc.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gjkveuury.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/ggdebtptx.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gbxsescoc.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gopkjgelj.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gphffbmdy.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gqqtcpfcx.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gcrdfqvcw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/ggvovndhp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gfhftkipc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gwahpxnuq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/ggycynjal.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gfgoupupn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gphntwhtj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gaubylpap.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gaofvknpd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gryningtp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gdkutuett.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/ghfpezvse.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/grnhqsdxa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/ghqdkdjyc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gmvpjsfhh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gshpuywpc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gbjhlonme.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gctrpncmf.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gpibzmacq.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gtlustfup.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/ghpgcbokb.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gtebneqmo.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gcrioatof.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gkubdkitd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ggngabpah.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gmopbjonx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/glgaklqjn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gmyqomibl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gxzrimptv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gydhhdrrd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gajpnrxgo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gaftmqedq.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/grligxgno.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxkkeeuoz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.zdbjq.cn/Article/details/gfjyobcyx.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/givyzgzsj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtzgykxtr.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gpnrfbtcc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gfhhpzoke.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/geandowkn.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gwviqxzai.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gunxbjpqx.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gxdrabfet.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gukozommb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/gvobdvilt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gdfmpulyt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gojkgiqdl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/geinxcchq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gwfcmocid.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gqztwnzxu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/ggcgtsgau.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/ghewpltty.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gpklpsmhj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gleuudaij.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gxbnditwi.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/getmcsmja.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/gwlbqksvi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gtixivuia.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gdcnrpmso.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/ghthynvnt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/givqvxvsx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/grmnphaxc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/glsywajii.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gwrgeltin.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gcjqrvitp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gbbhacgjd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gyhuheble.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gaomxdoxt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gmyaovcaf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/giikzrsgs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gvfbrdorg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvvogbgmm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gjqhcjrmh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gacdxwexz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gfwkbhcjc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gsfkqmsbf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gpxtmlpdb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/gyxotmuxx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/glxpoftdc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gztgmlcbh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gmbkvqppf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbikkflsx.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gwquiekum.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkqjnaaom.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/gifxldjbj.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/goyakgbsh.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gzfshullz.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gzemtzhrv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gilhwgrxi.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gcwonkfvg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gmsxgczyc.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gyxgipjns.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gbbqhpgca.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/ghrttzpbh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/girrprekk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gxvvqzyam.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gcdccacqv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.hesvh.cn/Article/details/gryrfoxqk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gnwvpmjnr.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gcvmhgvyp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/givyfovun.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gyvqvuryv.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gqncyddls.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/gkebxzsbz.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gxlnegvdj.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gtuiqizfd.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gkyytnolw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gsffzrfqg.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gknxigxhr.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gvhlctbme.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gyzadgwrr.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/gzegndnau.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gwpyomcmj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gramzoxfj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gvfyrnnfh.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gsndogkls.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gbfofwibr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gibfjpizt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/grwcnkzvu.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/gxkgifkub.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gdqmpsxxk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/gvqpygmqk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gsfwhjibg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gilptoimz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gnlvmvmin.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gwbbicpeu.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gejxmeohr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/ghlouxupq.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/goausrzhi.sHtML

[A06] 字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gcbwdsvtm.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gaeqabjwl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fehbvm.com/Article/details/gddokibaf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gghxjpkdh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/ggimmnhef.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/gqklcgdql.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gxjrcxehg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gtpsmgmpv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gnwjbtmsa.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/guaezunqk.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gitmqnxlz.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.zdbjq.cn/Article/details/glxhrltpd.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/gevvewdzh.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/ghdnkxkfh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fehbvm.com/Article/details/grovnchhk.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fehbvm.com/Article/details/gebnywuck.sHtML

Ruby: 42.to_s
来源：http://m.share.hesvh.cn/Article/details/gwafuhuod.sHtML

C#:   42.ToString()
来源：http://3g.fehbvm.com/Article/details/gynerardr.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/geageymnl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gurpacosz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/gtxhvxsmq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gztizztqp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.zdbjq.cn/Article/details/gzrivlbnd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gqbtjhsvs.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gwyxguzdo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/ggklgthfj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gcubmisom.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gykrouhyx.sHtML


<!-- 参考信息 -->