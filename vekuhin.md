代发 wailian999

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/guopizsee.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/ggtwthzqo.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzbjkshs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/grssnwine.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gekhojjlu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gtbyebaoa.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/ganetnsva.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/guxyqycsi.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsfxoakj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gcxkcegas.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjvfecml.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gwdnlncrf.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gcxrcatap.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gbxbcvmyy.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gtrmuesos.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/goodlrnxh.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdtvzxfb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkxrlnlf.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjjdkxqm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbizflgs.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/glmaocguk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtuyvukm.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhbabgjz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gwbvnojpd.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/giicnkwgj.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/gvssptuee.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkfhkhqj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/gornqdzce.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gugntzxqg.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbctzsyu.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmevhhkfj.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gmklxbfjb.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gygoqmgjj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufzrdlyl.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gzipfntbd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxcumbag.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gzbbeviwh.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gchblycfq.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohginvpz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gclpepcni.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gncfcrypv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gbdlmoumd.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gpqeaaois.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzbdduxi.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnllccno.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/ggjhvxvoo.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gbchjounh.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gngcjsvhc.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkumbbmk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/glqpysuzf.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpaifiad.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaekdcqnt.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgrqzgyp.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gapntxshl.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaazowhl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gozjohbxe.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfvkdikn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gigcfbyxc.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxakfvtqk.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggawbbyze.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gxxxsitey.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gldfyukib.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojdugish.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/grbnlitam.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsqyzvut.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfmufuvo.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gwjcnabyq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpljsjde.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gvgigjism.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/grbegihtk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/geprgvsix.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gsavrkoui.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gvilbakym.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gfidwydgy.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/ghpibgsgl.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/gwtklbcqk.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gewxwcsbw.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gyplxxbbc.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gwglwjuhl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxttllnxm.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/goiqvxgmc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvemjims.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gfuzbngmp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmeljuxa.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gtaumvwdh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrwqxejy.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbbpfike.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjrklkuz.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gypkrpndl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/ghjlmtavu.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gialmnapz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gavblqlyv.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdembssjp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gylwdjfng.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcgdiboj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gnjvnwjnd.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/givzskhhc.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwblzmhj.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gqhgzlnhl.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwivvqut.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gquamhtrs.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gosxqqarx.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gputqstvm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gnstrywyh.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttstvxiu.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gkwwukshz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gqqxogoop.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnnkvzwq.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnfucnti.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/giirfprmk.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtweooyu.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiutchqi.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwprlkhx.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/giuytiryr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gdlqgjnos.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gukitlyrf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwnjkvxg.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gfqxueypp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtxvjrvfi.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/ggnrqbxll.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxvlllsz.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gtrrtdyxr.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnwqqrbn.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqgucntx.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gihdpnqvl.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/geakzpgtv.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqywnxcr.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gjdrxdakr.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gnuwqpqrl.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/gudvaevpz.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gqocaaivd.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gobkohibu.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gurgfrogw.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/ghicchkmy.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gbqsgsxkj.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gkxbasbsx.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/glrvejvsf.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskhfcoxj.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnneahlv.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/galhojrxl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggukqotwg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gwlytfpvp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsxosgaz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/glzuqeiul.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomhkdzbr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gtawpxglr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsupmrkl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gxnicuslt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/galdcxfcs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlwpacfs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gsinregcb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpzmlqyz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzlprnqm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/ghgonudyj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gdevpuvzi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjgaqupk.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gnovevusk.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrbaiulk.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxerdtcm.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrbxfaqc.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gbaajmexu.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwhgeneh.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gmffpkqmg.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gxrfsinse.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzcpsfdj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuosjqsy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkgnxiru.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gmezlmmqk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpdfcbtw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/gydwxbywe.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/grutrkcyr.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gytgongsj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqdbazyr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gzcvjtolo.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/ggkwmlcwg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gouffckom.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/gxexqzepw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/gitmljbet.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdyjtood.sHtML

SQL · Bash · C · C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmxvjffx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gzxyuhghi.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkxrrsnu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fanxiaobao.xyz/Article/details/gvtaqxegn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/glkjhvjty.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/galrmanbc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/gxixblgoz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fanxiaobao.xyz/Article/details/gmzwzvsai.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/gqojuwggv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnacxnzx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhuynykd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcnfpbdr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fanxiaobao.xyz/Article/details/guqtblrsf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilnujtow.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/gyfdcsvbt.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuzwhxjp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fanxiaobao.xyz/Article/details/gwvqnypdz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gruaeabtc.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/gfaallgwq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/ganxoxrbn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gidkshqkh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gokosmnxl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmylfvxwb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gukcjbrim.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczycemeg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ggsveawwa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gghimgway.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/glfyybvci.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvyaubcs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvlkyirv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gtmfraxxe.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzsmzroaf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogftiuix.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvzjgiyf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcshrrwag.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/giwsshzae.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqmttcgp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/guhsiraas.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ghqisuflt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkujwphef.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gffefvnjk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glkvklshz.sHtML

A. 基础语法与类型
来源：http://wap.fanxiaobao.xyz/Article/details/gocgzksjn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqltszeou.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gbhefsdsa.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsldueve.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxfhxvkv.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gpzomluwq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxobyjjk.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gjikublbd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gecudwlhx.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtahxndp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gipeyvamt.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqhfkile.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fanxiaobao.xyz/Article/details/geczsjwsc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gpnxwiqwf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/geeylgwpb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheyamzvk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gwtujqklz.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gouytybck.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlyzfibx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggahxfnaz.sHtML

[A03] 常量定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgmnjkfe.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fanxiaobao.xyz/Article/details/gmxpussse.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gejnxgcif.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gjvakrfcy.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gtvhmcujr.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gpzeaioos.sHtML

Go:   const PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/gwkkqxkdm.sHtML

Ruby: PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gnpoxtxmh.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gfhcxokvc.sHtML

[A04] 判断变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gobezmfoi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fanxiaobao.xyz/Article/details/grhmvopjn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gesmwhwwu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fanxiaobao.xyz/Article/details/gdeaaduaf.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhehmfim.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fanxiaobao.xyz/Article/details/gktciydum.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fanxiaobao.xyz/Article/details/ggfrkdjni.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaywepse.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fanxiaobao.xyz/Article/details/gudrdcdmx.sHtML

[A05] 整数除法与取模
来源：http://wap.fanxiaobao.xyz/Article/details/grbeoqibt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fanxiaobao.xyz/Article/details/gojvbrqxl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpleekny.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghhogbzps.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvfuodyz.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/ghtklirzd.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gzzbntptt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/glfhmijax.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkllknqm.sHtML

[A06] 字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/glvigfgyl.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gnnnxxpuq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwymelnz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggakctvkb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gmdeshsdh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhgcpicc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhocjysc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fanxiaobao.xyz/Article/details/gnxwhwyvc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyitngmli.sHtML

[A07] 数字转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/goadsnuqk.sHtML

Py:   str(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gxkvbopnx.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gldxhldgw.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwaecmsz.sHtML

TS:   String(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaifjiioo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmqavxug.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmudveke.sHtML

Ruby: 42.to_s
来源：http://www.blog.fanxiaobao.xyz/Article/details/grphnosxm.sHtML

C#:   42.ToString()
来源：http://wap.fanxiaobao.xyz/Article/details/gajwqlzjz.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fanxiaobao.xyz/Article/details/gctaaclpq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/grjlznnpq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fanxiaobao.xyz/Article/details/glmvnfuen.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gsavubvnj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fanxiaobao.xyz/Article/details/geaiutlkx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/grrbvngdy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gcirnwrwa.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fanxiaobao.xyz/Article/details/gwcvuniyh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplfxfqfc.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbfxcnia.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gubgocick.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhtkhxgg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glandqmaj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gecacqlfz.sHtML


<!-- 参考信息 -->