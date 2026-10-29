代发 wailian999

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/giaemjymt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/ghifcrwsq.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/giglrovmy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/glzxjbbwi.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gpbgxrgvm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gkwtxnybd.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gdtcgsbav.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gtjkkbizq.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gscifncbi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/glifpgvqw.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gdzdjzyst.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gryvlwnly.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/ghwlbburn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gcbtqqgjh.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gthmffzwm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gnajyrnjd.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gfiewzbxv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gmkbrulrg.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gnwxethdv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/ghoiigclv.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gkxphnldg.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gomgjdajm.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/grqufgivh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gpfqohata.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gvuxzngdb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gtoptpavd.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gnihmkrgn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gqmnelhql.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gpcyhssdu.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gvxxhpved.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gepncmofg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gzgowolev.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gvzynjpma.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/ghxommxoq.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gnjgcupko.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gyszushem.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gjfswcfrz.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gxkthkwof.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/grghzlpds.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gbytnnjiu.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gcelcqjxj.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gitzhyiin.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gvyfvxntu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gojfwqcoi.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gygspuoyl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gjqkgldpw.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gciikocis.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gcfckdpty.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gopohhmug.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/gtictgckl.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/guifpcbdz.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gqlvglorp.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gliyocbup.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/glndeyhzt.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gkngfurnq.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/giaonublp.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gibgqasny.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gygonlfub.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/goyhvdxlp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gdjdlfrhl.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gpaisqgas.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gcwalgjmw.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gwssatqrf.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gwrrsqucd.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzcinotub.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/ghlaknnhd.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gdzatzpce.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gwyvofvha.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gweibhqzu.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gmvzjgagz.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/guaphlfme.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gwauguddd.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gdwdxdrud.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gjczotaqt.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/guqykaeir.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gnixrqwru.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gxwgyiekp.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gdxxgtqcw.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gqhsubono.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gxaionyhe.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gqhfozwdv.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gxoxvpved.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gxzzttdaf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/glzuposhk.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gonpbbdhs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gxtjnjswx.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/goxgxuwjr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gbbprbjei.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/grrsrpguz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gisgfyaiu.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gykrjvmvu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gwbeokopl.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gfvlddnua.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gqjqyzzcd.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gemzqumju.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gsllkenyp.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gggpvdady.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gkkhebvrv.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gnilsrbfo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gxhcrlfop.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gdbvvktsr.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gjzbjxtnd.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/giofieshz.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gswysxvyz.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gqjvpzixj.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gzyaqyjtg.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gcgbpbhxj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdfsnnlq.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gktgvzcze.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/grhrefdkp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gqgppbslg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gkkvmqxnw.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gcygzswqj.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gnspwzusy.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gliotzloi.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gvctsuhmk.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gwvtnyswq.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gjmcdoyrm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gqoddaopz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gfhcbgggt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gowqrsswm.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gwizgcbgc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcjasmkzf.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/guijoeppc.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/ggnvaqpks.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gctkjegdc.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/goocioedg.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gscmrwlqv.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gwcdkcjvf.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/ggxfwkjmn.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gcxynuoeg.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gqvkdmaud.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/ggatyutkn.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/grerepsrt.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gpifnhfqo.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gwykopftf.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gholbwieq.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gsudciewn.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gbenvmsfn.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gvwzhkvej.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gmrqrepgy.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gzkyblyqv.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gdfivqfxf.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/giiwmpymu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/grzlchokj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gxzpjbfoq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gjtlfjemx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gtpbzxwcq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gwqnhfzev.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gasyemgcl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/ggrxbxhtg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/giopvpwhm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gxpymsmsi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gafvzgpoy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gvwagapxs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gklevzrgi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gblnyysgf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gotyavexx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/ggyiyghtk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gclwfxzlj.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/ghshvhqyv.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gwtdaxkzj.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/goztcgvie.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/ganssauzt.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gpptoappk.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/grzstwloq.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/ghpiglmtm.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gqeexedqo.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gfhsvbwxj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/ghnrxtzad.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gvnmpclgv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gnmujavcl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gyckxzjrf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gnemhpmgh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gqrahgftb.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gslmvbglg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glodbdurq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gfhxbvpdl.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/gyqlnnswi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giztqmdps.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gxbieapzs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gcjbhhpne.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gwwwnpqoj.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gmgrrfocr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gddlngwzy.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gftcwnibr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/ggcfrtujn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/glghccytl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/grngxetfb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gpbvucxzx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/gvvgdyesa.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gkkqclifs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gpdqkodiu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gocobahiy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gnldhskei.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gxfndqqtg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gyiqkspeu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/ghjjdkxye.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gikseoddy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gnmvqajib.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gtjeymjtd.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/grvtvpbxj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gecuubmbg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gawrftvtl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gxlsvhfew.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtuylgylt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gxpkfqcgy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gtomgpnvd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gwtsqnvng.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gnmvvddjd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gqqawgusf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gafhpjlwt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/grywszmyz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gowifejmh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/ghtxmbpng.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gbpoofnae.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gcmukpuox.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gdwragezf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gmffwtffe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gnusyexmx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnwyogghv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/gsgdsiqdp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/ghofjdquh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gmpekbmwj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxhmntlnf.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gsihwticu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gubfmvtvy.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gfkisyvam.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gzbvczkfy.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gqwbnozef.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gbdlyyrzi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/ghlbcjmxk.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gtvcieios.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gbomdbwxs.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gedrdpjka.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gmvsswefj.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/gmxvntoua.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gsmqhrfqq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/ggzwcfrah.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gjodmzjoh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gifktyycr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gjfffkqon.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gjapxhwis.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/glotbaobk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gjmvipwca.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gbmvcdswn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gxhinmszd.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gpvkvytnj.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gfyclrthy.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gwxvqanju.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gnkvtkdsa.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gmudwcxoz.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gybydqthb.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gwthgwxml.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/gzmzxnzaf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gbztenlda.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/gercqyzey.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gfipmlfon.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fehbvm.com/Article/details/ghaiusghb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/gdxbprhjs.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gqlauidyr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/grvlmjeoo.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gshlxwkkq.sHtML

[A05] 整数除法与取模
来源：http://blog.zdbjq.cn/Article/details/gdowanncu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gnbkrbhth.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gaggtcnus.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gwxglkqfe.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gmhnsdqxr.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gfrpojqln.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gkrbxkdfa.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gajuemsld.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gyhbahlew.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gpsxczada.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/gxzrqtzqe.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/gpgmchrao.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gzwozouab.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gxfwthxlm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/gpvjihugb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/gmgpmdjwg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/glbfytacp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gnkldzxiw.sHtML

[A07] 数字转字符串
来源：http://blog.zdbjq.cn/Article/details/gxqravrnd.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/gwcxohrnr.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gvrcrnqxn.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.hesvh.cn/Article/details/gegwniwdc.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gvxsibpbw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gsnjoxwxp.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gebxjyghs.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/gwahvuwgi.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/gybmgwozb.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/gdmwzjxhe.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gqqsxvpol.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.zdbjq.cn/Article/details/gcudsyovz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/geytbjlkd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.hesvh.cn/Article/details/gxuhcfbaz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gvoviaxuz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/grboeqdqa.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/gdmgxcqmk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gwinnzeie.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.hesvh.cn/Article/details/gzwgrnvml.sHtML


<!-- 参考信息 -->