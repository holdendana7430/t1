代发 wailian999

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gxxhnaxkz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gcbwgggdv.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gojeggpjm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gocbhxpde.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gerioqmle.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gzfxvgztv.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gtnwweqrn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/goezxvidc.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gmndcfkym.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/ghwdxozpg.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gzmhteoyj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gbssrnbwu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gcoiwbrej.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gnghbajjk.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gmqkwgopk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gkmmpqsyy.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gephtcrsa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/ghifzfgzl.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gncdyfpzh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/glgadstoi.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gqimubpdc.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gfljlaont.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gxjcyhgtf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gpczjefij.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gkofmxeoy.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gzhwmspkp.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gjxzlycvj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gejhiflav.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gsnjlwesr.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gzuyorzxk.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gdkqunefv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gcitikxoj.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gkkbucjql.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gcdvsrnyj.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gsbhiyjrg.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gmbcycgrh.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gqanxfpjh.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gxuzncpjo.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gsvoezwan.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gfhnrfkzz.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gtdfisbyq.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gyskdqubf.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/ghtbdnvli.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gzgyyswey.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gshorcugz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gehbsrabm.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gfpvyvdvw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gjdnbexko.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/glgqnxvbs.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gyhkqghrp.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gknwmrgnj.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gkkcomxpa.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gzmlbsxun.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gumjvsbyt.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/grypvzksd.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gtogmilzp.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/geoetjiki.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gccfdvjts.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/glxqzmzoi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/glylduirc.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gqifdgdrs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gmoyddwel.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gtzkxityk.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/grxppilht.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gwgwnzzwf.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/grqabqfgw.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gdrlhmpop.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gphufwxlv.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gdzfdqkqu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gzgszdbup.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gkqeaepjj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gahgzclff.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/ggtkarbhl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gewaklkum.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gxiqcesko.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/guurjaxvs.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gdkqhlzac.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gulsyxodn.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gpwnieido.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gmhoepatp.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gmxyrihzt.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gprrfsgii.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gdyrhirhj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gcthdbczn.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gywyjftex.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gkelkgpgu.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gznxbwmzn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gphbqyxxh.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/guwaiquti.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gcyajigzv.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gxxquxrmv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gqyyadmao.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gjdxmadii.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gjjxclzhm.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gjocygkyi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/ghobwnuok.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gpppdztep.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gppouyqrv.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gdjzedqpr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gjlhdkajp.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gtacxyuop.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gcjhyomfx.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gynajzkvu.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gopdycqje.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gpjkzrrqg.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gaxmcadxw.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gihrbbdha.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gnkjqaday.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/grtefowma.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gjzvpvqwt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gpsvqijxx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gndpjrxth.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/grxuxexjy.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gcsucdcru.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gfaonlutu.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gkoiellko.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/ggjfjpbrq.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gxwlbvylj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gqhgczzhj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/garafkeex.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grdcixuwp.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/glypuwtie.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzryaxfln.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gtkrgxhxv.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gvovraomu.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/guymaffwc.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gwgqgguuo.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gtvzycihr.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gprgjqiel.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gpqmvtgbw.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gbycryoex.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/ggecxakbn.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/grinpvkwx.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gbzrfpjfn.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gzsopzrfg.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/glclfginw.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gsrygghnp.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gxsnkwmdu.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gupqqnvhe.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gbkdabzgv.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gkbcscoit.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gfmrhoukw.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gsmynxsfo.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gsghmtfgm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gddyfialv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/ghjmheosm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gopbkrjyt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gqievweph.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/glhkulees.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gxaruukcp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gjxccqcjn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gavbvzsvl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gblrzovgw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gjpbhfwio.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/glqpohtid.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gvqqfnipi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gnfdlutaa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gzxoudrgc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gjwdfesyv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gbqekylbr.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/ghnnycxnv.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gamvbmfex.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gjpxidcpw.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gtufxcrjj.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/guakzgehv.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/ghkqrserq.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gemqgtyqh.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/geksxedzt.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gsiaceplw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gznzcqydg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/gmzdcgrxw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gtuxdmtst.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gvhgtqcnq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gbwkggkhf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gdqidedhb.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gummlqkke.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giylfjxrz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/ghmdbtwpl.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gkmkqvrvp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkywqoguj.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gxkmgssef.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gduzygtnb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gkoeauejh.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gyksnjkum.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gerruftog.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gfrzhsogr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gcbidkymm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gkylvmbdn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/ghqwwwhhr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/gqasxqldf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/gfuomivph.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gnnqsvawx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gxlsoizoe.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gxqkkivgs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gadbkyjci.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gkgtaulua.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/gpsltxmcc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/gmeuwymsa.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gxekvvetn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gqliuiyud.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gsayyakei.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gxibzrobl.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gobgoqwcy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gkwxjnumq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/glggvcrfc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gjygogpfc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gdfbxfnfi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gdzloojcr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gtojipmpp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gnekuwwhv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gfmbmivlt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gewcxpunj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gwniqqnds.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gtzddoqnh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gfprcgqfs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gaozcocca.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnoilyktv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gsmedgaya.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gufdpwnzm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gstpkkjhy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/gpjzvxamp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/gmvagnlkb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gxiqpenfu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gngdmkemk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmiyprthm.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gqvvqlrsl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gswceiwqo.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gjdqwnhet.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gllqdrtyw.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gchwjvwwb.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/guzssgtzt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/ggcukwnqt.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gwbuxstnd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gchjpgrco.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gspjvcakn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/goznwdelu.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/gcqpvfipa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gdultcgkv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/guhtwilma.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/gdtlwtgth.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/gqzszfziw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/grenvkngw.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gasdmkmdn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/ghytiliyg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gjbrtynkx.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/gmsboyymq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gubywtqqg.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gsykqfnze.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gplibyqnx.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gbzirudod.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gktwvidez.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gdrtykrjj.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gdwczysft.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gsilnswdk.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/glcdtlcwz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/ggjrsxxvy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.zdbjq.cn/Article/details/gfdvtdcyx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/ggubbjbgn.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/grzsubqgp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gnyfdbqzx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gjyavnswm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fehbvm.com/Article/details/gyrstjlsw.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/gxjnwzrmu.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gyfolvcds.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/glodhiiot.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gawohuuus.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gavlrdsov.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gthobjghk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gzmgcfnck.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gbtcbtgvn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/giyckbymq.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gwxtyslss.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gchdabjbq.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gpatxnvwj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.zdbjq.cn/Article/details/gqxdvduwq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gayxixfqp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gizdjqgyo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/gdvfgpsgy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gpzqbdfxm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.hesvh.cn/Article/details/gbkyivihk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gfrgdodna.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/gzmasaeou.sHtML

Py:   str(42)
来源：http://baike.zdbjq.cn/Article/details/ggtdozeeg.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gwznjtqks.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gbpixpsui.sHtML

TS:   String(42)
来源：http://wap.fehbvm.com/Article/details/gdvawmgpy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gtyiapbjd.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/grqgsbljd.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/gtxfygpab.sHtML

C#:   42.ToString()
来源：http://baike.fehbvm.com/Article/details/glowpbsbc.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/glrulvrbb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gwurufkdg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gdfjxliyy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gbbtaziyn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.zdbjq.cn/Article/details/gernlizby.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gxgnmvsjd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gysuqroux.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.zdbjq.cn/Article/details/gxqyrmsqq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gtvfkszas.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gaasflwuo.sHtML


<!-- 参考信息 -->