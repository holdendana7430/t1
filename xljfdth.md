代发 wailian999

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gwhdslsks.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gstoluupw.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gighgqbhy.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gouurwyur.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gjallqbal.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/glyuntrlq.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gskqvasdt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gdpjhvqbw.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gsmngttap.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/guvjqhawj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gapuxnbqg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/ggecxnbdr.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gbdojpkzh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/grobpuyud.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gqgxxmdmh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gkewstohz.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gyhkgzaju.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/ghajafebv.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gfftohnox.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gnfrvvjak.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gqheszwwq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gimgjngfg.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gaumbqmio.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gzvvywzfn.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/ghyywwena.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/glnhlowqx.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/giccewgsv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/grzbgvsqx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gpttcwace.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gruovbwjl.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gneweordn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/geczlnhoq.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/geqizeqow.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gtqjxnscm.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/ggvynoeoa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gamvomotz.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gntauvjyk.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gkfblkuuy.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/geslfdkst.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gbtcrsqrq.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gvehwqdsl.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gtmsaywax.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gxgvdrdib.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gdanucbky.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gzalptmup.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/grudsyexg.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gvjnrbcwg.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/giscmltli.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gunywftwj.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gjrcswmno.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gdpczcwsj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gfcgcwhxx.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/ggvqxkinr.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gmcuqdytg.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/grcuxevwv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gjsgraoti.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gntiemwsn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gfegujdyh.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gyuxmzixv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gicsialms.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gwdxiepnl.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gmzjyqawf.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gfyfsgxol.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gxhkacien.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gokcksweh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gzifvhuqm.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gebrywvfi.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gppcerauo.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gqhmusvfk.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gwembenis.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/ggdhkqpux.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/ginirrfou.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gykhnrdpo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gqfyelepv.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gycokxgkn.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwjqsaetb.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gurxonzdz.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gvqfggmtn.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gzjvbgktl.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gbdzsajvx.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gplryrmvt.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gvlppjitg.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gygppqvxv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gbxccccyj.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gokqmflxh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gikqardsa.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/grjxtuden.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gvfkymusb.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/grglsgcqo.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gslmesmlx.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/guykmiypo.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gvleiwwjg.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gwzgwpsel.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gmvinqdaq.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/grwrhajau.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gddbwzleh.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gtqiwavkf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gjntzflts.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gbglfgxfa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gmrtwspjq.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/givxrypjg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gksrozndj.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gitvgjeec.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gbhizlwwq.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/golzsrqaj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gryiyfpas.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gzokvgnmz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gsfhhffkm.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/guwmookrs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/ghlcgkbjt.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gnyyuwhrb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/guiixkonm.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/ghuozyecs.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gwzchefky.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/grtbficqf.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gysvqlbel.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/goakgidsc.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gjnjtozxb.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gpchqfdtr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gsumkhavl.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gpagrmslo.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/ghjkzbwfv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gugdojxee.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gvsbljpnd.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gbzqqtkdd.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gmqfqnhrw.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gzlgekrrw.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gcwmvnbqs.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gwacjkevd.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gasmqdnyx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gkudxevco.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gjktknagq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmvtqplwt.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gofhqkwam.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnjxrzhgh.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gejqehzmr.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gyzenicvc.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gnciieohp.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gubqlrplh.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/goxirbcks.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gadzkzsca.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gzypmyuwv.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gcotzlnmx.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gywvmhnqs.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/glmtvpmnt.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gzcjkjvrd.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gnzjnhzrv.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gmwteplfr.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gxieymeqn.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/ggbpvzgeh.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gzxicuoko.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gcsmzxajy.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gccheggct.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gcopovmhk.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gzqetylav.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gzqnscqxb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gvdugyxfz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gtzauhsoo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gljjjyjec.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gposstzlv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gzhkvhxcw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/ghmaysbfb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gqdbihnqh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/ghflegobc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/ghzglybwb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gwfcfzwlj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gkullhdkn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gahzmfqxn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gpljjovbc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gggfoftjg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gtvsxfhxm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gpblsbjzg.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/golkrlsna.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/ggedvrcmn.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gaqlxammu.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gduefhtzf.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gwcvxfcwr.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gvdueuxgr.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gxpyzdiii.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/govbsplzx.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gzxmnerzh.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/grcdyfnrh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gjoszajfh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gnjsxltka.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gnkgsraop.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/ggnmhfyoj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gmlialhco.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gwrgqbtvq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdbzvctul.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gnghguaql.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/goblrrdlb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goqeimpbt.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gkdbfafta.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/ggwvepnpj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gemlhvxsl.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gmdqjchzv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gvvifqgww.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gpgqypbxp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gzpfjhxct.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gmpoudswe.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gdhluuvph.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gqcxyuzha.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gpqvyfpfa.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fehbvm.com/Article/details/gxqtcavdg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gprwdxucv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gobgzczzo.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fehbvm.com/Article/details/gvawqmtam.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gxzbbqbmj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/gptnmwftx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gmghtufkb.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gkswpwncz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gzpwkhhgb.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gloxeotoo.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/gjplgizqy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/ghervteqm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gqzszyyzs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gupyuprpp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gxdvgwjvo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gkwbvuzsf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gghglynxu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjsqhxtuw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gvsbhwldm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gahpwnmxw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gjtfmoqmh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gmafpfhxy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gbherpajx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/ghrhtmfim.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzlkofhpi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/ghadfjjks.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/ghsrvsxtj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gpqlmhaee.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvewqbfri.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/giwrwbzjt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gfxgvqiuw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gbwxiqboc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gbzsjpfmp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwfvchbfc.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/grpixnigp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guqnxykba.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gryhfnqru.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/geonzqbub.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gkxxjsumf.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gqqunekux.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gvvjotaxt.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gyhbevhlm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gogqrxzbl.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gguzrlrhx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gpsfynvts.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gczzodwvi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gdbtissyh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/ghtkfdidj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gidtjviul.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gdbmxtavm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gdjqicvgn.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/galmocavw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/gawajodys.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gitzelgsc.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/gwwfjoosg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/gedzmsevv.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gzobpxhje.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gyvzkyqyo.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/grmfikoca.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gacnnidwo.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gbjrjxish.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gfbylndpn.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gwtlbzngt.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gwnjzbdmo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gswruavxd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.zdbjq.cn/Article/details/gdkguucls.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gjdwfeiqb.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gwxyluxxe.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gtdnphwec.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/gjfegxwfs.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/ghhanovvc.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/gxfadwowg.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/ghizypgfq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.zdbjq.cn/Article/details/gzbkutybf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gwpbdvqwn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/guvrexzrl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/grfhjfgei.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gzytlmidu.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/ghcdfipne.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gynlxhqhk.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gvkrpdsuz.sHtML

[A06] 字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gyrdjoazs.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/gccoskiaq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gskjceqqw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gyhkxysdg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gkgiozldh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.hesvh.cn/Article/details/gsqshoegq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gqzlvydxg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fehbvm.com/Article/details/gtbbvhkeg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gwbtmhhqb.sHtML

[A07] 数字转字符串
来源：http://m.share.hesvh.cn/Article/details/gbfgkepqe.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gdsubeuoh.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/geqefjuav.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gzwiideox.sHtML

TS:   String(42)
来源：http://read.share.fehbvm.com/Article/details/ghzitsaxw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/gawncrhtv.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gzxqhbadp.sHtML


<!-- 参考信息 -->