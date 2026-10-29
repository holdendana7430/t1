代发 wailian999

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gsnetmoav.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gbzhkawrb.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gnjesvfuk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gezqlxwmm.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gvvwieodv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gupauhqxm.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/ghgcnzjda.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gnbpumpmi.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gotovoqxv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gpgduqddo.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gtgytzjal.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gkgynveuo.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gfworktnv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/goyjmyyff.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gzvcnbztx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gdzlfopyy.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gmabjetpm.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gtpaalwpw.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gskbciypr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gbbquitwh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/grchpppoj.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gbdacqxpo.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gzccrbnea.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/ggfozptmu.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gsxzcswlb.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/ghwdbaexz.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gbaydlncy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gokbnhhty.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gqwexpgkd.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gvkpnutzf.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/glyqedzof.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gvtvpdkjg.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gmwgmfxes.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gvwzvvclk.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/guqgvgwwk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gdvfkekga.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gzcapheso.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gvoudiehr.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gzaqwvymb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gpystdyxe.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/glxweoqrw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gprleawoi.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gmcabardf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gimomapyc.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gdkgjzqzm.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gfofqgpcb.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/guvzdhmbw.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gaytijkyt.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/grnkdrdbi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gkzolohms.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gqxkiuvfe.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/ghpidsvxk.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gzawkknel.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gnhgwitfh.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/guigyjixj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/ghquwadzg.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/geswyxfih.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gottklhhh.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gfbmfqsxf.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gjqnduwbe.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gqmulwdbq.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gjtslrzrs.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gnvliyrmp.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gxbemvifj.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gasauetwz.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gecqyzeoa.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gkuadvvzd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqwnhmzuy.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gkefbspye.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gtbyqayfp.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gvbuggzsg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gzdjpurar.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gqunlmlqz.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gpwvffiro.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gagrbfphy.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gfgtwpiox.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gojhffaif.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gspkbgksh.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/ggnydferm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gepeupzgm.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/geojkuzsd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/ghdyiuxng.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gqgitsgba.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gobgfdswo.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gzqpjjkct.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/ggnpqqlat.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gxjezknqf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/ggfrzrwax.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gawdudsin.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gnjrwzhoz.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gpewusurr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gjonyisvm.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gfigellpv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gzifojlxu.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gmjpswcuo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gyfanlxxu.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gsporkidw.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gykchghth.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gfbwsmgwc.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/ggognjvnl.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gwycgpdau.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gatbpcyrx.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gwaalynuf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gkmvfzpqi.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gpuldcgxb.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gfjanprlo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gsifpqgst.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpijutued.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gvjbpjmmq.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gsnewimuo.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gtvxwawvl.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gieumkwuk.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gbbdmyyyg.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/godvbmmkk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gjrxipuxe.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gahnempgt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxjfuplde.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/ggrevbbgq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnosrkpuo.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gahywvfho.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gzkhbtnyg.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gtbiijmnt.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gpevqmivi.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/ghydgbwfz.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gjdhplcjw.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gssomhcyx.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/glfxmqbxr.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/ghbyfbyxj.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gztvhqqvs.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/ggjwubkjv.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/ggxzoinmo.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gbrumkuyf.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/govvikamw.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gumlvdkgf.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gsmhoiuat.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gdyrfjhwr.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gzfmbaqzg.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gjotytwkx.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gntglrnbi.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gzfnamlas.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gnduwmzbw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/ggiubbemn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gzbucnwtm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gsamwsnup.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/grodcrsnt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/ghzfwjbnr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gmbuibjll.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/glslbmjyn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gyjrinkol.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/glleyeqjq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gmlakomfa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/ghcqlknto.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gbpjgkicb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gvuebblfi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gzzeftawi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gfodqgsfm.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gyxlabjya.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gjywviyrj.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gcvdujuyj.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gabiybwxn.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/giukrlmgg.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/glbznztyr.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/glavlrbhf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gkwppanmc.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gpkdmmbjx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/ggsztewxd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/ghtgfwopz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/ggffmipex.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gbskekhtb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gfrfjgpnl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.zdbjq.cn/Article/details/gfgnfantd.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gqqfkzybi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goictqafp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/guqjygdxs.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gfndjsidb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggwnlcgpb.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gqevcowjr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/grholtqfz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gttvnfrtp.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gucojxjwg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gyabccbgt.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gavfsgbkf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gzhfyxqqc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/gbuqioqrc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gflhquweb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gipoywdkp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/goyxmwxre.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gxkgebeag.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gljsgjkkr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gwugfyaao.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/grdwvsahy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gugawckts.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gwbqowbdh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gbziznleu.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gdozrindo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gnlxqbqps.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gtbtofxzq.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/grlddajsl.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gicfaonzd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gntkkqwhq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gjhtyqvyg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/giwllgrmi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gtvtugzox.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gqcilyzuo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzjvxirbk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/glqgoqegq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gmyriqygq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gugmdfzal.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gqzhhwclt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/giodlenjg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gkhwzjnlz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gewjhkomj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gucdfbfbu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gxvfyzvbt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gloqezjsl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gmobvozkd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gxfsgmomo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gpmxthbir.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gngfjbiec.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gtddwwpgf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gphkegoyq.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gtbnmuhkc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqbejdfnq.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/goqrctvkg.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gwrdemngv.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gxvbumaiu.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gjxqdrxqk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gkjaavgss.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gqrknurun.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/griogbqfk.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gnfzejnza.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/grkuntqls.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gzwrwbwav.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/ggqqcyvag.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gdlukzenz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gsgutkvsl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gxpgvixqf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gfxrpxjyp.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gnqwegzzb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/ggmtxtgji.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gbppiyffo.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gtukolhfk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gbzycftzx.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gxccphpik.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gpklxhyqg.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gqqpjelbc.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/geexelnmm.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gaglhlldu.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gmvdemoqn.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gfcwszoas.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gdlxuapqp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gwngmpone.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gcapwjpdp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gsemdzvwo.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gieyxzequ.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.hesvh.cn/Article/details/ghkntabdw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.zdbjq.cn/Article/details/gkilewtjx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/ghhovilsd.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gcbcnegpm.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.zdbjq.cn/Article/details/guzlxfewq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/gducgsutx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gshwsmxfu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/guolkdauc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gzggylfrc.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gbxvrzgoh.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/glsexegni.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gbvoavxkn.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/grfkclznx.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/ghwnjdrpk.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/glmprahin.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.zdbjq.cn/Article/details/gmflpkzpd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gjxkjgfxd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gatyficte.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gbcomyknh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/geddbvsqd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/gvbxsdzzi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/ghuxwscqv.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gkgxdpbfo.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gvdccvkzy.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fehbvm.com/Article/details/gaiivgrnw.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/guynnwyfn.sHtML

TS:   String(42)
来源：http://www.blog.zdbjq.cn/Article/details/gvmxgyyuq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/giaqldyct.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.zdbjq.cn/Article/details/gpjxvhotw.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/ghwykswiw.sHtML

C#:   42.ToString()
来源：http://www.blog.fehbvm.com/Article/details/gyjtwubjh.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/gkcziuzpo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gvehdzvcu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/gyiszbzko.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gdhwihhnk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.hesvh.cn/Article/details/gpzmrnzeh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gnwcbhiby.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gskukyhsu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/gyobuxzoe.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gmitihjax.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/ghggvollz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gewzjjjng.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gzxwnxmqx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gtjgrjvus.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/georndwlm.sHtML


<!-- 参考信息 -->