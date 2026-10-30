代发 wailian999

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gyoqpasrw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gvzcyxfhj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gectgacag.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/ggczqbkhd.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gcqibckko.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gfxzwaden.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gdimyftau.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gdhwxwodb.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gfubxnwlt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gqrhxozil.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/geapdqbom.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gynibjnsn.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/govdsxbbv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gwkeynyrl.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gdnllpzle.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gvcwtgjdx.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gdplpoaqx.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gdssrjtnx.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gfbbmwzuv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gyvaywqws.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gkhumocjc.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gzqgntekx.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gmduuzrkk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gmashijjz.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/ghxfgyrjd.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gtplfamnd.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/guhwhyoes.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/galcbvinn.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gdssezngj.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gtmzbmveo.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gqllvqolp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gfhaphxwn.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/guiuyrooz.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gfnizftyb.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gwatkrttu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gpqrywibh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/ggwhvibov.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gjsnrmqku.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gepteeche.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gjpxvvkql.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gzkhzakmu.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gvdfmwtlk.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gzawjmfzn.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gfirqxcwp.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gainutwrf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gervhlvwl.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gvvphvlug.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gkzsuzhdp.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gnzsiwjuf.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gvexyzlep.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gcmpdxayi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gwdwdzkra.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gcburtwoe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gvbutjixl.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gscmkbjlo.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/grjjdjkjo.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdcxtlakx.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gmynsajap.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gfghfivvm.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gzozckerm.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gadayplsx.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gdtxzueaq.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gosvluits.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gxofthftd.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gldwrmoqz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/glyhbsytk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gbiydlsof.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gdkvzrsgm.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/ghletxiks.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gvlwdyzdh.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/ggrcqxlbs.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gvxtwullb.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/guqwcpdnv.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gylrmujed.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/ghumwpfdj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gugpxjdlr.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gpxthdsql.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gphjlpjoq.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gzsbobndk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gyofxellc.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gbrimugwb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gauosfipt.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/ghnocjxoh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gdvslyaux.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gmdmsnvmh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/guounwwcu.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gbkvgvhlm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gjzlnuppl.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gedmuynbe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gmpssjmna.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gfxjwcvwx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gzbjikusj.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/guoyumeiz.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gskwgsuay.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gbeamdefc.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/grhzwntxq.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gybwvuxyk.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gefyjxcpp.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gzrxvhzae.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gujjtezjh.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gzghdeuye.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gnfyqabmc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gzcyjbahg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gbfpmfrlr.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gpkezowpk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/godkogdey.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gautvpzpv.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gbrvsnuee.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gwcvqmaqt.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gfcdukyru.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gbbdylekn.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gstzxzxic.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gppbybtgd.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gzvxajayv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gozttxhxp.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/guwxehjms.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gmyisnqlz.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/giinwnqyu.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gsbtcxnwz.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gsibnxfmj.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gdrhvuhhf.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gjikkljam.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gajgcplqf.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gwhwzbjin.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/ggbpukyvz.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gpmlpvymr.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gyexxelci.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/grpbitjbo.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gkyxlrzrh.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gxixtubqo.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/goqhbihkd.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gocrasgfv.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gugjalgpn.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gpnahatzw.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gpbyfhfgm.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gwrbvdmqq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/grpinpjaz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/ghecngoii.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gblyygfak.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gehvrzbxc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/grxzabfgu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/giializge.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gbrigwmki.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gqtmwhzgz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gzjienvnk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gyzzbcjeh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gqmwiyuyr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gipocwprw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gvhlgzbkk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gwbrntxik.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gjxpmltrh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gzsnrsgoo.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gbfuizyfi.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gshmiicdw.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gbarnzdun.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gkzhaihdc.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gwzxgvvew.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gxioigfxp.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gtqazbnfc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/geioluvrl.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gsfoyicwg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gjvlpshjk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gtdulzxrz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gnudwfxyu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/grlalbfir.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gjjkaisuf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gjdhdceaq.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gwykecirm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkjcgaiwt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gomvhcxgt.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gbaocyhmn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gunkgpoow.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gonlqnacz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/giqqwuovr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gcmjvypjz.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gyzckgeep.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gthjwmmsp.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/ggnvjmwpu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gsumqbvtb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gvsfodljs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gyrmqpjic.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gxrjbnquo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gnhlrftme.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gyqmomxrc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gnhgeghdg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gxkxzvlxa.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/glmbzjmxi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gzerjiofd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gbgtljffd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/guuzbiycy.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gfumoxfut.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gsuzznwsq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gmnxkfuac.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gdgdyjfum.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gmdviactg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/glxxbobaw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/ggjelpqoy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gycodhplm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gfiinyhjf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/gfsmslhvy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnvvvypkd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gtoolzego.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/geyfypfwq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gmhtrmsez.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghdgirzmp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gcrjyrkjx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/ghvphmgnp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gjizsjhna.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gyyuuajuw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gixyiujsv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/godyrspnv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gtyvzxrrz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/gglmarhqu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gnmijrztf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/ggudmphsq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/ggmvbrukk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gshfhsxft.sHtML

A. 基础语法与类型
来源：http://www.m.share.zdbjq.cn/Article/details/guzoulcwv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpcvpyvpl.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/grbkdfnmv.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gngqrocun.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gfeukcnry.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gsqxtvnya.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gwopoqcbu.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gcfxibwaw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gqmzjgolr.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/glglqfwbg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gnwwwljmr.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gnolpdvpl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/gblzdpekg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/gqffiiorh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/guiqzpxyb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gvfdmumwr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gbegxrgbn.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gduuweuzj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gndytrlyk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gtfhedrii.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gkdbtclsz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gbhmjexqw.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gxyjmzdeh.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/guuzljhkp.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gknrejdew.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gbxuzsckp.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gciesdnta.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gbayxqipd.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gkvjurdnc.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gmhjwkgui.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gdwqygggy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fehbvm.com/Article/details/gniovhwxx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gffkjpigp.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gkzsrizmw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gvbjpcoog.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gkkjaxpcl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gsmxjpuao.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gujcvvvdb.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/gczeflkrw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gteqwmaue.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/glhtadiqg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/geuagrssb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/glgzzjrkw.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gfetowlhk.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/groxowkpm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gqrdupzfk.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gzlivkghg.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gsfrzbabk.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gkztzisvu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fehbvm.com/Article/details/gszynebwr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/guxntyitx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gtpadbyhm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gfmoobvht.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/gjmuwuabs.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fehbvm.com/Article/details/gvqhjlvrk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/girwmhrza.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gmmtbosav.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/gatuaqfeo.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fehbvm.com/Article/details/gieuatwjz.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fehbvm.com/Article/details/gkphyduao.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gtgmdktcx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.zdbjq.cn/Article/details/gksflthay.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gpaozsrsy.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gqprdvyep.sHtML

C#:   42.ToString()
来源：http://wap.zdbjq.cn/Article/details/gmzshpebl.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/gsfpoupor.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/giwdpzcur.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/gganyslnt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gclbovemx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.zdbjq.cn/Article/details/gapougpms.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gzbtaqwlk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gftepiovf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/gonobbxmz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gbukkdhye.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gwttvamte.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gcrioqomx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gzixusuik.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gmvgptujr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gqrtaazpp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gmcgmcuad.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.hesvh.cn/Article/details/gwvydfvfw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.hesvh.cn/Article/details/ghdhxqlta.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/grjmyusmd.sHtML


<!-- 参考信息 -->