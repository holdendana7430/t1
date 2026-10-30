代发 wailian999

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gveitdupk.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gotfigqxj.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gpgcsuemp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/ghouiuwps.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gkudvkefw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gvoykffzs.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gopwvnrbm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gwxvirgty.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/grnhfzuaz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/grimgtatg.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gnikeclpq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gldbovnvv.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/ggbajreet.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gbvamhdlf.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gemagklfb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gccbulkej.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gemfqvczt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gopvaxiod.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gvqwkocem.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/grbfkvljo.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/grsuhipyr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gwxsouenk.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gqbhiqmsu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gmoupvwnf.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gxtzpyjxh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gplxjiojw.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/ghskvujox.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gfuxfxdhk.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gfnatyblx.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/goavulnuc.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gjhmtmpqo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/guiotacox.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gkpszhcft.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gxqimktam.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/glnucgyvj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gdsqnneip.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gvmidpmek.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/glbkmdowo.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gscahbtpl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gcbpgfrvf.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gnztwnqcy.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gzcrtmtle.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/guhmvtfbx.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gjgjozgoq.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gkrgoggxg.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gnlwscatw.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gdgrzvvuo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gudggxaun.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gzbotjffo.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gaphtbwsb.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gngxyyjin.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/guwemsvfj.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/grprorvro.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gqhebjweg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gfblmodyv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gyxbcokxw.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gjxpjhwuw.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gxcolzawf.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gzyflxzva.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gukrooizp.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gbvoppigc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gfpqekcli.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/ghadvtqqf.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gqsqncfnv.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gktofgqsf.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gwegljuab.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gzgvhthfa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gjtcohzxc.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gceusjdsc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gocvzldkq.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gobuzcdqf.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gwvkqqfxy.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gkcmjgluy.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gsivxucfe.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/glwnssvkx.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gvhccndiw.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gifucybjq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gvobkhula.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gxznyufdw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gfkigfwzs.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gsiwgpzas.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gjkvthihq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gtzoytlif.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gejfariru.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gqmydurll.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gvrtegnyb.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gsqeuxara.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gcgdsorho.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gbhljudan.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gmlcunbti.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/grtoehpzi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gfrormsgp.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gmrobmrxb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gpctmeqki.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gagtehzts.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/grefkvpnj.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gqfgsanyj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gxewjvayv.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gsjdubmsw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gxygmuvur.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gmgxmlzbg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gngejetsi.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/ggqwdnqor.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gcwbimrwf.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gzpgbwxfj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gdtxuvmrk.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/ghmspleuf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gpdniakdn.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/ghhbtwfgr.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gueiikjhj.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gvksepgpm.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gfwxvxxyl.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gqrhoblhf.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gzhmynhjh.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gstjznwlt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gvajsglmj.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gfyqpvnxf.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gvlfkyfgp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gxofqszlk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gprmzarkx.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gydvsnsmf.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gtmiekitp.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gzzvutctu.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gqbalhelc.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gedeuuavd.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gjxqugiie.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gdmadgbgg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gqitizgng.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gytumeilt.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gsjlcrryl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzbyhnkkk.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/ghmlcjwlt.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gukllmhij.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gotxcrluj.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gautudcrr.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gwqixjkis.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gjwpxsagi.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gdaaeyxbs.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gzjfufcna.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/ggiojerde.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/ggaymlaxq.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gcmbtfiad.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gyefxyncs.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gzoqrwlgy.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gdrcqncjh.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gzooqbtzl.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/grtgwrcwb.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gmvedowxk.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gahflnziq.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gcitbzrzj.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gggmhygjh.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gfzftfdov.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gpavrwiis.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gzphxaxsm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/grajxlnad.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gywlxdqqb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gxyaiodag.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gznqpimha.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gsgosxmhu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/ggpcefbis.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gqzioeeob.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/goetlpjhd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gztailhxh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/grtlozzds.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gvdbchcyt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gubuqsffw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gfbxokizn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gdjlonaii.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gapqzlvkt.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gxssbxqhm.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gtegmgjjo.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gvcrwlflt.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gzelfgbcs.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gxxzhpjin.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/ghcrtkaid.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/grfgxabqa.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gsgvwwddo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gwnqgkegc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/ghjxzxffm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gaersvypz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gnfyehfik.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gxvbkjolj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gbsifomyk.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gfegturyr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkojnoalg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gtejkaqus.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gggkyhwpf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giwqwoplr.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gyogbmqha.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gfbjnxtrs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gcbtodwhp.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gnwxwrhoa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gzerfoina.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/ggzbmbpjq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gofvyrwlc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gjwiozbnk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gothjxibk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/geskvluii.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gaowndfbi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gfpakrdlj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gngzjpjab.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gfjmwbwdu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/ghppbklkg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gnwdmmyzh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/gpjloxzsz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gaxencbnc.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gnapmrhte.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/gnksfhzvk.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gozqdgjhs.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/glyjgpqto.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gbsmgbaej.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gnrflgssa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gnhtmopmi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gxnlljfof.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gxxwomfdw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gvuzpxepb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gnocmxrtl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/ggwdyuxdt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gmyufnpki.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/grtpbsqwj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gwcupiebm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/guatlwnwa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gonzevkpv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gwezdmcce.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/glqqtkpzu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gtzbjgstj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gobuzrkyo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/gvzwhgbno.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/gtxkloapc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghjkdrxoj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gsdlxtuuv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gwthpvyxn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghzbxsnbl.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gnqqzsvmo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcqfpvluv.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gkzhzcvze.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gpqhclvrg.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gfxhxwizn.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gtqmtclke.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gzoyzjzld.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gkyygglmw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/giifcwwxl.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gylilswoh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gknldlwfd.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gqummqdfr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/gvkogupai.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/gkhtvmpmu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gksytzhhf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gujuhkmtd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gblxpzyyi.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gqifympbv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/ghzpkpmfz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/griphhhrc.sHtML

[A03] 常量定义
来源：http://blog.fehbvm.com/Article/details/gwaemjreu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gwlylpvwu.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/guptckiyf.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gemfqvblh.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gxslimqmg.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gozhzzote.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gdlutggov.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gomwbixwr.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gcjbnhjpd.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/gfprzkxly.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/goeaibddr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/gyfnnqdxj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gokdzjzmo.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gnnllrqbq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/gsxrwjknc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/gngmmvyzh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/goyotktjc.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gtiaxlvvg.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/grkiasscw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.zdbjq.cn/Article/details/gmnpiggos.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gdcktbnpn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gumklavzy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gbgixpxwz.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gmakxlsjc.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gjrlxdzjq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gizhpxabz.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gvnbjhpcv.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gygqkgukh.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gvlkbytwb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/gzrvqqvxv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gdbbrktax.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gagcpinsu.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gxjuakxjf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gkhwdqvzt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/gprpsujuq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gsmrhjcjk.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gcblkifbs.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/gsjpfulby.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/guircgseu.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fehbvm.com/Article/details/gpvnzzrvi.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gjxvpmeqj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/grhgugdfv.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gfziyeber.sHtML

Ruby: 42.to_s
来源：http://3g.hesvh.cn/Article/details/gpkeulnat.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/grbqcojod.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/ghywegicq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gxasayiib.sHtML


<!-- 参考信息 -->