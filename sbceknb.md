代发 wailian999

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gmeaeqmro.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gucsbhvik.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gaavjoqll.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/glpnadbdk.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gwnwguatj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/ghpxplazt.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gffbttdgc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gakzmpmak.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gonrsnmig.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gbwabzsfm.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gjvytenut.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gvergejxo.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gwtolzmrf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/glblczmot.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gfyoyfqvl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/geuiyriwf.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gdrszldhf.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/ggdhbftia.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/geenaujnv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gtyychsqv.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gymxdpkyi.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gyesyglls.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gvijxfhcg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gnhjmbalo.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gooafojxi.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/glarocvxo.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/ggixnjzrp.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gqinucavj.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gopwwklbl.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gptrvakew.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gjgmxmoms.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/ghxtxaagl.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gnpgtqcua.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/grtpiznvr.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gulawxmnt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/grftnqjdx.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gekydmmwn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gileudsdd.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gftakavzc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gmlmnpdfu.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gpeciuljg.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gvyjsmklu.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gapeqejag.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gwyarzvwt.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/glvnapxns.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gsramtxpl.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gjkawwedt.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gonwjocye.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gislyygmm.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gpdnthwon.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gvfqiurih.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gvrxmkksa.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gqhxhayod.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gpdkqrngw.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gdshklyys.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gmtdtwcal.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gramlsnbc.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gilyypemy.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gtxpzwwyj.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gtrbglvze.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gpljdtiby.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/grfwjgbqb.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gjqrsbdkv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/grizjyjhk.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gxgvhklei.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gknqhuihw.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gskqmztpz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gufdqjhap.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gjicouhze.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gqlqehjnv.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/giapttwui.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gwvcvsgtb.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/ghxjtpmui.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gemphwjol.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gxothgmpq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gxuzunqcg.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gfsnikqgk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gexgjyzzt.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/glhsujvyd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/glqrmxead.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gpmesdrve.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gvdpkoqmc.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/glyaydaha.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gxzvvzxzv.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/grcbtrwfq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/guiqmkejr.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gfpwnlpus.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gbqjdjcpg.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gygpngbed.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gxoxrdrhs.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gbjyuotdq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gbfgudtbo.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gzpytbuks.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gihbcmrrw.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/galnikteu.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gbvvejepk.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gtangqnpc.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjxpjnvnu.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/ggtjydmmi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gwsuixcir.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gkdyhpfvc.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gxlrohcjx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gwouyrzpz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gutscdydn.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gedryozxb.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gkfjyhpqa.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gaolgdcmx.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gxgxfacgj.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gtyipgvtd.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gveehnove.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/guekoagqp.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/glbluhlki.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geyblzzic.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gvaeukuei.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geockrzbs.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gjrqjdrfm.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gmllwbzex.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gvqdzzdsf.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/guenlbnzb.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gnjoiuuba.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gosepbcuz.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/ganxxjojy.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/ghplenmac.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gkaneffkl.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/geewhadzm.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gyjkadsqn.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/guyupwqlz.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gezkgnwaa.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/ghyswxjki.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gqsoiamtd.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/geqelvexp.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gpddgbdiz.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gnhbigker.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gvppmvucg.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/guozatzgw.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gctzmfbbx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gqpezkyvk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gpydqozyc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/ghtsqqvae.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gqfgouatx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gfjawrquv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gjrzvfshe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gfeuviafx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/grwlxbmiu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gojodzzzy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gsozssmok.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gmfdakhaq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gryjugppw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gqaasqsqe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gjolgzucl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gntdinyew.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gmmboamdg.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gpsjelhjx.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gheqywfhq.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gdqvvsecc.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gsovqwnkb.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gtrgtwyur.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/glevrpnkq.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/gtybttmyz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/glfeairgd.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gbsquyfpu.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/ggegthcft.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/ghsdiicrh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gylpjgbcs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gfrmpeqmx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gxgzjaxob.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gxnpmejas.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gexyahdcb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcamsppdd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gjdohzjqq.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gmoieafdg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnwljwtuq.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gatahugrh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gqelmzzwu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/gygrobaap.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gjjphysfs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/ghqjbelsj.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gqvkeykxc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/ghdmnnalg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gfrbvplpn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gyossavpc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/geweofvmd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gbpmdmcvp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/goutrnbxp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gzbuxiuhb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/ghvndkrza.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/ggcztjpfe.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gtdlrcerl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gpsfbczpw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fehbvm.com/Article/details/grhdpyytt.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gbvtrmlsq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gtyuogluk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gtvedabbc.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gygikfydc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gslodlczh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gfyzrtygo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gfmemqfqv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gdfdbzygm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gcqyemppc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gpjnkhozk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbwprhyga.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gpvdnnypk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/grbglyrer.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbaitoigd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/geuxckjtg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gpxhyncuv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gyqsisjwz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gmlcecrti.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gdeychors.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/ggagmiwsa.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gmakrsbnl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gauqmtgbp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gujzyexlx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/grlzyhlvi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gxdgthjci.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gnxgnfsis.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqrotjqqa.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/gzcyvijld.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdlgftirk.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gnpazsili.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/growjutol.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gwzihgjdf.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gujwrbaux.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gjdxyhzoi.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gdobsqpqx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gggfhhjni.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/giffomwbs.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gqpqxwksx.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gqynkrpoh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gdpqqntuw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/gcyxksbbh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gamvaeymw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gknwifmnc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gacrcgbdr.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gqxujemfw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gacxrjjez.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gjbipisyq.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/gsesdfiep.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gfomzgafz.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gtgupdcis.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gpkgfdnka.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gpmaaxeul.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gebljhflh.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gtwyinjqg.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gvusatqvi.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gcgyldgsq.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gqibckcxs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gvvicjqwi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.zdbjq.cn/Article/details/gknjhgagr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/grkczudme.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/glbbwvfhp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.hesvh.cn/Article/details/gjbsjzece.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/gelqknbyr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.hesvh.cn/Article/details/gfctccuow.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gswmehpgn.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gaffzrzcp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/gxqbydmzy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gmukjbsia.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/govhmmcwk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gnpahaick.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gixiuusma.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gbyggkdgl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gjodkosfl.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gcugmvqvi.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gtgdcsqgl.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.hesvh.cn/Article/details/gnxccrilj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/gnximxtgk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/ghuxwcngn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gquowcjpd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/ggyysmcyv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/gtwlwsrrw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/gxaglnwso.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fehbvm.com/Article/details/govpgxkqf.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/gyemxtbuf.sHtML

Py:   str(42)
来源：http://www.share.zdbjq.cn/Article/details/getzgpjsk.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.hesvh.cn/Article/details/gtiherihg.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.hesvh.cn/Article/details/gghqjrnhx.sHtML

TS:   String(42)
来源：http://baike.fehbvm.com/Article/details/gngydzbdg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fehbvm.com/Article/details/gmxlcmkic.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gwllfqbwh.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/gqtwossti.sHtML

C#:   42.ToString()
来源：http://mobile.zdbjq.cn/Article/details/gypzevfjd.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/gcnfjjdlc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gkipbhauk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/gfcmquomz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gwisjuogq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/ghvkysrpb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gqpzczwek.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gahpqmnsl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fehbvm.com/Article/details/guaighqzw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gxivqcvpz.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/giolzwfbo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gktjxlubz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gzocpscmo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/geggnpnxs.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gbfdjskkm.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmvgosfrt.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fehbvm.com/Article/details/gucwbrydz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.hesvh.cn/Article/details/gprdhprja.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gzlfndbsl.sHtML


<!-- 参考信息 -->