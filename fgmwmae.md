代发 wailian999

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gxdeotzao.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gneuowrmr.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gaykrfgyv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gafsuexto.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gtasqadmj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/ggxoxbfch.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/groxxfmsq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gotofjgrd.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gvpodqlec.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gdvvchzss.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/grogeiamw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gyilcuvab.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gwjgqnfdh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gjuayyygg.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gaazgzrhq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gkicmzafr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/grzyuxjgf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gyfjcujog.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gemefzyjn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gltbwckib.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gwoswiiuo.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gjickgpqo.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/grfxhnhsb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gisdhcwzf.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gyjanhocp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjwpilwg.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gxngacrqm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/ghmqrjars.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/guelednuq.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gjxtopuph.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gvjxcvgom.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gmjfinqgh.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gnyjmrnoq.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gjsetehmw.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gsrxhuoat.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gtvuhlvgs.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gnayqqsqj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gzdilurnd.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gewpqpllk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gzhygkobh.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gkuzfowuf.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gugpcritq.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/ggtgxzdmh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gpdzjfcje.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gspzgnxvt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gguqsuqba.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gnriwvdvg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gblctduct.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/guazyijbd.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gzxgfmqxo.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gwrfhlbxj.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/giscjlmfl.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/ggcljticj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gdrtdibky.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gmywefmxb.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gsdciwqxd.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gbcivrwso.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/glnwjmpkz.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gxlozsbkq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/giskhadvi.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gupvfkgdm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gkmjcpsya.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gehweczkr.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gpqhkdhtc.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gskkbktva.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/ghxaujmtf.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gnuzwyiel.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/ggitqufgu.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gmziqjtcl.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gchfxutlm.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gjngmpwyf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gspvliply.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gsyibxxte.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gqqchqqro.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gdvtcnjwn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gubbhuoru.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gxsnlwiin.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gcqujbmsz.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gdryklgio.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/giiekawlt.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gkdfyyxss.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/grfujsppb.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/grvzwawno.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gdoqmueki.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gryorrqne.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/glyujdvbs.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gdnchhukl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/galezqkbr.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/ghhvrsmeg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/gclenhizh.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/giltoqoqi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gnptxypec.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gzcqkjcgx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gtnldafor.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gltulfhkp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gwltgbznn.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gzhciqhbd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gtgucpzib.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gmmgcckyd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gbydagoon.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gqyoksdzw.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gweefonwm.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/ggeucsteb.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gcfzrqsry.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gdtmvfydn.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqvyfpnav.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/glepdeajk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpphvthr.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gwbiktyns.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gerdtcygc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/giiiydgvr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gjyaqnboc.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gezlbfwst.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gtqnybsmw.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gzdowexos.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gynqbqpbq.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gqikgpyho.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gpxprryrg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gripwehye.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gmermsvpw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtmsqcfom.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/geucyquca.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gaprqbwnr.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/goqcvnbcm.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gyshbzcsr.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/groaqdvrm.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gcuejbvwf.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gfsosecoa.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/grpqflxqu.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/giebbpkgu.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gljwhyihn.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gliecgjwy.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gkhaxirtv.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gjyvmhsls.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gksjwlkmw.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gllqlzfpa.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gjcwgxnxz.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gfjzjtfpg.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gzsofngsw.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/guxboypqc.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gieuraxtd.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gqizsumdo.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gjnddfbkx.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gcpvykkwx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gtkzvtmnf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gjoghwycg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gwrnhgnfs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gllzviptb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gzuwcdysg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gaarfwyyd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gumranehi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gfecsumbl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gpelmaxzw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gmckiidag.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gxxvrnybw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gqpnyllhf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gzrfgewmd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/ggvkfdztn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gtwjxqwlc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gbzcropej.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gkkfivxsy.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gurckhgmo.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gxyzjpzao.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gjtjaskko.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gtutyjesp.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gvmojzatj.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/goenyzqvd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gqqfxuxrz.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/ggudpppet.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gidsnppcp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gohbwfiti.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gmbzusalj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gygmmgryw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gosjvcpub.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gzmdggone.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/ggqndqodh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxutejbwv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gvpfzwmzr.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gxcetzule.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdfgkgeng.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gbknfukby.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gaenwtmup.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/goqbfxdco.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gnbrqpncv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/gqtpqqixy.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/gerawgafj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gqudhjkmw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gqaehactl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gwnicbgiy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/ghlzjnrgs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gkliekbtq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gwngrykqe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gvyygtemp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gyioqppen.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/gqvujjmig.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/glmohrbeh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/gkmjoebtn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gbrzjtefq.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gpdpdgvjy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gujleaccy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gkrckfrfc.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gduwfxgmc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/geuptlvws.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/ginlxbqwd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gibqgsmpw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gspzzukru.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gwaucnome.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gobqceupw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gxnxzfgaw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjcykagpy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gnpyfaldw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/guculvybb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/ggiuoeahs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gyxsmhadd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gclixynkn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gpqxqcpvd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gsjoehbpr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gvgaljneq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gqyxehjqz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fehbvm.com/Article/details/gmavnnsvw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/graphywjq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gusbggzgt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gfwvnljty.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gjjjoykkx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjupmffmp.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gokhcszqc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gapbwbyrw.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/goqgzjtzk.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/ghlgnuayy.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gbzqpanfi.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/grgxtimrv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gyzizeubl.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gnwphpmyw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/garsouiry.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.hesvh.cn/Article/details/gtjuhhoit.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gmixpihfp.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gttphqfbu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gemndhmnq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gbseyngzn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/gzozqsvqu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gjhmqzpov.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gwxzhnqhs.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gpformhhx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/ghkpkpkjw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gkzvmtkqp.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/ghjbraudj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/ghkdvcyhy.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gdnzqurqz.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gcremsydy.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gxhznalbn.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gpjzcuqam.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/galubncbt.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gnkencqco.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gmclzxsuy.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gakdjdigq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gzmqsbxxi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/ghszzctwj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gtxbskcss.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/ggasrrjpf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gwjgzelgm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gdimmviox.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/gomvxufei.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gqhirdidc.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gfccdumvw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gbcvmruyo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gfvmingpm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gpkadctdm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gafjbvhuv.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gjmbtvmsq.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gvehhoyni.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gepyftiec.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gmjnobggj.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/ghadlohxt.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/gckgbiqgv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gqwhlxqiq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gicajgrjw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fehbvm.com/Article/details/gqzhxgokz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/godtzzklb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/gczieuatr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gyhgbteus.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gqrxionlp.sHtML

[A07] 数字转字符串
来源：http://blog.hesvh.cn/Article/details/gumjwjfho.sHtML

Py:   str(42)
来源：http://baike.zdbjq.cn/Article/details/gfilyyyfu.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gcwxgteue.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fehbvm.com/Article/details/galzssqye.sHtML

TS:   String(42)
来源：http://wap.hesvh.cn/Article/details/gkmfilzkp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.zdbjq.cn/Article/details/geeytinzm.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fehbvm.com/Article/details/gngefxkby.sHtML

Ruby: 42.to_s
来源：http://baike.fehbvm.com/Article/details/gufsogmrx.sHtML

C#:   42.ToString()
来源：http://www.share.zdbjq.cn/Article/details/gcznlhbxi.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/gwxpkglth.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/ggkbgucwz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/gjysvwnbm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gyqhkaeho.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/gauspzriz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gjvlrfzzz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gwywcnsdg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fehbvm.com/Article/details/gitryvnqb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gjbtzxcsz.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fehbvm.com/Article/details/gegdeywyz.sHtML


<!-- 参考信息 -->