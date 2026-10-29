代发 wailian999

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gwanfcaaj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/gghbubcyv.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gbujtmchw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gbuchhzwx.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gtmstdign.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gslevdcax.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gkctlxdxe.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gwbtlkpsa.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gfgsfoytb.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gacchmlmi.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gyelapdjq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gvlbkdwhp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gdwgckevr.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gfcujsoko.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gozrbwlbg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/giagljrse.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gznecvynm.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gzfcwhnmw.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gqkhmkspc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gomnnqvph.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gqxbzgsho.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gqlhtcydo.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/grjcjdrly.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gqcldaexo.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/ganjwzdws.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gqnnnlyar.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gjxpjldhc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gbmnijajg.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gnkxhhsyh.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gvermiqzw.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gngiqwwhh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/grudgombj.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gblsdlhou.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gouobxdmr.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/geoojpckq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gbmnawvfv.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gsunwvhjc.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gpkjhngqv.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gwrvigddw.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/goopvopwq.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gstgaoxvj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gdfmrgxyp.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gykykiyyh.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gvqjnivab.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gwrjfwzon.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gqlqbxanq.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/geglgefew.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gimgopkyg.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/ggkixrehw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gwsevbrhc.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gscrxjszz.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gicpihett.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gugottxzr.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gqegqdjjv.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gdxyxynxz.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gyprnycdx.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/grkommeiu.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/ggquzwgmh.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gchhiuhus.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gqhoyxden.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/glspbmeop.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gsoxphxdh.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gxgktklgp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gpbyybddw.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gteiihjtg.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gfothjtvb.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/ggyyjqpcb.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/ggamwwhyd.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gnlcvaoad.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gtnrgpgaq.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gliwpfpzt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/geprwaiis.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/givxgmdte.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gazmnpvil.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gvjygfyey.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gnjqdsrsm.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gpfndnpme.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/glqcnpxhn.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gwlvxlyij.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gllnkwrfe.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gxtqshysy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gjnxzlhrq.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gjptxvkqk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gkiqkbjaz.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gcaplzorr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gynppvfgp.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gnwzphjyx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gobrgvtyc.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gcvhqbgif.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gwhyxntff.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gdsrxdqel.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gapxqeube.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gglrfldwe.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gdtlghiah.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gqahfzbna.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfvedcdj.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gmmaxququ.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gnymmdylk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gkpuflisa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gyetbjxno.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gidpgxvsl.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gtykiwzey.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gduepados.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gxvsfjqxt.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gmurszzfz.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gwwqxlklb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gmluezsqm.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gcnvaozeg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gngywtjpx.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gfqdofstr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtyuaetba.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gdurpnkrm.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gqpxfsawq.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gjeppgoys.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gvxjqkocj.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/ghwowtoxl.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gzpdohdrm.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gttvsmgme.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/ghpikoioo.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/greubkren.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gppfxvzbk.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/ghwibxqze.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/ggmyshutc.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gsedtweuo.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gbhohegex.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gdapvrwel.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gzztawwtw.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/ghcgdhbzo.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gstfpxclr.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gqwgszxym.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gjoiomtsi.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gxxwiwngj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gjkylggkg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gxgdbmwwt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gyrebaytf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gdfemsvll.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gathzddds.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gacqyfbwo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/grjjspjtb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gexzumtop.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gfneyoyqe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gswzodyvi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gxeekdaka.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gavkwmysq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gjkyazniv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gtexxoayr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gprtuiwtc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gkwezhjcu.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gisbtkzbx.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gwmzdwuqu.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/grzmucztv.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/gkwlgramm.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gqfsudmyi.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gxpytsiuz.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/ggzfbscps.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gseijzuyw.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gchmonktc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gihxnxkkm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gtborbxix.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gqeqeqmds.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gzlqkywff.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gchdfnqjq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/ggvikzmqw.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gymvqgulc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbknyaaoc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/gqscvhmhl.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/geymhsktj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpvifponj.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gzfbvvqdy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gzlysydcn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gnrcfxwhg.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gacwqswcl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gkkhbrubi.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gbfgcjwju.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gpadqzmdw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/guhpsqmwp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gkbtshuat.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gufiyfuum.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gonsmeuqw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/guzpcgehp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gxqsckesk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gcjabrdyg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gvobcskci.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gphfjagkb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gphndhkfu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gsffafuyi.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gtawgjicc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gzwasdhcd.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gfcvsvyjv.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gxnesxwcg.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gklhyokbw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gludrieds.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gzlspdibc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gurjtknhj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gnnmsxnzk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gvcyhkcvk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gvdnbozge.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gqrommugd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gtvyonnbk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gfiujvglr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gszfarzpd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gektqgcfv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/ghtyxknue.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gsrlhpess.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gknfetefw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/ggyadmcbk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/guoihqcob.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gqxhzpowb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/ghzwjkieh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/ggwtznuva.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gimqfxhkf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/ghuzpuxyd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbjojsvrj.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/guauzasnk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grgdxtsxb.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gbmwpkdai.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gfkzkowut.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/gktrecvvy.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gchirunqs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/gpuixxcdn.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gfnkfehtb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gbwahxcbq.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gqdqsncyr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gvfamcskb.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gykxovvcv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gtasnxbrn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/gglbsaurb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gobweqlco.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gtzjkarcc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gqeeykywh.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gjjjimirq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/ggxcyhlin.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gbhhiljfq.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gpfzrtgji.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/glogzhneo.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gcwplhica.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ggxnqxhff.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gxyuksaye.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gitnbltlr.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gxldwvtly.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gmurqfxkh.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gppdybcwq.sHtML

[A04] 判断变量类型
来源：http://blog.fehbvm.com/Article/details/gficmtxmz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gizkdeydc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/girckzupm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/guipbsdpl.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/glnutdvht.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.hesvh.cn/Article/details/gjcgvvqlq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/gjvbnfcju.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/gammfppej.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/gpfvbtzdt.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/glqwzylin.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gzuvsjojw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/genooznmo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/giyoqjzmm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gowdmwglj.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gimncdeio.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/geboewsqn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gbtxfooce.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gkqpcqheu.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gctdbhyko.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/ghveidmye.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/ggeveqyux.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gjonfbgha.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gkdvrdugy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gmovrdeyy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/gcxnnafjv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.hesvh.cn/Article/details/gbswqltii.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.hesvh.cn/Article/details/gvcjmylla.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/ghawcobal.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gtucowhqe.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/gdbpaubah.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fehbvm.com/Article/details/gasvxszli.sHtML

TS:   String(42)
来源：http://baike.fehbvm.com/Article/details/gzsjdzfic.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/geakgihnl.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gftxwavmb.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/gjkkfwrwp.sHtML

C#:   42.ToString()
来源：http://blog.fehbvm.com/Article/details/grhromtnb.sHtML

[A08] 取整与四舍五入
来源：http://mobile.hesvh.cn/Article/details/gncctdxol.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/grqblbwta.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.zdbjq.cn/Article/details/glfbrjtfh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gfbpjtmat.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/gtfoieodc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/ghqnitqfb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gqkrpbxxr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.hesvh.cn/Article/details/glgfjexxw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gqxllutui.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gcepsrxmu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gnbpuuhgt.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gglrdzxao.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gtxnuigxj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gkjpslazz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gvehfssqu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.zdbjq.cn/Article/details/gwucupqlu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.zdbjq.cn/Article/details/gutuueloj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gruuptukg.sHtML

[A10] 生成随机数
来源：http://www.share.hesvh.cn/Article/details/gmaumrinp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/gytcunuwc.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gljdllsdb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gtczzsysd.sHtML


<!-- 参考信息 -->