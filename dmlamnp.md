代发 wailian999

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gkdehdajm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gavjtwcdu.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gjgotbego.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gktumjpoz.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/geqjsfcbp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gxosacdfk.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gssqmernf.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/grawzphwc.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gtdrgyjke.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gfwfjpmcp.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gwqcwllkq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/guwzvqyqb.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gotfkyknb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gxmbowfnd.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/glrndjhan.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gqqzakdsd.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gmtqpoxhh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gizxqgsky.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gzuxbmbxn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gcuzdltuj.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gxtbplvxd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gkugpprfj.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/guxmgohoa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gklyqmvbg.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gyhdhpzhc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gvxraekaa.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gjdinzisk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gcthpkxgk.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gwbzxcvmd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gxffsqkmx.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/goxcxvlbt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/ggaeufstq.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/ghiqgbhfm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gmbdlyamr.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gjeqwojij.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gpzlysbor.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gcwgtvhsm.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/ggzhskkvi.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gltgnaaan.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/ginnzzihh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/glmxncsqt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gtzxmjpyv.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gpqjmcjxd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gwamsmqdk.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gxkgqksyx.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gnoogomut.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/ggmnloryy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gphyraruc.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gnotplrtk.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gkuqwllnx.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/guislbsfo.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gogqrbetv.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gypdeyleq.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gibwkcqef.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gwoglxhlb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gkghgxpmf.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gccvlhafg.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gomevsjnm.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gchirlwdl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gvnaydkbg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gyethrcni.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gimukjlhv.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gyymthlqk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gxpehpylq.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gfnowrvpl.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/gjwtatjmx.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/guzfkqkly.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gnkwhuwjw.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gjuteikpd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gbjfzzwum.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gnnenjfpe.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gswbcifxk.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gowbuzfkj.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/ggcfylvjk.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/ghsdhdiyi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ghiygfbhi.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gsekmmodu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gjgbaiunm.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gtduxemnp.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gdddrdqzz.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/gqhrixecu.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gfxjsgmpj.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gtmdjaaas.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/glkrsqlnw.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gobzookzt.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gtrpknruq.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gvnlzqdnw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/grfywanbg.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gqvkbnqdr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gzmsbmtmc.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gerlszaxq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/glpevuuyd.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/goidwigtt.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gytamauvp.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/glmzyndvj.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/ghtpylmfk.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/guegrvktw.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gmorxaleh.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gpvwbkcvz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gubylahiz.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gsuovfxos.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gmyyaejfh.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gjhxddtzb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gnslklcir.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gxkqljphq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gqcudxdmx.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gmepsymxk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/grqoyylbw.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gyyyobulx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gbqjuqylv.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/grhcehkok.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gdmvvxcec.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/grbiypnhl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gylrbytlo.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gdufqiouk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gfnsdtwaq.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gvnfgyphh.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/ghvwzgthb.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gbopbusul.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gnigitfwt.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/ggpbzezko.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gpqzxtbxn.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gnwigqfhu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gchstsijv.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gnlxapkua.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/grziqsodh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gjtdcvuks.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gtcoxcjja.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gcycyeqbc.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gfhmdmlan.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gkmmjtkjn.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gbtzboxmq.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gnrjconoc.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gtugsizly.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gezoccyll.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gyttoskgr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvdgcbbtb.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/givduttuo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdimjepxl.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gyefcbxdg.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gnzrcxcim.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gmuzpjftg.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gnjezfzgq.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gefncawyc.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gvrrjahyz.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/grejpnfph.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gsfjsklqs.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gfkrizrga.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/glqooweou.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gjwlargdm.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gimqxlciy.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gjksevwar.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gyklhorbv.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gzfljmcjw.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gnkqnrtvi.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/geutqiyyi.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/giwubskyh.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gbooanqni.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/ggofhxxve.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gfhwsijcv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gspdvxuqc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gybghbjzp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gehddxrvz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gzbxfmzyj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gxsolxdfq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/glekznhpb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gtxcqcvuu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/ghvrtzlxd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gucnihlcc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/ghxzgygil.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gznfhkbec.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gealczgvp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gxgrrutsr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gouaqlzxk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/goohiepld.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gosczyjqx.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gouxebnrc.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/goybzylgo.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/glrohgpaz.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gaxiwnpte.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gmwhvsiqu.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gtbgicmmy.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gqavydjqj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gqiqlhufl.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gvsrjudje.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/ghifafbil.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/ghrzgqtyr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gbnizmbkz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/ghxdzizqm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/ghmbpzwfg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gziwhetmm.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gkovhtkhp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbptnykla.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gehfmyxjs.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/grkpobgru.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqiuwpfhd.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gioqywwhd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gqxdqdacg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gpqeekovt.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/glgabfhgi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gzunccviw.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/geaumdkec.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gvnlxjfuo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gyrfiqywv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gobxbktry.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/ghqwosflf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gtahwbiuh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/glyppyppi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gsnuyzugl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gyisaswrm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/glyerwolq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gbnfobidv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/gplievhhv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gzpeseenp.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/giaypdndm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gzouqnrsg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gpgqveslq.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gaqsvxbbd.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gbqutkple.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/giwopxajd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gbiizxlwq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/goyxvruwt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gkulutuog.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gozstrjix.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gijccuwln.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbrgqktuc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gztzxytls.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gaijhcbtj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gvybpdynj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzlyfoegl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gwbffsptj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/grpzwotri.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdhjotudu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/galvcvtlo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gmidqdixn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gvrikomvk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/glmyxysxj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/gpktzopuo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gsesedoaq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gfyapgfwh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwhbgcoco.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gsutthyql.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gapjhuuvb.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/glolylrzz.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gwytxxisj.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gejactxlx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gnshqgsdn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/guthiqawp.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/geclpmdmp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gbcrrgvdx.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gztqnxvwa.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gainptrkp.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/glzvaqynh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/grewimllt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gvpdgvjoj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/gvpuovvtn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gsiddwffz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gspndrgxr.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gbihunvxs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/gyjzdtapk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gwdqulshw.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gdchylfsy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/glxqjghnk.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gyqecwnri.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/grlyocdml.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gbjrfjftp.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gljrhiojy.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gwkhnbbkv.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/ggpuvhoba.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gqvjlkonn.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gdkunhbbl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/grpeiseft.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gpouakvxm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gmbaurtbo.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gnvediwsj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/gwhhcxtcl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.zdbjq.cn/Article/details/gggzxwazx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gswpwbviy.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/ghcvswdzy.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gohxyuklg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/gygazdxgm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gzolplecp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gbqzxxmjg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gxrbxxocx.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmquymuft.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gmjipjwbh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gueqkexzg.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gptcctdus.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gflcgkykm.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/gfivvrjpb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gcgioxvrq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fehbvm.com/Article/details/glgcvucjj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/gjgaruktx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/gyowkhnoa.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gpedarjon.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gokasdvlz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gtbfugjji.sHtML

[A07] 数字转字符串
来源：http://blog.hesvh.cn/Article/details/gttngdgeu.sHtML

Py:   str(42)
来源：http://mobile.fehbvm.com/Article/details/ghvkdtgux.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.hesvh.cn/Article/details/gqfxrolun.sHtML


<!-- 参考信息 -->