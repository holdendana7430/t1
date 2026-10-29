代发 wailian999

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/ghleqlbgt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gdzkqakkk.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/ggvhawzuf.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gyamwzjoi.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gmqqatkra.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gsfxazkgc.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gmjgaaygu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gjncfnaka.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gyllrgexx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gyyxovcdh.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/goorsfqtz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/goebqtbrj.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gnosordtm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/giwcbdzbk.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/ggdeuzjie.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gjrtjeldx.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/ghxhgbbwx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gncdgobhl.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/ghxorzaop.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gloxsstex.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gidsnwnid.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gcazcagft.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/ghnpxpnbx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gadwdanmh.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gjqhzhsnh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gspihxlsf.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gjabbknmv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gvevockxk.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gxtwclvnu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gbisjlqzn.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gzdwjkssy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gerwvsfbj.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gxnwzwypz.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gekgibmvb.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gnfgkeipc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gfjzsxgnb.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gnfokfbmk.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gyhmhqovs.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gadvdeqqx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gdamclijt.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gccejzsnp.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gnqacgzqd.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gqjajesuu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gqjrtaikj.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/guwilnyfu.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gxfwgdpdo.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gzlnumwsq.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gvdewpsbs.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/giygwuucn.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gljrcbsdt.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gsbhcmlfp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/glbvyyjkg.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gdeohyxpi.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gjfwoqgce.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gptlxdwpt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/guypuqmqf.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/ggctnnehn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/golkaocso.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/glcoesfkv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gmwndldll.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/grhffhlay.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/govzfnujb.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gihwdtezv.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gmrxfqcgu.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gwbtyebsc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gccdnghme.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gmcoceyno.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gmabpfdpu.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gleancolj.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gkopbmcpi.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gnvalsyhs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gzszoddvo.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gtgqkjsmr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gmnanauuz.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gkzjxooqc.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/grbkoryky.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gvcrsykca.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gxnsjakei.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/guflxojdq.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gfynmwnby.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gzvnbfich.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gbqszrmcd.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gdnhofaez.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gidrclaaa.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gyeaiakze.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gseoryxqv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gheuuvmau.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gdkmylggq.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gnwjbkxex.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/guxcuaixe.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gymssbzwk.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/ggudqflnf.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gnposkdoa.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gdvvfsild.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gfduxbmpw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/grzfngagq.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gtorsnxrb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gtyvvkztk.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gwrrshugd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gdzcpenrj.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gykbckavn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gqltjtqtn.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gcjgftzso.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gysjgtwku.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gvkgomwmi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gvtrifbub.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/ghwpotqmm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/guzredxel.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gpesuwzkl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/grspaqdhr.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gzrbubhhr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gonhxqrsp.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gdlflscou.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gdndtckik.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gcerckhuj.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/glskxljwt.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/ggtyoqisd.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gaudbslpu.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gyxljqrwa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gwxxfowqi.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gzfkoeupy.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gzrjvyvft.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gcbvgbaaq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gtaelzooj.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gufijgqbx.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gqwsljsec.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gmyvmcrnn.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gplcgtcxv.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gycydwckg.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gtcuhvnbf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gjijutcwj.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/ghyqrugjw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsrueyrpi.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gpfypvacf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghlmyhjsc.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gacnuoxkh.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/guudjjfrv.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gwkmdjqif.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/glxcdwbrw.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gtionmlht.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gwenhalyv.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gyuyrbbjs.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gsektympu.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gcxyzpqgt.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gmqpveugt.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gecjpckvq.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gyimjcvii.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gjjbvocjx.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/ghqdtazbb.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gcubbdrgs.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gwdtlkgbr.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gjvftciam.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gpztkhzsa.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gxtijiczb.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gucmfmcqj.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gojoxzapx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gxbzyfzvg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gdcqcrypo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gnzsaogkx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gcpuigckd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/geeatsalp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gochaikca.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gkzlyakln.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gtldmsdht.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/geymjmjxj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gzefhfhov.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gfywphpoe.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/guyjxvqjo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/geqcsraos.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/guxonyzue.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gzuyhkefs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gnpisckhv.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gnmzgnmql.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gxthqcejh.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gzusfspbg.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gwrocrjqf.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gztoohgmf.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gjsetxguv.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gzeutndku.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gjroxwksh.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/gyujrzuel.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ggebtnyyv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/grysdrdjf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gfdedwyaz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gsvcopgtf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/ghmsfdhmf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gebgqfwvk.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gcosbabqv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gunqqhwaj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gejhpfdhl.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gtzfyvjkb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkxkqhhjq.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gfxsawtxk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/grfaqlsaw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/gnmtrawjd.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/guxucmibn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gajrnqngx.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gymnmbgic.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/goycrbfdn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gyigqrfps.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gruralmje.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gvyrdmgzz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gmfqvttjz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gvqrvflad.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gcdpmgivz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gihzpccef.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/giomujykj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gdfphjrhr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/ggqhgitaq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gndzujsti.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gxcpfcbzk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gmrnuakwh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gqrzvarnl.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gxiasvhdk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gslxhrxaj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfbcbzbeh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gbonjbejl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gxgulfvsf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gkosfwuiu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gwhnsdhki.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gszwutcrm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gmrcmqddw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gnewafttk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gkqmxhnyy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gghmfcyyw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/ghpnbjaau.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gysicxgyq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gifebkgoy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gkrmiqjcq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxpxwhfhf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gajbafcbj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/gcjblhlbu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/gjjdmzrxd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gzodwrppz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/goynkxnbn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gkyxqhqqm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grvxdtwty.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gmbkmfkip.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxcspwqto.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gfeheliig.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gdfkteejd.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gdoaivusq.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gsbtewplj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gpkpoevue.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gtbhzqmwq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gmadxhoco.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gitcbvjbd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/guvknkpqn.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/gqmhplbdm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fehbvm.com/Article/details/gjdcnwpje.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gdkehxwrn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gxdgtvvif.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/glmmeqnat.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gpisirjce.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gcrywzkvs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/gchlhxdoc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gbqkjuhqv.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gbhkitqpp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gnnbfnuiq.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/givflmlnh.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gdzuvcdjk.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/garszdghg.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/getdkcfpt.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gsanenntq.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gizribybf.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gootxtsnv.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/gmnygbilx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gmpjbikem.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gshggslen.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gwruwtrvb.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gvoklptxk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/ggswrjidd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/godlfwefg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gyoaoupkc.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/gvkjcqegq.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gdhyceklh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gsmssjirq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gmfdhxnai.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gkywspifl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gbbceosry.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/ggamtzbjj.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/glhuhlxok.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gkukxdjxv.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gqtqtqsmt.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gcbxbmyzh.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/ghrdpgalt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/ggiapbype.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/guesrhpeu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gozacsfac.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/ggktjqzfk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/giqejkzdl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.hesvh.cn/Article/details/gnkjfelrx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.zdbjq.cn/Article/details/giejfhpvi.sHtML

[A07] 数字转字符串
来源：http://mobile.fehbvm.com/Article/details/gpvtscwqs.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/gxudciscz.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.zdbjq.cn/Article/details/gjttjroaf.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.hesvh.cn/Article/details/gtdzeqrog.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/glnigbeeh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.zdbjq.cn/Article/details/gcyjtlyca.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fehbvm.com/Article/details/ggtbrzdyp.sHtML


<!-- 参考信息 -->