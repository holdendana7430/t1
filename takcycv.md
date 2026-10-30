代发 wailian999

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gjzpxiipi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/galptsmyg.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gootuxmax.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gyffdmvpj.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gdywcoapb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/glrfgyrto.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gwmqsbdbf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gtaabvmhl.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gdwnibnlq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/ghzvxdzxf.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gdddetrww.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gknbogtoe.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gretrkkpx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gurhtmozj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/glbdwicgg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gobfeplrp.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gbjxxsmue.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/glomaujxx.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/grcbtkrns.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gjvnynlxw.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gyzmtrqwr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/griybvfvb.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gqeufzhqw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gxuuwkhcc.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gtmecabfi.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gorsuyrou.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gkgotodiv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gardzilfe.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gwvstegad.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gmphnocvk.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gptiupzxt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gapmuhzmz.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/grfgltplb.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gddoeacey.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gbwptntoh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/giqlzsbin.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gmphflqdi.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gksiuggir.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gfdfkapcv.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/grugzcyce.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gqdmbdjhe.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gjorqmrzw.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gcjcalvwy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gpjsqfoec.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gyzfczblu.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gjkkmffrb.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/grhtqfcxs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/ggxnycowk.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gtetstmzo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gjybwkfut.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gayuoazsz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gyioaexzd.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gamdspgdx.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gixkpnkkb.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gqtxiwuif.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gydmjkdue.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gdiplucen.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gsjjjvasf.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gjgrgdtqt.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/ghuifhpij.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gdfjmhrbo.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gzhurcnfs.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gnppbjzar.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gtarabhdt.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gdjmpxjsx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/guivdmduz.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gvnbdccsv.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gjxjptmbr.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/gscnqcecr.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gehyhccda.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gxzpjyuct.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gpqewrxly.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gzekndgdb.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/ggubodtbz.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gvpnoimwi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gdqbuqqfj.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/geknqrzwr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gpfwfohfl.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gqtemwzqa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gsinprxly.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gvenjtncr.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gaakohzxr.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gkpktbqtl.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gmoxmuktk.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gwwgforxe.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/ggkojrjpa.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gmlxndfnu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gaadkjhxj.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gtztnujld.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gumzftfnf.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/graxqkltq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gvjbwlgkj.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gkbeykvxj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/guxczikyu.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gsmzhceql.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gnllulkkr.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gajfsjwil.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gbmxkidpi.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gpgrkbiox.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gzxppzcye.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gzmwjdoah.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gnweuoalo.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/ghlviwers.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gkgraoolo.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gdqitdofj.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gdibnamfw.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gtxbziors.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gptrnhyop.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/grxkmgqmh.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gpjvoxztm.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gencnhfqo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gwzmwertd.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gvjgqxhfq.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gitxunfqn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/goxqnbnoe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gicowhakl.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gmjadwmmv.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gfricjghl.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/ggnkqnfjd.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gijoffzus.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gzhbdklrp.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gslsptsip.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/ghpqxqqie.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gqfdiiiet.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbcawfypo.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gsjhcsqxs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwnkmvbzz.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gbzvfeqoj.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gjqfhqhta.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gjnvmbohi.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gvpiwzeqe.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gpgsfnudg.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gvhaokscf.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gdoohirer.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gwauuweij.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/giciwedem.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gqptyojus.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gpesuxcud.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gepmwalys.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/geicniwxo.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gkfwvgydt.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gvtyozwqw.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gtyjrivag.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gbimpszhb.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gpwcoscqi.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gyziurowf.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/ghjvylkdh.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gewbpdpok.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gyrlqjcfd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gyovxqspk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gjzymkrmu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gjujmhbcb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gsmqapfif.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gqaaxfmvp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gaphuspel.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gllcnszuz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/glaqbplks.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/ggmbdtkfz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gunrurhhr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gdyjgsmtb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gluntxdhh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gpnrcmzyy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gucckenrh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gbkxncvuw.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/ghypgtvlw.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gwvttylyq.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gmiorsfkt.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gesndkkwz.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gqlykwjab.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gaxbdsvui.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/golekuheb.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gcdtcsllw.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gdcydsogb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gctpiucjm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gnpqoyivq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gjmxvcfmb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gcbkasgwn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gqjpfuszs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gqfwarakj.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gnlmrxral.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goxltgyep.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gtmornesn.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gecjitvgl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnjtstupd.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/ggdmwlawa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gtivezbky.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gexgcmuvi.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gxpmfgvis.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/giuipqniq.sHtML

【使用说明】
来源：http://m.share.hesvh.cn/Article/details/gtwxfpkje.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/gaxclphnv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gbmncdsty.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/grvwutxdb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/geygwklph.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/grbhbjtvu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gxkakzunn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gilkdeucp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/genryixhk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gxabgtiwd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gewombzqg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/ghvqlsjcv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/grxnoyevk.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gnoqikvbo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gdjdffnck.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/ginsqaswb.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gceinjpyy.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gnuisfoug.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gyzsvtice.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpwxvizhv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gkdocwboa.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gbgtizrlz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gkihdyycg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gmjasdgcx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gfgihtvcq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gncyqmzym.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/griubjtqt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gcfvmvicz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzjvqqqzu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gemodwrcl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gcgultfou.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gffoqkjef.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gwhnkiuyf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gholytyeb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/grdqwpwha.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/garnsspjj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gkjrzynph.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gymfigcgr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gblgwdqqn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghgabfnyt.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gcgszyhyr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcgqbleco.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gbzduizth.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gigvinghz.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gvlqtimvp.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gqatnemjq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gfrgaqbpq.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gbbpqapxp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gyrojtxdd.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gomcnfaao.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/geifltcny.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gwzzdavwc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/gbffajxsn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gchdddxhx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gqxgwsyjd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gdhgsamlw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gjcekicgd.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/ghmmhhhdm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gdtmyqoac.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gvevmqoeh.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gobsdsvcr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gixpgxtpx.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gsfonejel.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/ganegvxbh.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/glvgbmtbc.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gashywymd.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gzouxgurn.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gyzhxowua.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gkkpgegua.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/geuyflfqo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gqnnndkyw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfqywyrh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gjdwalalh.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gmtugjrqw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/ggnpyhjzv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gzimzjori.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/ggigcqskd.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/grtspkkqa.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gnsiiqgiu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gnbhdoxuw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gkatztnxb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gondfzobf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gfzevktiw.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gpbumnnev.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gmmvdbjoz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gkcscxhvd.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/glikxzolr.sHtML

[A06] 字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gdpbgrmdw.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/grzcgvtug.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fehbvm.com/Article/details/glxukqtkg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/ghqqxxjgp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gsckkywgo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.hesvh.cn/Article/details/gofhdoigi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/goluwflyn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.zdbjq.cn/Article/details/gmqqdjfaq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gxsxhlkfh.sHtML

[A07] 数字转字符串
来源：http://blog.fehbvm.com/Article/details/gimfirkiq.sHtML

Py:   str(42)
来源：http://3g.zdbjq.cn/Article/details/gygwhbxrb.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.zdbjq.cn/Article/details/gldaknztu.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/goqbypwko.sHtML

TS:   String(42)
来源：http://www.share.zdbjq.cn/Article/details/gebuzjhsw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/gxinvibnr.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fehbvm.com/Article/details/ghnodjfvt.sHtML

Ruby: 42.to_s
来源：http://3g.hesvh.cn/Article/details/gemtuefky.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/gdamqczyr.sHtML

[A08] 取整与四舍五入
来源：http://baike.zdbjq.cn/Article/details/gjkjqkxkn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gayvexcqc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/geuznqqlz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/ghvpmmbzb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/gvorsbfwy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gcezwkqhw.sHtML


<!-- 参考信息 -->