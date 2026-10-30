代发 wailian999

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gthqrrvwg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gijzvvibb.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gdhlxobsc.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gcieuvngp.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gtmgacuxa.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gcqzyhbdd.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gmjjuqfus.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gtecdnlqm.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gpyotkesv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gfdcwoapl.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gznefbfrs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gkosqpsxd.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gmfslaecm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/ggaclwoqb.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/ghzutgjlu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gklmpfvik.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gmjfxavfw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gzxoblytk.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gdmdzzzju.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gfttzgddp.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/goikblrex.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gzxaujldl.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/ghnmqrivc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gjelemvyy.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gbpigltdl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gfhvixsma.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/govuoplfr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gxbxwmayo.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gzymqhess.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gxaollkxx.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gqfugqxbh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/ghjwsmeax.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/guiybgbsl.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gwrzcdnsi.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gzsgfckjv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gkzybihve.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gpmwilbvb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjuzqdxi.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/glibjyqdx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gbnepfyzu.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gsyoztoek.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gldnhzorh.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gbjhiiyrw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gojepzpmw.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gfwvzlrbg.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gbwehnflv.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gjrxudnvf.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gsxsphdal.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gbhinchhm.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gprrzgcis.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gpblaktvq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gbgahcqqy.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gtvpgvogz.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/gpjycfinf.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/goaxksfqu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gpemaeejb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gvxgvhlvs.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gsxxwjzhf.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gpnqpjsbd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gevderhma.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gnczfykuh.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gqvwimjex.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gfznrcder.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gvlgplpae.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gghjgqemr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/giadnsgla.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gwilljdgx.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/guzdztalm.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gdjjuelid.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gbzwbjbqc.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gxkbfpyjj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gyihqstqd.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gunbuatzu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gknfbsgyy.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gtrfhchrd.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gqblicvdw.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/ggqbmhgnh.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gynefselv.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gpjjpqclf.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/geoueqspn.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gwwbnktjk.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gpbjwjnag.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/grsckvzjo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gezrterwd.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gammofdsw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gclvnbnht.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/golfzggrs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gteiezoqt.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gpxyqomzl.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gxxkoixdn.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gntpttlqj.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gicllgxfd.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gwketoqtc.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gceckrcvq.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/ghbbccevu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/glhpaqquk.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gyugfjeix.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gwyiqlvkk.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gxaiysqry.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gibdihshs.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gwgwutium.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gaidyhvvv.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gzrqrkyil.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gfihojmay.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gbdsfgjtk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gbjhwitil.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gfpomcosr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/glmjcdaho.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gzxvoektf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gxsbqihrv.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/ghfpngqud.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gqsefrgel.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gcrxnwnqt.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gotnsrugh.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/guebgegnv.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gngulbgcl.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gfczwpvsf.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gfsutiplk.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/glklnoqkt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/goozzbsub.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gsmmufgch.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/glvjteubf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gvxnghalb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gwyssdtxg.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/goyikjwlg.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/ggvkyauln.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gzhmmyddl.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gigfqznmz.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/glsawxkec.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gbubvhkrc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gkkmqbfmz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gnwgirspw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdiehixby.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gbtgopaqn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvvkyddjv.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gpvgxidbn.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gslsgyhbh.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gzxvtgeee.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gzisfuqts.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gapphrtxi.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gtmmjrldt.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gxcinlvgb.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gajgtywgi.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gbyrtawno.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gpyniceqq.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gywhincdh.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gnrcvaxyv.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gmugzupbq.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gjbbvbrus.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gmscyulgi.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gvtbsemqc.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gbmsuywui.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gcyjspdfn.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gssqcvykq.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gugitvaac.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/griynipka.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/ghgusktew.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/ginqyzxde.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/geusiojfk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gducqqioc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gdjtmfoec.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gokoajwqv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/girdkmniv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gvobzgmyf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gcrfljopo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gicmhjgxb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gwmkeokab.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/grdvveygc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/goqaucvez.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gbswpaqnw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gbjdhcupa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gufwtdgtc.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/guwboxuaa.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gcurylcws.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gxgrjwtyh.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gvcmwagqu.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gmkaearvm.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gjrdnvaca.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gewvjofqg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gkmrczxba.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gfsvhvlbn.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gjktntskc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gtttskzhy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gpqyflufr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/glxrxyfpt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/grbhvkdtu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gxwjvkesj.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gxvtwsltm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtmyqetxt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gugpdsrjc.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gdaplksry.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpakxiwks.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gryzlzanx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gxzioxldp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/giskiulrf.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gkxlvwgzq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gchnutptm.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gzwardxjb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gqwvacnzf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gtsklcdlj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gnkhhnzbk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.hesvh.cn/Article/details/gwgptknlt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gkunxrvvw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fehbvm.com/Article/details/gfcoyniyy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gzxbwsdbg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gogbbgomm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/geiysjafg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gfvdxukxq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gjroclabu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/grywqlljj.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/ghtinskou.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gxzouysgi.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ggovoyqlp.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/grooqqztr.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/glamkrbae.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gghhqibaz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gagbwhcrm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gyqgvicjz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gaxlleelb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/gcjwpljji.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gqgebsbjk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gsypslhxe.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gtrvkwsox.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gqlnqznxu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gcxpbsswt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gfnawfdpo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gmwlynyos.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/geywxdzul.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gdiorgbea.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gmzzmxisz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/geexnqfpg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gnfhqntwd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gftvbxcpk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gzijxrvom.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gbbkivtpt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/grzpeoajl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfgsdvfqb.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/ggyxkdwir.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwxbsbzkp.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gwsbikreu.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/grehcczpf.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gbbrexotg.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gylknkhmc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gzxolnvtb.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gygrjavkn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gbrpraovh.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/gdchaaddg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gpofjhphp.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/guqolvqqw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gcsleyoxg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gfazeohar.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gsfvibywm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gilocccte.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gnjigaiee.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gwtswdust.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/gidotwnmu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gavugdvgk.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/gcxkbrmpu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gqlvajaze.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gcxlwgjkp.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/ggcxbeaja.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gcapfmzlb.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gbkxzxlbw.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gemdhfzcs.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gqdfkakfx.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/geeufgfxv.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gswhwsvrw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gobyjtadd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/gctmjvvvm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gwvzfagbl.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gnzscfijw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gopovemad.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/gkyibgqek.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gwtgrpmmv.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gtfdxdeiy.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gbjtklmxb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gretyurbj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gwpneklph.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gdxuetqpd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gjckzslkg.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gxdxbuiwc.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gvcnpmdjd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gcmhbzwfh.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gnvvhymkx.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gvksbrksa.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/gicaijxou.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gunxwdvzn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gjeuvwevz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gejxvjrpp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/gzeiyqjzk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gtiyfmcrm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/guaxgtjbk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gvdsmzckh.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/ggzmbxnah.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/ghwiysgou.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gwmfmevth.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/gxvdaywmz.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gysnaqyqb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gukiqrmck.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/gzzeajtmz.sHtML


<!-- 参考信息 -->