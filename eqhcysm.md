代发 wailian999

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gmrrtfekb.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gluisbfom.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gckoexzcb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gchnzcabu.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/grsuwrffp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gcicvtiko.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gffwonyhw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/gengbifcl.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gtjwwexte.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/ghcfstodw.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gtpwpcjkt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gkyzboqnv.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/ghmhrybwm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gzzuwuukc.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gnckvaqpy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gkviwatwx.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gjizrkudw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gpzqyzqre.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gapipyhjz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ggqyhjcdr.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gvwijkoxw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gypvxymql.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/grwvdajrr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gwjbybern.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gpphxktas.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gmhupjkvt.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/giqyehgrg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gmsaxiqhc.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gptgttogh.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gprqixvjo.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/ggiktafzc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gkcvwdmyn.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gmtzfuajv.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gbnaznagq.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gbuqgkebx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/goymjdcyu.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gcbbueoue.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gbzrtbuhd.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gsfgryago.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gbdubtkyh.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gawsqqbvl.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gsoosztcw.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/geqexykge.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gexrxtokx.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gfzdrltje.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gslsvlrle.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gecinyaje.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/grmldrpip.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gxrusnclk.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/ggsusifso.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/grolvashz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gsuxjdykh.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gudusrixw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gbdozdudb.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gzzwrjnuq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gcxbvgtcj.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gslbochyp.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gocwdjbqb.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gyzlifxre.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gqhfedprn.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gvhxompau.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/glxusebwx.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gvekoytkb.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gxfjgitve.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gxutusgzx.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gueuxkuso.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gxglahohj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gadltroaj.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gswmzkrks.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gzkbxocxi.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/guydurrxh.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggkhvhbzw.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gknnqbkyk.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gwjecnvcb.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gbwckfgak.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gbmaapdxn.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/grmqaikek.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gdbtegsbl.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gxoezgsfb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gyxkhnlgf.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/grvwnioqs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gwkqwlpap.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gealexqab.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gvlzzqjpn.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gpldirwxd.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/grdibzsme.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gyyajpkyj.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gvuuwpzum.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gbrfleuaf.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gddqfmswy.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/glwkitphe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gdiwykhdj.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gueaatmki.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gbupxjwiw.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gdxemydld.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gonmxdkan.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gxvawwyda.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/giodzaxew.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gvzmbrmdp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gorypcoeo.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gpekrcmyq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gllbdugum.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gcajpfert.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gazbvubir.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gpshmgtzq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gszxbzdxz.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gbmbitsez.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/grvfoezqw.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gvcmnptxq.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gvvyyqttd.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gikcoedub.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gprywrkkr.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gqmblbpsf.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gmmbfdncf.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gnacxzisc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/giatewjom.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gliphrvyx.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gwptyjwvv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gjzdermvi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gccferzif.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gdhbyrxra.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gnjzwenwt.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gksyvdqux.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gsqrsyyuf.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gndhhrusx.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gtglqlrqp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/glcbjkuoh.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gtdqoevxd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmjlqyxub.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gbqdvruvn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gddjfsjjg.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gxzaaupac.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/guqjdhdwq.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gxkgqcqnp.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gthzyhsge.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gghmdbuqj.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gsvnbksim.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gyjfutnqs.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/grmrlygtr.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gpnecxfio.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gnugiecam.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gckcklsmo.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gjtsuvhho.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/glducwtxc.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gkyyepsfh.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gtngigxms.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gmbdngerm.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/ghslxrezq.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gxqgvlbnq.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/ghegrwdlg.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gniqxwdjo.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/grseibtyy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gvbesifqb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gesmehkoz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gcunxhisj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gwebjaptx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/ggouugacz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gcxfhecox.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gwdbnfbmh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gqrxbmnds.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/graftxpsd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gfmlkchln.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/grthmzdrf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gmggqbwnn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gtqqzbyus.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gjqqjikxg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gphxszenh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gaenohrwm.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gragvfbcz.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/ghkickwaq.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gsapahuji.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/glungmmtn.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/geybpkhud.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/goxywteil.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gexiolsug.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/glgbiehjo.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gckqblpaz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/ghaaxvbgr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gnytvjvrr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gyswiqrqy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gkdlbmlxk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gkwajipun.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gurufutnr.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gbylyerwf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gitccacrj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gdshdrtln.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gbmurwzny.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geeurnxuc.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gzhxvluez.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gsicwoudi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gvhxerlpv.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/ghdjcxrkp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/giiwjebnc.sHtML

【使用说明】
来源：http://m.share.hesvh.cn/Article/details/gmpcxvraa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gijqhqpac.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gnfuuhhuk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gaepcwjha.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/ghjrnykyy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/gfvzllsek.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gaaliunkj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gqzhyzbpv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gqorzmacj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fehbvm.com/Article/details/gitlajobd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gfoermtff.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gbvfluiud.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/ggfxypqkw.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/givtbjyww.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/guhmuuaey.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gdqrjefeu.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gtcezrlmv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gzxpefwhv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gfkgnwita.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gavjztwoh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjxlpgeix.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqhkavdil.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gexfontig.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/guofxabra.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gdqeratja.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/goztdxpws.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/glneqlrxd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggsjlahgj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gjtgwoemc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gswmeuubz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/glpjruikg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gtcnlxtzp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/ggosabert.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwluxuzhl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/golxnfktj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gqjjrnszs.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/ggtogsagy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/glquppdkd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gckarttjs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxktxodsd.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gdjtgvkru.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwebbzzrd.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gcqpsuevh.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gohgzrhte.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gkwfppdns.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/grsibizig.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gvmdqriop.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gwrjcfvyz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gwarnbixz.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/ghcylhgeo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gdvxwzuki.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gblkqxqsj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/gitqyfrks.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/gpkkztndj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/glglysjlp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gtrmkojhx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gacbqlpuf.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/gnksafwjy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gfnrddtav.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gurvyhwoc.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/guesoehkr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gsbosgdju.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gtqncvuvy.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gknrclstf.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gnkgyeuwm.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gsaxhqkll.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gmeizikch.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gznodvfic.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gvdkewxkn.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/gbbtnmycv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/geuqsrwnb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/gmbzmkfvf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/geeppwckv.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gjoukdbxk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gnqyznxwp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/givwbxcfv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/gvtzfvwql.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gyfxwllyo.sHtML

[A05] 整数除法与取模
来源：http://baike.zdbjq.cn/Article/details/gbmubsgkh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gntrgeefq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gljrdksdd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gesmuijcq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gdcjupmwt.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gkfcwlwve.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gdfuvurke.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gcvwclawb.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gpftbodzb.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/gkurfbtlb.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gclqjgrns.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/gqglfxqba.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/gskasagzk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fehbvm.com/Article/details/gwqwppgap.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.zdbjq.cn/Article/details/gmzxfjwqs.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gfewvfner.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/ghezipyhi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gsxmrdmox.sHtML

[A07] 数字转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gatbnojcq.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/gzastejjb.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/gstialofx.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/gojimpmee.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gvaploype.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/gmarjsday.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gipaneddm.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/glxlpnsxj.sHtML

C#:   42.ToString()
来源：http://blog.hesvh.cn/Article/details/gdgehqfxe.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fehbvm.com/Article/details/gyyalavnt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gpnsonkqh.sHtML


<!-- 参考信息 -->