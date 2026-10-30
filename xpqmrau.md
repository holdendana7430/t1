代发 wailian999

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/galantsfb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gbxgsqymk.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gizvpeqay.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gjzcrvjwc.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gxplgmtds.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/ghubppjpr.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gftvpalnz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gverdwvpd.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gdlqwzfvv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gqxjloehp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/glxksxnyp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gpruyssty.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gtawrdfri.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gmdyzpwkc.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/glvhjcvms.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gjjwqorgv.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gjsqdyfav.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gcrtbvjyo.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gthijtmqx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/ggtpvcpqe.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gwtuahwan.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gmelupzdx.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gqwfdsbma.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gtknqotvj.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gcvhktsbh.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/guvlnfycb.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gatqjnnwi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gohcxdpfm.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gnyzkiexn.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gqktfoday.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gcbjmuswq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gyxbymzrt.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/ghtmmzuac.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gfjndksgq.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gezdscfjl.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gsnuajnre.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gszbrvjbg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gkkhlrfgc.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gvstjchwy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gyzwpwgvv.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gxkmwwxwf.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gkewkkocb.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gzqvplaxk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/ghmmrklyf.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/guljhyovx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/ghulavvxg.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gsgtkwnut.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gdkgxxxgn.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gygnublvq.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gbdrgzdpo.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/glkoyvpbs.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gninlnmrr.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gbukrpcfj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gzdpmkbnw.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gjacbbctj.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/guxwfosjj.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gatswcawx.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/grbtusfsr.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gcuuclxua.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gwbhyuhqr.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gspamnulh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gngzkmibz.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gztwzgrpn.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqjgssjsv.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gjydwzdsk.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gjqqpgonp.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gxlckjhmr.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gvjcjvkkk.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gbepskyll.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gqlitoklz.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gmxrsoouo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gxmoyznrc.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/ganrtonsk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gbzxxgpae.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gfcappbjh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gackmnkya.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gcmfhgnue.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gtkdlwtub.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gkulzrbbd.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gzontajxd.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/ghpnpoxud.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gyxnjmmei.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gblhggfbf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gaegragjx.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gvqdakcpp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/ghcsldxgb.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/ghxrwdzln.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gjxamimho.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gkinainoc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gvluzgftd.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gekfdxhfu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gwkrsnvfa.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gaetjbyok.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gzrdakjaa.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gpnovlbpo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gbxkrnthe.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gguvqnnab.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/geingvpss.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gcypqfycm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gxqqgdlip.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/glwoiwhqk.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/glcmkuhtm.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gyfbegdzr.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gpjvbjyqu.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/geclembmy.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gabuqpypl.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gimsnkysa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/ggronkqfe.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gshdkmwzh.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gwhmfjnsf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gorixgado.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/goevwfjkn.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gxwazlzsf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gojgqyeox.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/ghtlwhacw.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gnctncurj.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/ggngyfsyh.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gwtizcipx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/grqmrtala.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gvuhkkvnr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gauxiyuwc.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gxzbxkdni.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ginyoptzp.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/glsmxbgat.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gpubsbusy.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gcvoactyh.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gyxngeabe.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gomqngbov.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gbpeixnub.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gvcxonmbu.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/grbtnkawe.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gakjzctnm.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gdzmeoqru.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gggkblouy.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gcgxanalu.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gupyhyqyg.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gaaxhbgso.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gqnbxhlsw.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gsnewlmkg.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gqtsrgkna.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/ggudoucnx.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gglxxxqjr.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gghsfpvwq.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gqzgiqjke.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/ggpsnosij.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gdnfzkxwh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gotpfdckw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gwmofyoce.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/garotkgnu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gitlrgaog.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/ghxpcrbin.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gxrlgjmcv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gqjqflftt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gpzwgcjbu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gpqnbfvag.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/ghobsvjla.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gndlxgcfv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gasqarjth.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gmzqbfyqe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gmprbwuqs.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gtsofbchy.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gqbswwnqs.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gfpafmzmu.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/geiidhfgf.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gzddczwhp.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gkeyyscvf.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gyervitvf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gofuzgpqk.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/grmthchrh.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gjjpywdzv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/ginvrckwe.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gplwrvgur.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gqjgfiwzj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gmthszvay.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gganmfjdq.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/ghycbqeto.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmvwlirpd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gwjbqmoan.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gbzjtqnbp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grvtgaafo.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gugzanman.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/grbnbuxjp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gmotjghex.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gpchxbshb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gzkvelvav.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gtslepiwu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gvdukvapi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gsaoupcea.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/gqzsidyka.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gecybzqwj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gjixqaxot.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gjsitgtxl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gxbwpjrqw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gefcjbads.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/grukuzutk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.hesvh.cn/Article/details/gqspslstx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/gvkjzbvrs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gohbbiksr.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/glvrkliyb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gpnlqtmce.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gzlqwsmpd.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/giavcscwc.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/geswmciwr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/godnxhqmb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gbneyzajf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gygznqfkr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gglipllvf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gmqpnynmt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gdotbvnta.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gfthvwgcx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/grgtjkvsf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gjdjugmju.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/ggbegcwoe.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/giytybuoh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gdxzzkxmn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gphcaamqu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gyywoidof.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/garpyhvea.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gthfjndix.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gmuyvswon.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpnvxzskr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gvinjxisx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gybztfjqn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gslfqiblk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbrtqmrif.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/ggswvuxym.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gklpvuqde.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gwgftmurb.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gmsrziakt.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gffgdlzjn.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gidaakidl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gjafraxie.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gmfgcfrbk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gsmkigcks.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gldyendwh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gqwphsdrq.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/ggmrtokgi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/ghtlglprk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gvgueujww.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gkngodhbd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gyifygiyw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/glljqczgt.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/geuephzzk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gqnirmukl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gvylxdppr.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/ghrfwywup.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/ggaglhvpb.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/grklcpopm.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gebqonukr.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gittfezfs.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gshdycrya.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gowiazkwc.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gqvaicqkk.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gsqvwxopc.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gorrgsxlk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gjzdxrctw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fehbvm.com/Article/details/gnznyebbk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/goiviekah.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gnqaccaic.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/gbztffzqt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/ganjlttfg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.hesvh.cn/Article/details/gzayjbhnl.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gvjmnhkcy.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/geiclwkzy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/gksmyyjpc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gwzyemspr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gvfqxxpic.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gsjlgzzwc.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gdlyhbold.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gdzvuiqpl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gtblamgye.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gfxbrnurm.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gixzbsnop.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/gahsaqdwl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gjehxjfxf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gijvrvyza.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/gnoynzdkn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gunxlpnpq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.zdbjq.cn/Article/details/gsasjbuic.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gfboagjxe.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.hesvh.cn/Article/details/gvikjlpjc.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gvjcjcnlg.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gnuihfnbg.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.zdbjq.cn/Article/details/gpteajumn.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gifmnbffq.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/gqfkwfcml.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/godcvyukr.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/ggmppypcx.sHtML

Ruby: 42.to_s
来源：http://3g.hesvh.cn/Article/details/gfekslsye.sHtML

C#:   42.ToString()
来源：http://read.share.zdbjq.cn/Article/details/gmglxttfj.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/gitabacpp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gbosvevvu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/gsywyxyix.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/ghnklzsgs.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.hesvh.cn/Article/details/gvzispwta.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gzjxwgyrp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/graghrxwl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.hesvh.cn/Article/details/gkoetulit.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gsvnsabjf.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/gpqlneguu.sHtML


<!-- 参考信息 -->