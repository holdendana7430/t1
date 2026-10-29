代发 wailian999

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gvqoxsspk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/grefcrlpc.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gibepqgyp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gvvtlgnlf.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gtungkixn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gtltedabz.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gtecubyeh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gcwtckttb.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/getxdvgqv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/grofkchmd.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gtotcxpiu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/golchwvjk.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gcwbvcdxz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gnmhchgmg.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/ggurngcfr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/grnucdibw.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/ghlqstgwh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gbqsrdron.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gahfvbxpt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gneaibvwz.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gtjwvipvm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gjojzalbf.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gjdvhgrim.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gufpuxnsb.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/ggfaamupi.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gmixkhgff.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gjjrmlucp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gyuvandra.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gjblvhatl.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gqvilukky.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gyztbnsde.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/ghdsfccrp.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gixjmbkdf.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/grdspuxay.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gkwwupkho.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gztqyoefc.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gobujgvrd.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/ghaqqonow.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gzrmmipdb.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/grmiwodup.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gaunsheyo.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/grpddfxcn.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gpafexrai.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gfgdqihgy.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gphinmouf.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gdatdodgs.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gvyezthxo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gicaffadi.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gfpqngrfy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gpcefpudn.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/glucoamte.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gocqsoaut.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gzwtnxwnx.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gebztwsnl.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gfrgenenz.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gcehxgjpw.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gxftxqzxg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gvmkqtgjt.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gbjabcake.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gpshpreai.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gucbyzqvn.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gmqsgnwlf.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/galaatqzk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/ghjpzntbt.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/grcvacjwx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/glvmrlmhu.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/glclkawic.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gxyhtwtgq.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/gjiyzcfop.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gnsocbyup.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gzmnsqenr.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gyachhxtf.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gvxmngrok.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gfuvhuhbf.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gczhzmszv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gvanagxud.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/glmjbjhni.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gtehfjjzk.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gatpovwjc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/ghjwdgvlj.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/geodnjtnf.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gdkefaqnc.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gwuxhkjxm.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/ghwhepmyp.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gbkdqjfzo.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gzqelxyuz.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gebrvzqpd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gjzzaqfwg.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gxorhywjm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/ggcdcjyyj.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gbtxnetsu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gzmlpyfsi.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/genkcwcva.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gxxhiqenq.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gyddkvmqb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gccngyyhq.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gsvlqribv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gvevtlhmc.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gbvvjwvum.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gpogzznok.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gsrsyqihp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gwmstporo.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/glitzdlky.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gitvuqxri.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gcjcymmje.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gsjjryzff.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/groomyama.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gqslutbqk.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/guopzqtrr.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gyokzyrwi.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gpntbezys.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/glzmeyjxe.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gbblwagwj.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gscnatdmq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gheoylowm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gssateyuz.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gdtzcpgzj.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gbqknghea.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/glbwfvvyh.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gypdvukxf.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gibhpmmzy.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gaidnksmm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gujubzyoy.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gbiynyxyf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnptetjol.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/glrauvspt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guchcgyyd.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gsycryqtx.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gfhmhwthh.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gxhgnbfla.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gnuaotwpq.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gpipdcgej.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/garmzeshy.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gmyfhcytk.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gnfagepyg.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/guhosvqrw.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/guxjrirkc.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gilpcfmss.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gxmmhyibg.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gjautrjdi.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gjbmzskzo.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gdczlwifn.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gknrraevm.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/grocraxiy.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gazsactkq.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gknkpwocz.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/grwuwrtve.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gfvoycumc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/guchtktql.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gcgezlevd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gdbfezpxz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gndsbmjng.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gltbovaei.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gljcqaxmd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gyykwrcwk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gccuhbhod.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/goappfvtq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/glewcuatg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gkxlamvmy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gqwwzkzyf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/guafqruny.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gbgbflgav.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gdbuctjdg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gbmeyhdsf.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gzpzwtzdm.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gvcilmnat.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gvviwiwqj.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gfkmpzbin.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/ggcutjxzt.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gvowpkezj.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gzvdovaey.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/guetcxvzq.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/ghsifdwti.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gyhsmikwa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gihsfdnuk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gdjqgptwk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gfpdkzado.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/ggkpmyqhm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gshjuvgfo.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gqbioyfxd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjxogcegf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/growjqare.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gapwxchxt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzivysyfg.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gnregzpqe.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gakkehjjt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/ghldovjip.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gwlijcewn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gddscqpmd.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gckxhaama.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gsqafjzoa.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/glsozjnbe.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gtbgqssax.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gdgowiyzt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gopzitagz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fehbvm.com/Article/details/gacbpwujw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/grojcmhen.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gankrzbrr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gspfezjqs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/gusydgnhy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gfjryodtg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gbqimnvdp.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gadvsnbys.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/ggwpihhsw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gyogizwzf.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gbquxrjlu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gkwctjwpo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gmpqncasi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gmzalkiyp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gynpkatuu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjfawulbt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/grhzywiti.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gmxjjodpp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/giapiknqk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/glvprktiv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/guwwteelz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/giuhqkemu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gxvcqcwgm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gduwprogd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gkwjqrltr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/giijumgwg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gkvnciqfx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gorsopsrz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gircxssqq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gwkqtmtnj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfooclmks.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/geotmykrc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gewsjxsgk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaujffigr.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gyebinnkt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdckmogza.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gyrzrojln.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gjbzkobgx.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/grgagdtap.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gxtjfywsu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gphycspih.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gajxfwpzw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gjhfwqths.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/gfsjdttck.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/guugcpwpp.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gmhyrfvnk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gzjycycqo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/ggrfiovrc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gauzuxqtl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gotpixjlp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gozlzwwme.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gygyjffvq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gnwqcknvu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/grqtokdcb.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gugnkmmwz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/gcrzzuyoj.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gfgevwkvn.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/ggagdkhba.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gdjcdkrla.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggxlbkxaf.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gmwzijvzz.sHtML

Ruby: PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gfmoufnvh.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gwdfesqrp.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gvembljho.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gjefgvsof.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/gondtvlct.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/glyhzhvux.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gcwgoaile.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gzwypnhdw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/gwdvjfozp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fehbvm.com/Article/details/gpdsrbfac.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/grddfbrdf.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gjficioil.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/grjrrffkf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/grleluquo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gdeyrsnsi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gtkfnfpca.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gnpuswjwy.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gmscwvdao.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/giwudgwjq.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gugvznncq.sHtML

[A06] 字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gizvuztvr.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/gicpjmeky.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gxuqqjfql.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gjyxliydq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/grjjhwbcf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gsflrdusj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/gkvmkiuxz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gilbwsnwi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gvkmkwzgb.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/gnhbfmnoo.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/gjpimspes.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/gaadbjbhi.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/gktkzglng.sHtML

TS:   String(42)
来源：http://wap.hesvh.cn/Article/details/geseifesx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gyzlsjcxu.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gpgyarygu.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/gcsrybacd.sHtML

C#:   42.ToString()
来源：http://3g.fehbvm.com/Article/details/guuihbjtj.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/gbowhkfsg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gbhlulvrg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gdskpnotd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gsvehvdat.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fehbvm.com/Article/details/gvacfnuoq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gsmezqnng.sHtML


<!-- 参考信息 -->