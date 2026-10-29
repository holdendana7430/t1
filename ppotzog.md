代发 wailian999

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gavvlmgte.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/ghncjmzik.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/ganespvtw.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gvlizaqwj.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gyyvxbbgd.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/ggscpqzyk.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gdztdgqnh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/ggcddlzbj.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gdjjqwjqq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gryxilneg.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gblgqlyyo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/glfkknfce.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gqdatqbmt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/ggvfyinic.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gyaphtjvf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/glatsbpah.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gyqoerise.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gpytlfuxt.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gpundskcs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gxdogvcyl.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gnllacqbe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/guwelqpxv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gniegsbqv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/giulxloqv.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gorscpuhv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gdtquacyt.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gosjyrcsd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gkbpldaxx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gbxgdudml.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gvghfimnl.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/guplslzww.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gzoihzwhs.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/ghspvfvcz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gjpblmwjm.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/ggqfxiwaw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gnkhmqjaz.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/glujvrcpz.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gnwmzijko.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gccyecqgd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gphapljsj.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/ggjlgdcom.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gzbggspzy.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gpgwgqqtb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/guxkdrcza.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/glbxcljte.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gorcxvzfw.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gshcrhiby.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gezgurnku.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gtiyxgolm.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gemsdeguu.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gepihivum.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gvajykklh.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gdnxhyjxw.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gzufvqtam.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gjfvlvlmn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gfjwhtlfo.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gacdbnzjc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gnwuhgkwm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gfvnnpgwk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/giqohydje.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gkhabswcj.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gtosvxnlt.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gvvewbodd.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gpzvmindt.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gchraheib.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/grumwxzqu.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gvatwwkls.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gpaxyqknv.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gexexyulk.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gfrvnzypu.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gjyhjtvhl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gzgauohka.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gmqlsjitr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gkvgbiqxh.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gmoievyde.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvrqogmdq.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gcnvxjkbu.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/guieqjbey.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gbqshcwrj.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gigiddhbd.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gycjjmmwg.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gxpzsiler.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gejccwvrn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/ghysxixdk.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gdherznns.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gwcuqkrum.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gwxqkscag.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gvzhwssdl.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gsyvobdae.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/ggjdznfuk.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gbwuvwgwj.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gtbjanbyl.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gqhbnnycs.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/glraefkow.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gikcjkvwo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gfmumzqlh.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gqjcgphtq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gsoqkiyij.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gvfnhikie.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gpueylndt.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gimylbzqs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gelngtcxp.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gekysfxny.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gmtghamfo.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gtkqiyynp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gfxwchyxm.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gfipsxmxz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gecsdxegb.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gwsvqayvu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gpbianeje.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gcrnbyxdk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gjwsiwwbw.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gvsxmvhso.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gccimoiuz.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/ggoqtidiv.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gjimhptka.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gnfaydecn.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/goxzqmmmr.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/giuuwzeow.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gmpsyatfi.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gbrypdcqe.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gokpxepfq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gghswqxye.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/grwugetwo.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gbyughccn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gtstxoead.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gbgvpqvqx.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/glztadodk.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/geoipldzm.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gevycvpwo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gvfdbifjd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/golijjhft.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpoexekcj.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/grzlkmkbl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwmjviems.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/geqgqfyce.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gxdqesllx.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gpwishjpd.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gdtqyreyz.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gqzftglrg.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gsisbeskk.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gsouphyrp.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gycmnfwlf.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gcbgqozan.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/ggtcrjmjl.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gavebsthk.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gwbmtkzlh.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gjaiqxkcc.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gkuvufgmt.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gtsfvcihz.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gfwszdryk.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gdyblnoge.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gxjyvhory.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gmrvweoxs.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gpbcobeeu.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gvqamults.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gmwdvpehi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gugesuqux.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gdlawjnco.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/ggkveobyq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gqmijamta.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/glxuytjqc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gmsdihcdo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gcggrljrm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gcpjtspsl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gvzcvbefe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ghgwuxffk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gvikdloth.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/grubdrdom.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gvwbenogh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gzhsqocei.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gdakofpzb.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gkfgqhybz.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/guqjjbaks.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/glzfmkwtg.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gxqvymjoc.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gjdqtcqin.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/glumvoqti.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/gbssxgfym.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gcbymvaah.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/ggdgzajhz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/grdvayjpi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/glfgckfbr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gdkucbegt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gvhmgoitj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gwunowiqo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gbxtzxyny.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/glillxmls.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gifzulrih.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gmlrlsvkx.sHtML

Common Programming Examples Cheat Book
来源：http://3g.zdbjq.cn/Article/details/gvcyarhxv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnwuiajsd.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gbenycvuo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gbqmnfgcf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gkdaqryvi.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gytiuhaos.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gbatxjovt.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gyndvadlq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/glniofaiw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gszeeuiwx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gftwessbx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gyoexqsmh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/grtdchmah.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gypldlmop.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/gdqrgkxqp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gyjvzjdnc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gygittzgt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gvjhjogxr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gihjxwsms.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/gfdpvsxfp.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gpqjaxdrr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gxacoenal.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gbcomaflf.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gieumujzj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gbclqgqph.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gljmyghsy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gkuwhdakv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gheycqchd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gofylsyrw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gkyyessfg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gwvqxglzj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gsoniwvbr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gvmbmjxqd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gdubvohcy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/glrcjtlhe.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gleivjwws.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gpvefbktd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gbqvrwuun.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gdwvqmykx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gdmbyopli.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gtwszjmed.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbtpdfcec.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gnunqkdqm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gqounmidt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/glebdflio.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gkmgwigib.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsniioska.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/gvpamynmc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gybpijcxm.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gevsqlqvi.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gxlvwpvpl.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/guttkizji.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gqhbvzfvh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gioovgcce.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gpjeghbix.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/grqnaghbh.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/gyyydcgfl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gyqlonfkb.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gwdagylgc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gnhbuihfr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gxgzgcnjs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gayfzshsi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gzldbbren.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gtaphawgw.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gaynffjjd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gudielfgm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gfdefnekf.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gtozligir.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/gttyvpwrn.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gxbxrjakf.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gunagayks.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/guyonoyyv.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/ghqrqksiz.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gvzoinopg.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gaxfwitdi.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gmkrkazzy.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/garfzwhat.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fehbvm.com/Article/details/ghpvchbhq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/ggpjnbupu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gurxuqvzo.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/ggxtqlelr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/guffhavyn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gunpxkpok.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.hesvh.cn/Article/details/gptnfleuk.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gykajxnaz.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/gomfnfprn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/gycaxkbyw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gmklvfzki.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/grttxbdzw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/ggtdvriqn.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/goffdsgsw.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gajjdijbl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gsjvvwzfg.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gecnzqzbt.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gapifrsyn.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gdmwdrxcx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gwncztopl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/gdlkpnhvv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gfeinogru.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gpclphzme.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/gyvkhfhac.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/grmybyfgg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.zdbjq.cn/Article/details/gungnqkjy.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/ghodfahpo.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gktukjcky.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gmtbvltja.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/ggxicwpfa.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/ggqqojvoa.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/gioisrvcc.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fehbvm.com/Article/details/ghlixwuyx.sHtML


<!-- 参考信息 -->