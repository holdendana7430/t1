代发 wailian999

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/graeaefuk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gjdwhgtjm.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwizwczfu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/grdmizwth.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuuiyviu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gvxihupxg.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqmrtrjf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gvrnbymvk.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhnmljgv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/ggwsrcpnz.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gdelwvtju.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrdfitng.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gmqkyenld.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/ghjerkdtv.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutqcuwak.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gwvqkwdww.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gdfuumvmv.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/glsrbkvkc.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/ghnsocazq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gmiqbaurs.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gzrocebbb.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/grvjscoom.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuehfciw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjdllawx.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrpaflup.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gynyteqvy.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/getszogrt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbhsthut.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/grqeqpfto.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/glvuuexwd.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/girotsyva.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/ggwuhogjj.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeonttbg.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyppxugd.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnuedjmh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gjfycjlez.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/goupyktln.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gubwapeak.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaayepze.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gwjertyqu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydhryozi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowazauoc.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gkulnzszj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzwohahk.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyqfnoqb.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhxispvc.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbzivqgj.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gmazducbi.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/ghrvgfwxz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gqdzrlgey.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnxcpcuo.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdwsfvxh.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuxxcgda.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gmhojlctg.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gmernrrwc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gebexmsrw.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gbvclgbtv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgsaxvid.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gbilcrhbc.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhckdzoa.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gohekogvq.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnwzzzip.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcevrgnsv.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grodvuhpm.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gyabicgff.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gdikugunc.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gedryeuru.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gggbhwluz.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkbfgssy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaezwayw.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnhqyqco.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gldefnong.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjbszsfw.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gdnzszvoi.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcxcoibw.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxcxieet.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqaxwugy.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/grzydtjys.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfbboqmd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwewxsdhx.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpvgrqwp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvlzykxs.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/grvzobmje.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gyopmuaae.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gnpfjplqk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqskoicj.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/ggknhyabo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gtvtaqhan.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvezvuyb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxehnvuhn.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjbcwmyd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gloiacmre.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwleqnoi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geahihwrd.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiotowuz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgpgcrkf.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoivfuqb.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtajsjxx.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfoewjvt.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gznnpgoif.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gsweqamfw.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gfzrirzjf.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/guozlxuiy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gumikqxjj.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvuoexmm.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdftmtsj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/glqkjxnig.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcrytgfx.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqvcmvct.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/guzqnehsa.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhdezqoq.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsktzjrl.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyiqraxf.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/guaulcsre.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gadheknat.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjqnxvtq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsapcceif.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gtppkixok.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grotwysld.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/geizhxpld.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/galfifvub.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/giiftwjwp.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgfhvtlz.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gxkmjhnjz.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gepxuhrjg.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwgtxlto.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxhbzyls.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gxvfwyruw.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gauynzikp.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvwcobae.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gpniaphfh.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gwwatkaau.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gusexzhfx.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnosurhba.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjcradeg.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gktqteuup.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/ggszlazzl.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/grfigezqt.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gynwuvzzm.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gegcnivkl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gxjrxcjjg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gmnjnoeav.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gepfvxxai.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpdozpvl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnadjnrha.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpcipzqn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbfijnsm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/ghqjtyaha.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gofiahyfm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunpvckod.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxbeljwb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/grokuhmvk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnauidpwr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gbhcyrdde.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/ghprurcwe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxncvvuf.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gtxyhlbpb.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyakiwqa.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gkxilkzrf.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gtmozpsxy.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gocltumxk.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gqoljhkak.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/guhouyiyy.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gztaobczs.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvfqibrc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblxwlqwn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggehvtqtq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbjaugrb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/gucvgcgso.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/ghxgugiyn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtbszfyg.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gmrjqlvff.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvtkcdju.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyigrgfrs.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/gfofriuux.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gydftmblu.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeqlwdlh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiezzply.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gkzndwfde.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmvibzze.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjatiexhk.sHtML

【使用说明】
来源：http://wap.fanxiaobao.xyz/Article/details/gyqipdwgy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gdpdyyxcv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzrhymjl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/gcmwvdghb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasnqivsm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpsfnkmz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/gnlmkchay.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjtvjeup.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gibffflza.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fanxiaobao.xyz/Article/details/gsrfswhch.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqniiace.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaewbdak.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gzerlyxgp.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/girczttuh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fanxiaobao.xyz/Article/details/glsrizhgm.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gmnaufhvy.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/grqatsyrr.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaofwofh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnhqlneu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksgkoxul.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqspxzmz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjhwaxxq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gwxkgjjmi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gwcyvqhiy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbhojkoy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzvptpxv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gaonhtyuz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnwkybep.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjhzkgeq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gszoegwoi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrnoosyh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/guibpfutu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gaygastic.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzrqeqzee.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fanxiaobao.xyz/Article/details/girwiczka.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gctpssgvc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gpogctfyq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gprtijqwu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmwswzcs.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcekehgss.sHtML

A. 基础语法与类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gonluuqxb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgqdleez.sHtML

[A01] Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbpnyrmw.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/grhfsczzj.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqpuhdzx.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gschlfltl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/gunqvgrea.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnrgrnsd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxzuoddu.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbvhdaok.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gkwdoaykp.sHtML

[A02] 变量声明与赋值
来源：http://baike.fanxiaobao.xyz/Article/details/gqzpmgkof.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtulfgjs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefjuezac.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggilhibqx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpczfipzn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gyapunffb.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fanxiaobao.xyz/Article/details/gvbepasrm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fanxiaobao.xyz/Article/details/glslecsyt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkzjwzym.sHtML

[A03] 常量定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaclixdf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdinmfjg.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gibfomxqh.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvhjayyg.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gftuvkgkh.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkrhrvig.sHtML

Go:   const PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/gowwbqfes.sHtML

Ruby: PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/gjdfaiddj.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvixleeq.sHtML

[A04] 判断变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/grxfopbfb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fanxiaobao.xyz/Article/details/gzczwgzat.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphgnbiqu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gkcbbmamu.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbqanoug.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fanxiaobao.xyz/Article/details/gzewreztt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fanxiaobao.xyz/Article/details/gmcioctsg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fanxiaobao.xyz/Article/details/ghviqswkd.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fanxiaobao.xyz/Article/details/gygbtkzle.sHtML

[A05] 整数除法与取模
来源：http://blog.fanxiaobao.xyz/Article/details/gocvbtdaa.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlfbihxa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkyxmqma.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoksokqx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gnxkeyolc.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxksnpqu.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwqszdyz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxayubzpq.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gxstuuzrq.sHtML

[A06] 字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhwenwcp.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/ganougism.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gnrmnaiza.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gndzspcvt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gdsnmafhn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/godkhnibq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fanxiaobao.xyz/Article/details/gxnlizizk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsijrexm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gsxkcllgk.sHtML

[A07] 数字转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gkyunilpd.sHtML

Py:   str(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gqhdanhmg.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gpirtpvzf.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gomsikxgu.sHtML

TS:   String(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gvrzgyxpb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gsdoitlkn.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gixswwpvb.sHtML

Ruby: 42.to_s
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnhtsdwh.sHtML

C#:   42.ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjuopssv.sHtML

[A08] 取整与四舍五入
来源：http://blog.fanxiaobao.xyz/Article/details/gqnrxirwk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjoqkpig.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkyjyurbo.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gkbjnmoea.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiobdgae.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/grcrcevwo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/glyrfkznw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcrbbays.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gmzomgqyx.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvncttnye.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/govxgzfro.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/geystqeff.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgbghzgy.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyoyfiiw.sHtML


<!-- 参考信息 -->