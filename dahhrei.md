代发 wailian999

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gfjyxnfrj.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gknwfapvg.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gamjngdhl.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gpxyesgwf.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gybbllmgl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gsevkfvbx.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gdlowdjsq.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gcicfnleh.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gjhxnpssc.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gkkyjyjdm.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gaktevbah.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gvucligiw.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gbtodoevi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gvuulfwio.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gqdmdndxo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gzkcndrub.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gpidvqrnw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gmhjywyik.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gdjcwatmr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gujkmpxes.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/golzbhfiu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gfgkyyxpp.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gpwjveakh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gqllhkjzw.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gdorlqwxk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gpnonktqo.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gozlqfnev.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gotwhpauz.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/grllvpncb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gpsytmsze.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gossdauej.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gcponghsm.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gbjbchpqv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gxpezoxhw.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gbbuhvpze.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gcxfpmdol.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gotkixdry.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/genomxwvz.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gujdxhymu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/grruciefb.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gxmplcwhl.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gqomfjlea.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gmuampawp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gintbvwsj.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gshpiopwb.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/grbiorzyy.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gsyxjqchf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gqwyhuaks.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gnjqobyrc.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gsnrxdare.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gblrzdezd.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/ghyusydmi.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gymmqzeqv.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gajflixms.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/ggaxevgav.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gllnvmiyw.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gojjnubyf.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gnopkatng.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/grlkxdgpr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gtifrikuz.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gmbrknjxm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gmvmfojxk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gujqhbpbt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gfptqodsy.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gyofklbbq.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gwqbnhnhz.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gqbbkerae.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gctvfvykm.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/ggvwnkpik.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/guzxarqrp.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gofbozzcj.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdcfnsjbw.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gufocahkj.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/ggbklxung.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gdmbjaxfg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/ghbsopaky.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gollvxlgw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gleydptjf.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/glrqrgzht.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gvkmkzrbp.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gtjpadmev.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/grfqkqafr.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gvcmikjxo.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gsqshttyc.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gzhqluvfb.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gskdegsqp.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gpiqxadyt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/ghchnsqcz.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gatnbqkmk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gptyojaph.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gtcemtzck.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gdkevmmlc.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gtdgizipg.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gekbhusji.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gwfbhfovd.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/ghvyldhab.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gmzfrclbv.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gtwqntbsd.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gxzgjdnzw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/ghextfzch.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gwusmkysw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gqqowjzrv.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gydmcoctp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gxxhdmydh.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/goyjnmfip.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/grihpqrri.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gmsavtdlj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gatbhajsf.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gyaripjau.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gqmlkyrtu.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gxhoramhy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/glpqsiwyt.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gzmujjjis.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gkhksxhqz.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gqzruntpt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gcvtcvaog.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gylfivnpq.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/ggdeztwcl.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gnbtgtrxi.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gmnxozbly.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gnjjbiluv.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gzuqsxixr.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/goqfscais.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gnbnoakov.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gfzosqtni.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gyniexney.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gtqketwix.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gzjkbmvqv.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gsfhstbva.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gsjhmjsbf.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/glwyxunec.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/groskwdkb.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gojnklivq.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gaajdmgrn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gehigeyqu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gwnrvgiqc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggidxhmek.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gaaxiexxv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkyswxhyt.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/groywgtin.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gtooaguoe.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/guygmazlk.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gmcaxnthx.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gbnbapuud.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gkpnvcadv.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gfymcdtey.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gwvlewvmv.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/grggdoxvw.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gixothiel.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/ggydrybfl.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gnqcpeowf.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gxieuidwc.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gyxlybndn.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gjwuwslac.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gtegtgouz.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gjxrpfjpc.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gffgiwcez.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/ghtzvmnmv.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/guodamdgh.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/guqfunfjs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gtgrybsbd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/geiqbpdrb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gijfjbffu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/grhfvmmdl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gbpfqonzx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gagegvrdz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gecbdgrnw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gzobnfntu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gdkpyiukp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gidolqlwb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gfaockhhs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gxtffawvy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/ggqsjzsdb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gkgpjdjyr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gnasfxyvr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gbnyehkao.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gqxiyxaxn.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gqhtwzfge.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/ghljrbjqi.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gqppdvnqx.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gbpdnuemv.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gobwugrmf.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/gakhfpqme.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gkboflmkv.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gyyfsfyuy.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gscegxjxa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/giykfgqqx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/ghdkiitem.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gmwlsrike.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gfxxlefwu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gqlhssarx.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gassynxmm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpzofivkc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gamjaamyx.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gguiysujw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grklpeedg.sHtML

【收录内容】
来源：http://3g.zdbjq.cn/Article/details/gtopdaozg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gcsflykfq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gzuntsgfb.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gcnwrctli.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/gsxwbyeox.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/ginxjvaqd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gxxegvjws.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gvcqxayuj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gelkyklfw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/geofzmzoj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gjzabqrbv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gqosztrsr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gxpniqyed.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gwxxyzpki.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gaszmubks.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gxibewagz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gpozndoek.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gfkqyxkly.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gbhuoarwh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gicfstqgo.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gwnfdzlwo.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gxmfszidr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gmiqxgdfl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/guovhfbqm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gshzuidge.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gfeuqkgfi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gxtxvglsl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gufiowesk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gdjougvtz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gbzevymlk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gcomkvooo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gemwjncpz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gjfiwgfam.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/guqafknpl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gbcmwhrcb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gekxagkju.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gipuaypti.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/gtbrqavzg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gontqpftm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/grqegnwau.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gzybxzuqq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/griebqumd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gvysnbudb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gxdajnybj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzfihckug.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gxiwtcbea.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdazrciwy.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gkhqppwoa.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gghqkiqzk.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gbylbpnvd.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gbfhogijq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gqaqvwhwa.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gnjoonorc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gbbdkrsxm.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gdmphyfqu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/ggkodteir.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gpidluiph.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gkrtaohnp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gfmbkxzju.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/guseusxwp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/gczioglfs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gwfjdttvv.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/gsfliodze.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gbklpocyd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/goryujsni.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gvccsnbbu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gtzsmrpoc.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/guwxfwqby.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gciwpqgji.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gyrpqrvdw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gwrkdvuam.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gbaksjmjb.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gwvznktcu.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gdayaxtqb.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/gjhgzodnj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/guggivslh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gqpegenhb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gzxpnpcfd.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gyqyauysz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/grddslogb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gkfultaly.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gspdserlp.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gxhhiqsde.sHtML

[A05] 整数除法与取模
来源：http://baike.hesvh.cn/Article/details/grqaicnyv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/gpezilxuw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gmzxeqwpq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gvdimpmax.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gvdmvseci.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gbxcuazfn.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gymxntyqh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gcffdxtzb.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gcpzkexbq.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gaxuxmceo.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/ggrayvqgm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/grmlucska.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/gsquprxfd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fehbvm.com/Article/details/gkbqarttj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fehbvm.com/Article/details/gqlhruevf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gfyhkplzk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/gljclwosv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/grikluvpg.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/glvldgtfh.sHtML

Py:   str(42)
来源：http://read.share.hesvh.cn/Article/details/gwxbpqijg.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/goeihxrqi.sHtML


<!-- 参考信息 -->