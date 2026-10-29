代发 wailian999

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gbcpwlfiy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/giunopvjs.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gewjcrpvu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gswgaykad.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/ghssdabde.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gzhfoarce.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/ghcgnppco.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/ghznsskch.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gwaqatwwt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gzrrsqkrg.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gswmdouan.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gjhhfjjac.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gyvcchdwe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/ghonupkxy.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/giuesduuz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gguepfora.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/ggthyinnc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gpfvtevva.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gvzsswbgm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gfkxqeaiy.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gvpbeulmv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gaxipwybm.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gexzxomhm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gyrecteoz.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/ggynwsobg.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gjytcbgtw.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/goddrbdzg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/grscpafvo.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gkrokekzj.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gfrnayrgk.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gpouwlgcr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gfovpamsf.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gpritihff.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/guraibbme.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gtlsqsfrf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gwzogwtnf.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gyudurrin.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gcqminwgl.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/ggvybnjco.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/glfirfcar.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gwpmqqpns.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gmkhbdjks.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gbrbzinrt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gakxtkpcp.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gptofjuzt.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gnjcmlwhq.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gtewlaeff.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/graqejmbz.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gwiimwhcm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gmgtzgipo.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/ghqcnxtyv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gdpvhrsdc.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gnayirwzb.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gibumiksx.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/giflowljv.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gvcgdjyaz.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gkyrphoub.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gpzrdsavs.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/glqujjian.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/ghfgyhvtj.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gvuclvqxz.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gbrirmwcq.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gsoqiapbm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gbivoguyf.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gblpyavmx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gwiitmixb.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gjmbvxmbh.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gveorepam.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gxkbvbwlr.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gbzsmudxr.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gyarlmnsw.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gqgdvbpmv.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gqmvqsksr.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gljqmbsyb.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/girzdzcoz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gsyefubra.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gitwowdrs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gspefvjkc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gmmalbmsv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/giqbpslej.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gmujzufcl.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gvlpweqvf.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/ghswellvs.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gjaerqulq.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gwvrgzocb.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/ghjwugjbo.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gotodszjt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gquumqgyt.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/ghelcpxcx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/ghnucpcgo.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gmpogvjty.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gjjkbwqxx.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gsqhfmceq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gwxtfkxxf.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gmjmmuztw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gawnvvlkb.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gvefjxoee.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gocaetqle.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gatysvtif.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gbciyvzqp.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gtbddzqqc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gejyliirk.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/getvkzztn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gzhnbiyjf.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gixjpihmz.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gmlmmviqj.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/grgaxjdnq.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gtvbkbcpg.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gugtuenek.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcuwgfqht.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/grxamcgne.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gjzmtpinl.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gvebfufui.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/guekuxuyj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gszigptjp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gechuzmww.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gcujttava.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/grxqptxwu.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gdfzgfvlt.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/glcynsjag.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gbeutsvlc.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gaduecjto.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gbifebuej.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gbalktuff.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtdcqmhcg.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gxnfgjjpz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdbkoleag.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gtwtfseme.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gpcodtflp.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gtlvpezcd.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gutgpenrf.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gsnuculvl.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/grzkxhnfx.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gehidqtif.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gmuygfcsm.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gjafnulbv.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gikozqhcz.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/goncvlpod.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gjaudkjot.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gvoviluhz.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gcyijprcs.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/grgpcjgwa.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gtwfprplh.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gynqzuwlj.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gsukvunkb.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gfezppfjj.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/ghncvimvi.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gcibpghad.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/ginsiyezb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gpqtxojyn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gdkavjeyv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gookyeqgp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gzrsvsxkh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gstfhleec.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gwjpvxygo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gweznblya.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/ghaccqolq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gstfxofnm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gadbgbniz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/ggowffsds.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gtfvajvwi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gckgdkasd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gsdxwogaf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gpbzniekk.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gofamsylz.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gvvzstyvy.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gbpwuyzoj.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/grtmggfjt.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gznatdcbu.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/genjgagxx.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gpyhisxsu.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gqpklsjfz.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gimiqxgib.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gcavyklxn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gqiykbdes.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gembzjyxz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gurkcznjp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gbrpjdpyi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gdkffdmku.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gakcwdykc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grokdtghh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gqmryoiwu.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gzfzrbxox.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfsrkchcx.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gadsdyqop.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/goesddzba.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/gpgwkhfuh.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gibxpgoyt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gblqmahmi.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gxrrixnfk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gdaulcwdj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gpxmmkdop.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gqzuengdf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gqyzyzeyq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/glcohzfta.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gsiabnxlw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/gvrfhpsit.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/ghustevqr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gqbdbpkvt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gxvhtpbsd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gbpiruazs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/goetmhoxu.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gmyobkpsu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/gokqwsqod.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gpiowgocj.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gqwhgyrip.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gglzykxmi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gzeyfngtc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gtyciedhd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/ghdetzfuk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/ggxcwhmtd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/gpfxbugus.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/ggtnoewut.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/glbanjohx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gmzawvshx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gpkrhdbxw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gqsczjxfo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gzsbotwlj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gednslyrs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gotkuectc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gepirhymu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/glrfdgllr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/ghwvlkgjl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gfwsvxbgs.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gchfavpyd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/ggmzaueuu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gvekigrqv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/ggiqyrmpa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyyfpdqxv.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gjjfxjhoc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkjnvtxtr.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/guqmvagmr.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gvmimqtkk.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gvzctjyek.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/grudxlkmy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gyczmvsld.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gihwplphq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gcrsvbzrs.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gyweamjix.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gwcqgbzzn.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/gakmacqjc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/gxhfhfkvm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gnfvjbaba.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/glorjkdst.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gzfgurieb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gkwrpcdml.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gkucfmfcg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/gunjwzvxx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gccprhria.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gqszeqjed.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gbslfelsn.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gtzanknem.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/grsdcrlxh.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gybhkhqwq.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gxyqdyksc.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/glxezfwut.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gprcojlsa.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gpzjnaahi.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gwuuubzth.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gsljjgyyz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gnzadidgb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gmunwzpzi.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gpnzoowft.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/guvjqhfby.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/gqdaqoxog.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/goedjbdzc.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gunfduhxe.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/geawjtibh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gnzpzudwr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/geimgyqqv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gwutyenfl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gpnvzjhdh.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gujhvhvfd.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gafbqdvcm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gpjwfchct.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gnkdrbxtz.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gfcodzrtt.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/gmkebzhgm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gowvqnwny.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/gsxefvnpj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/gabodkvqj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gpsawdmli.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gtmsotlmy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gkxcnklop.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gsjvonnsa.sHtML

[A07] 数字转字符串
来源：http://blog.hesvh.cn/Article/details/gyhkduobx.sHtML

Py:   str(42)
来源：http://mobile.fehbvm.com/Article/details/gdainuuqs.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.hesvh.cn/Article/details/gyxrpmvqo.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gqvnnonku.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/gykvjmcea.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.hesvh.cn/Article/details/gnkslviwb.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gmljcdpxu.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/ggckioegc.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/gvcqebjvc.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.hesvh.cn/Article/details/gbebdptyo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gbrkdaosq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fehbvm.com/Article/details/gkgicxyqq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/garwztfzb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/gqtfpuaut.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gydvyngnc.sHtML


<!-- 参考信息 -->