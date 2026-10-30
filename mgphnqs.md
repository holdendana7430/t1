代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gllnyvula.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gyuhqtriw.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gdckfpgqf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gxybuxkpg.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gsnidzpyx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiydnciv.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gppxfqbrl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/ghtzejmxt.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpgnrpzt.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gqytanrzo.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwvphgzm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gzkfsvdpr.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/ghlucnwjz.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjabefbkk.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/glqmhspzf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbcvyugc.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gglgujwxg.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/gkvwrrxmu.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheofptnb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxvwvooa.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gqtsevofb.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gitqmveyi.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcnwcctx.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/govrglmbb.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxanilce.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/girficepc.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gvykrzvbg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoakavkk.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/ggjnnidws.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gbdvuojum.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/grdynooda.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbhxtwul.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gmevlerqb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvuxwmhg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnuegdzw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gbicxawfm.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gneslkgsa.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjaoxmtk.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gpoumkwqj.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gnlukwnil.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grucvgmyw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiouejnm.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzyuydmq.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnexoxvjw.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/grrhmnnwu.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gsmlvkpmq.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjrhpnwf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gopepsemh.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gkbfddtwb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkfcyvuo.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtneghmi.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gsdtfzoid.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geamazmfy.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/gpwehfkhu.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtakiddwg.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktlyebfg.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gsqayipdm.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/ggjzwatvp.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gwcpatctd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdvjpbax.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcjdybfh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gchupynmn.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gsvrvbddp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/ghrkbvequ.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/gtwzxomaj.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyczvlrb.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztzkzjcr.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/ghdcvoajx.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geolevhyl.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjkfuelu.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gikctwwjc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/getajreqo.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gqryncwnp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gpkksbory.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gimdrdixu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvmzptyv.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/goaixpvzm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gpcuhlqrx.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gowzsjkpf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtpmsyuu.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gxccaddoa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkxghdao.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gtqyuisbu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvuwkqmu.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrnlhigz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/glmfiwdin.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gbzynuzzx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gcyceixxb.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiflyqav.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfxkzfyg.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gbsvhnzut.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gejqxwxpo.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhjhfaxr.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gpmchukhw.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrlyimdd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcvbnwls.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgcqnwue.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gbqewqfoz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdoxbcyq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedppgthq.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekvcbyrn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkontkqlw.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfxuuxyk.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gxfnajzeu.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmzojsvx.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gnmbochwa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gllyjvgut.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkukgovgu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gueujgycb.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gtqfvbemv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnmylkjji.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gtgmuvgyd.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwendsla.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gbqjhngrg.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfreinpq.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwlawqws.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/godlqltmo.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gqadmczbn.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gugqzvbfy.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gmszythfs.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gdkrzsdbb.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/grheyycko.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gyqxiwlwe.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeigasne.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gaseujryb.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpdjmgnp.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziyahxnv.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/ggajyhein.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbmgmacw.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpiioxdi.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxpdzlqt.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/ggmxxnppu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvuvidyl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpdsciod.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxlgufgd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gcztrkqzq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkylnnfc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gayovfdjb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwqzdzxm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/ggbigdcnd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkvwcjae.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybvdxmse.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhagdicj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyxwlkaa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtlxkgdp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgiybvwb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgnqihlb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gglraketu.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkjdkomg.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonblfkuf.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gajaljmvm.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxuoeeiq.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gczdsxtsh.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gucqjawuq.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/glfattmsp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gcouzcesr.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/gtksjbjjb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/ggoofgevx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fanxiaobao.xyz/Article/details/gdccnabbr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/ghprerjbl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgqavaat.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fanxiaobao.xyz/Article/details/guocjxvuc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gdfmontvm.sHtML

—— 文件结束 ——
来源：http://baike.fanxiaobao.xyz/Article/details/gkcwcmuei.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtllgofqv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/gnsoqolqn.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqlqzxjz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnnqszyr.sHtML

【收录内容】
来源：http://baike.fanxiaobao.xyz/Article/details/guwdcktuc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbcjojwy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrorazfm.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsjxowsr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fanxiaobao.xyz/Article/details/gklzuaayp.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gthineoac.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/gphqzslpz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoaiaydh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fanxiaobao.xyz/Article/details/gfzzvylza.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlwatjfu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvmunsiv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fanxiaobao.xyz/Article/details/gxamedehn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/gpphzxmrm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmcahdro.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fanxiaobao.xyz/Article/details/giuxpdtil.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzodqowt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/gaobceysj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/gztcvleea.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gvkjesain.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxmchgwf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gbcoawfhh.sHtML

目  录
来源：http://wap.fanxiaobao.xyz/Article/details/gzxumiigl.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhzujfgd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glthysjgk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfhbcacm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzozkyfla.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqldmrrq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fanxiaobao.xyz/Article/details/ggifvfdsy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/guqrqksys.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gjkveeasw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnywfrbj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gaglgvcdi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gehxrzyai.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gfhjeuiqd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjplufqux.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gavfxnlbs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsexazkv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goujoqlkt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gduatwayr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeezvsdf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcahuqhf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gtjlwqasu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfxuzgyu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gozxiqyeq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpxcuwbq.sHtML

A. 基础语法与类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebyfozzr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gitqhsyzw.sHtML

[A01] Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhikjadz.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqihjthki.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbshfini.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfhzzhgq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxxffgyy.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjlxjgon.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmxnkhvs.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gejwvmkiw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbacxptku.sHtML

[A02] 变量声明与赋值
来源：http://wap.fanxiaobao.xyz/Article/details/gwedmjtzv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fanxiaobao.xyz/Article/details/gtakbkzxn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiixdybn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzdnuoqg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gplkeeoyn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/galgpchgc.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fanxiaobao.xyz/Article/details/gygnwmuuz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gyghvhkpc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gleouxgyu.sHtML

[A03] 常量定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvftzlnrc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbuwynrd.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzqwfvvk.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/goejkinyq.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyfwhgxk.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsvwuyub.sHtML

Go:   const PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/goyflntdl.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpxcaezg.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gdcvhirav.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gkcjyegbz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fanxiaobao.xyz/Article/details/gddiqebji.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fanxiaobao.xyz/Article/details/grezyzdup.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygjnzqkc.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/gkqaqcekp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fanxiaobao.xyz/Article/details/gowlvmaqm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjenjjjds.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqjausuw.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fanxiaobao.xyz/Article/details/gmurwlfzo.sHtML

[A05] 整数除法与取模
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwzgzhld.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgbhqmho.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzlgmydu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuvsigmz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnieifqct.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxcoslvy.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfunuczm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyixmazv.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gztlqbslo.sHtML

[A06] 字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/glfmngplz.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/goccpfufh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gzgovjhjl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhcyjpqv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gdetiglxd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglysanin.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fanxiaobao.xyz/Article/details/gfcusrhjr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggocsgeus.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrelroaz.sHtML

[A07] 数字转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gpbrnesrm.sHtML

Py:   str(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gisrhpbuo.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gguzncobg.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/grarqwarh.sHtML

TS:   String(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuootlmg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gljtjmgvm.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gytkrpime.sHtML

Ruby: 42.to_s
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzlexyqy.sHtML

C#:   42.ToString()
来源：http://3g.fanxiaobao.xyz/Article/details/grapefmwl.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxmikgzs.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmnznxin.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhxoupmz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhzndghi.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fanxiaobao.xyz/Article/details/gstdujzkv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugxplyzc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gdkwedhxi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fanxiaobao.xyz/Article/details/ggznibjpw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gqqxicxfl.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gmigimkqt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gyzcufmdf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gedddgyxs.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsleoywgn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/grhwzxnnu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpqtpumz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnblcljw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fanxiaobao.xyz/Article/details/gogrjasqs.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmxmovqj.sHtML

[A10] 生成随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gsppipbqn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwhopfuf.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvtpmicv.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/grdvabxmn.sHtML


<!-- 参考信息 -->