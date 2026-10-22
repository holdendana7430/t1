代发 wailian999

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2bahcmsld.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2edjnexse.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xtkxwhos.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2adydbzrp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cbgwftrf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2lpjouyyt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2oetluqno.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ygtlwnxk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2awgqrdsb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wvtefugb.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ckfowlyz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2oeiesfds.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ichoebnk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2oktvpqwr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2nqegwipw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2bwykiaod.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2xzoxddsr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2tfrkgipf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2nxtimsgs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2muxflwkm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2awjctzzs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2anurwerq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2korstnnb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2mzzhpmoe.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2uonhrduo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2reoxeigl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2fcfymvkg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2qvopnioo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2vpwhvrea.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2jbjyxgof.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2phcccgal.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2udckenez.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xpivxudu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rucwlcec.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2dizhaxje.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ymfxqgvc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2nmtapcge.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2koyqksyl.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2spnapwqz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2nrotphsx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ovuzudzc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2twiylokq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2bohwnijs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2mwdjvqfa.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2jhcyrvfn.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2vdoqxkul.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hrqohvfs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2bvrcewrl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2yuhkqhnm.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2xdmxrjbq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2upsrmkdp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2tacwovzu.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2gvlswign.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2wfygvolb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xymxigwk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2dxtytzqe.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hklfyfze.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gpexusqw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2uwkypbbz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2dzoxefng.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2supvtyfy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2dqegdwpb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ucysaols.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2guxzawef.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pokdywqz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2xsnoqylk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ynddeutv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2qffgmkce.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2uofnclmq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vglwflwf.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2fiecflzd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2daxnsndq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2osjpucuw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jxopdpqw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cahfriyz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nhskheks.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2drmovahj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2mgwrjgqk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2aoyvntcn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uplubteq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2xpjrzybi.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2zetbyuzf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2qrzgftcv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rputkige.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2qijqwngu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2neymxydb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wajkufge.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2jlnbnvim.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ocgmdzhv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2vfqsszxg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2pqkmsgzl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2gcgpujoj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2dqgketzw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2zcszitue.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2xazibykl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qwctoiia.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2vsgggoij.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2tpsdbzxa.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2credlhfw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zdlwtqhc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ihktxfdb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2lsozvlfp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zcdzzscx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ffrsajkm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nxxczovq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nimbzsfr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2igzvtqvx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2vufeauxq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2bpbziobx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2avmratuy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2jspwznok.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qzfivioc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zypacofx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ntbdzysv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2pdlicwwp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qixkxzun.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2osplatyr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ywgblctx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2axfvlbxm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gmallctx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hervjvnt.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xljezxxq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2qfnhtsvc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2etldrriy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2bhmlxrbl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2kvqzrxhk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2phxitual.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2vlvbskqj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2koynwuqz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ubzwjmnm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2dwkjzrri.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2emrwlgtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahatdzit.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2bdfkkysn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgijogqq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ibbquqxy.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2etopblas.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2urbsvcat.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2gsvpfeqi.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2kjyieswg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zxqltrxy.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mcsoxiaj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2odlqrqjr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2yggexsxi.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2xzvxwrns.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2mmbzkrrv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2orpqyixu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2qzquptzx.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kpimfxfb.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2coqqphbq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2wfpfznig.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dunolhfn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2aeshavqu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tqnycgnz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2adioirto.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ezyupehy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2txwhurpc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2aqgkpxbw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vmdineyi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2rypgzntk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2sthwmweg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2iijonfij.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vilempfz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qvskasye.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fmmenvij.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2vylqsczo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nuqwfejp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cxbvjolq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dhyaxsvd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2yhqgrxhv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2gstcyqic.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kcimguuk.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2weybfswh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2qhskmvrq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2bdervcso.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ctngmjoa.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2bqtlpkvw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ytdanrqx.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nxxausxf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qaueebrs.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2zljjibcw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tkwcvuqv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2qjoyvnsu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2gbxjlvrz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2zynriwtj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2kbsweufb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2qacjraek.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2scmowvyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aykiombd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2fezbjbzb.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2umcbonae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfrwulmf.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2eanyedmh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2azgpsjsx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2hupvkake.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2fcxnpgvy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2wqndoxmp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2bpoenuoa.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2sbryukyw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2uggyngve.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ptkegokq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2uoptmybr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2nuquxyfy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2frpcypyw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2jjeksjat.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2mfutzlkm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2mhwvtrtr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2rzutvvck.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ymyymrvf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2jnsznybq.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2sindyavk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2temguqzd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dmqrkfuw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2wofbpsuy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ooqejinc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2dvmtbvhd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bclzmkfx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nhfdzlxk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vhcinvrg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2rhomtwre.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2mvznjrsv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cclajxfs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2vtymhcdo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cxwxqayz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zmcdfvhz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vwwkpqca.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gjuzpfzf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rkfohfxj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ivrdfbvn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wvsbamwt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gebjhbry.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ptohhowc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oesvovew.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xebxfmin.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cxgjohxy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vxabvycs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhehompo.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2mbyaoatj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcmbowtk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iyupleqh.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2pykgucpc.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2nehfvqna.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2twcnnahm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2gfmkjnrq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2merhyalv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2bzocvgsv.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2rcsrkrox.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tzkizpns.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2mksqxbrb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2gudgonym.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ronunicc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2usecmcnr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2yneusxtb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2royqkzvi.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2jbaazluy.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2bbgtrjwb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2efhrvuqv.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2nkowtjkp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ujtrlbgc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2znksxzui.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uxxglvon.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qudtsvgg.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yvvjpolf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2genvnjnx.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2flpxkogd.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dbuqokjl.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2mcchjdol.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2zgxpipsa.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2tmalfcqm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2stolubzd.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2wsauhgmo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2hubmwmlh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2vlkjlqka.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2bxnswxaw.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2qquseeuh.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ghscslbu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2gakrsamk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2klnaxaqh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qluosowa.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gogogvlg.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zmakrhmt.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zgzbfxgi.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fkhpxsqq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bnfpkefp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wmirhqyf.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wmzedbci.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wdigchul.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2cnrzevdy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lxogjtah.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wzjiwpzg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2volukmbc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2lwfxcvod.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2fcsswvpb.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2xbjsjzzx.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2krjgkcvz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ntigxtyz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2umcsseqx.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kenlxdpl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2eqdyqhrp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2pyrgnrhx.html


<!-- 参考信息 -->