代发 wailian999

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnxqhuqf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwdpornv.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpbqnasc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gokytxfvj.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gnmlphysx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/grylcnjrl.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gnannqria.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gpoyhnxec.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkoaidqs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynpcjscv.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gltapxxaa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwjbquxn.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gicmrknbq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmypoqgev.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gbllcicvx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gfrtyksyv.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gvtiwdndi.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gjuafdfdi.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzzmkjen.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/ggnkxxzuv.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gaubcvclj.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/goxmhfyka.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbzsuchy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmexfyuc.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gdevxisae.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gsujognub.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/glpcujgkp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaclldjz.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gzfkagflk.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/grnsfqejt.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnizedjo.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzsgrubt.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gndhpemhn.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/glyqzwazr.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/ghhayjsdx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gplbsvfvf.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gahhjriul.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkzckesu.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigahtamr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gohnyvwix.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/goiuphizh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkyssybi.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/grjijdzts.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/gknykuilp.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/glwembbgp.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gykwxbsly.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gbuftgtkq.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gpxwoxcqf.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/glddqvjnm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnkvjgjk.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gdvvbokzx.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsgbsofm.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gunfmmdne.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gamkqeckj.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoyildnj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gdmcgpaks.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ggspwxleo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/glpoxqmpx.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoeuanof.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzpahaxg.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtomzivm.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/gukirchcz.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzxrlgoua.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadjnitfk.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsarunzx.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrjdwhvb.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gmsdezhnu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfvatfbn.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzctmxqo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gsyryceju.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/grjwkacym.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllbotoyc.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdumfrbuh.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gbleghooe.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gsizmyqok.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyejbrst.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gxadxbaip.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnteocsp.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcpdmlzi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhdquktn.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gscjlivjl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqpoqfte.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwmzgrer.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzxvzpsz.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavxuzuwa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuimdpwz.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gponbpluq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gyelvplxj.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmumqibq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxynhpsu.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtskxeccl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gtdbbwpfb.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapmomgdj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gchkfqbhj.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gphnooyig.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvgwftfo.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktiakoer.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gumdzpeob.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvghunvo.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gocfkhaby.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvccznss.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/getyvyoma.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpjejrwi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/goqpluabu.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gydirioxr.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiimtsmx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkjrymbn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckyeskpw.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/girzhswdf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaefhevz.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/gnjamwjnz.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjymmroz.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gidsjnexv.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gfazaifwb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzgilcsq.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gonxyxalx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvksdxcwd.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gxccrvdsi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gifoeasyb.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/glcpwjlji.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gcqcjajvq.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gbutttywq.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwgmhryh.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gktqugknl.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gmfwtkgxg.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjssrbnfk.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gysxijavw.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/grydytqqu.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gbivxaude.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/grolwkhoz.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gogppnnbl.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gdvlbpnna.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gjaefnqqx.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gticmezbw.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gilnmfhws.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gqtrozliy.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/glsxchksm.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gatfowqws.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiecoqqc.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gcazpupvu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gshkrpkku.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gfopebxos.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzrgcxyh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gqlgslkdk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gamktcmcl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gvrpcnybr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gbscfbjqn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gemjlmblp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqnkstqy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gswghseci.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gtcohyoks.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gjncalszd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gashvhuai.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeyocpra.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyeqbnxb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gvasfohlo.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsclhzfjv.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gyamxxfos.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gwqegkzwi.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlsjrejp.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdtsercb.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gwjiztdbi.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/givcavxzb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/grzahcfel.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/girfvgybr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gcqoqrxbd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fanxiaobao.xyz/Article/details/glivadalq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gmkyhmvos.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gcsfuayrt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpkbgpjq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gtndhkdmj.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gheybdbfy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/goinkbqat.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcndlwpqs.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gridoghyh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghbkqwbei.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtnoiqrt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fanxiaobao.xyz/Article/details/gsylrogqa.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkzrcaar.sHtML

SQL · Bash · C · C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfnslkia.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gukhydyhj.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukyueiaz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gkclfxppj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgfqpkff.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/gvbgxjhnl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gobeqwbzo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gixcprlrp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/guqwiwilz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcwgukot.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjivwmbcs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fanxiaobao.xyz/Article/details/gehudrflg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fanxiaobao.xyz/Article/details/gsxijyhdh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfpeylaj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fanxiaobao.xyz/Article/details/gimjchuhy.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gnisrermv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fanxiaobao.xyz/Article/details/girfqkait.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbghgsxzl.sHtML

目  录
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlemopgl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gwkmuefgj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gekfyfdnu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/glfiycvnq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/greplzdoh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsficxyb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gitrxbnhv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrmlarsl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/goqkvkesk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjssnjhjx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gbsrsbuzc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gagikinsy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkslwvouh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gerolwwes.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnzyvjua.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfuahwsk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gyghdjwgh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gnjwnnytm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gbfskxlcg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gdwnqcluq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzcfaquq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gqyegxahq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gbvmvqlca.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gamguwqvz.sHtML

A. 基础语法与类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfqnlwsk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxijujwdg.sHtML

[A01] Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqbxnonl.sHtML

Py:   print("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gkioxovte.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fanxiaobao.xyz/Article/details/gwpcoyeib.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gokjscfer.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjgrompy.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtmmrdql.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghouqblhx.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsyhcspj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gikoiqgnf.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugugftsk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjzqopcu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/glwrkajne.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gwudgoyqn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmbgolhy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/ghkhwtuad.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/genwaafxj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gmghhvlsw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gccvjqgav.sHtML

[A03] 常量定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzckdrcv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdysksmdq.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvlfgbsa.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfzxxxad.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gtmovsfar.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gpzwwphsc.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfgnoygp.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrcxstma.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxhqzfzx.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gcvmlqlom.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbyumuie.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fanxiaobao.xyz/Article/details/glhcpjdtf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrhnfxxc.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/gywbivftg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrucokou.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fanxiaobao.xyz/Article/details/gadbtgfez.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fanxiaobao.xyz/Article/details/gvjtkmkfc.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fanxiaobao.xyz/Article/details/gghqawbzx.sHtML

[A05] 整数除法与取模
来源：http://mobile.fanxiaobao.xyz/Article/details/gglsrrzam.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fanxiaobao.xyz/Article/details/glrivcqcx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwzwpqnsx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmbgxvqy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyfebstx.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gndyxnrqc.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfdadjve.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gktvamrbi.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/ggisdfepa.sHtML

[A06] 字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfknzavs.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpbfhdyq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gdsioytbi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbxvjfkb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gpnkwbkam.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckqxnqtr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fanxiaobao.xyz/Article/details/gcbvqqzhc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fanxiaobao.xyz/Article/details/geafgzuyf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/guvzlpieg.sHtML

[A07] 数字转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gdjickefi.sHtML

Py:   str(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkoenidt.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkpkbwpd.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gjmlhkdfe.sHtML

TS:   String(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmbitwek.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gchwzmgrs.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gfyuhemqp.sHtML

Ruby: 42.to_s
来源：http://baike.fanxiaobao.xyz/Article/details/gewzgeqph.sHtML

C#:   42.ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpetwayv.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzefubvt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/goyoqvtaz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedktruvo.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfspwhta.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gshlefzvz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gxoazfrra.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqglyrbxz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fanxiaobao.xyz/Article/details/gtgxljymy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gfhdttjqs.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbddsptds.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtedmtta.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfjcdpht.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyuicxcx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gxickhnku.sHtML


<!-- 参考信息 -->