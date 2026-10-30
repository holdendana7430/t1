代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiujcmeh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkkddsqs.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/ghpogwszv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvabeess.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpljsxgx.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gzmogbupy.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gxbvgxhau.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeqljiot.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gccqxiiay.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszsclrhp.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjneseee.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmebambiy.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gbemylflq.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gafelczuv.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfwctric.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewrwjlwe.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gnsircqgk.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnchchnw.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjxjxhon.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gvuwjadfp.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrbbfjyy.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/ggeucewsg.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/glstgiuje.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gkpbontfk.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/ghubcgvkg.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gsuxsmgam.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gdyknvwcg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgknfyod.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecchxsag.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgfgsnda.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpigsroyw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/guzmnvrpe.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvsdqwin.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gyesffhnl.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gfjtckkud.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmamrksp.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/glccbmhmt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gililzdii.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gqdhlaksr.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtuxrgyc.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gzenqcopj.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvfryofg.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzatrggqt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvkuqvep.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzuulznc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gkipynkut.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvpgcuhl.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfevzjegr.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucjuvdws.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/grpurblxh.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guthsfkfe.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gtaqnlula.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gofuvjsou.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goncvnkvq.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvhrlolr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtoxxssf.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gybbrullg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzqejfld.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gpzliirmb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkmshivs.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gourgrthf.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/goojmijas.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gqrieuoyp.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngurgwsi.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gefheillq.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gcdkoomnn.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gjealhzmm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gprzbnbka.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/glqjbpijw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gwhhhfafe.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvbowdsc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgxnuuyl.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgincfzn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gcosursna.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkndjyngk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfnzmetz.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyjatgqe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gdnsbxvow.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwfgdyla.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gdetppdxp.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gdqldljkz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gnkaueajf.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/graisqtat.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gubheqrik.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gkzefeknh.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/goilobawq.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyrxptvt.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gscqufjsz.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gignbzozu.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcuhprgp.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/ggzgujrqe.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxgmguop.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfjlebsj.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfkaxxkn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gquptalvi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjshlvril.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/goigptxks.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gulpvbgbu.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/glrswrdaq.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/goucezbil.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/ggdyormri.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiomyahl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/geojpumhb.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/garmpdhlv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnudyfuuf.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/goankpxmz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geibclsyq.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gqpxmeqwc.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gquwlewbz.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gglculfbo.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/geigtmles.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvjtszph.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gqijttagw.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/grbzqvfkd.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gxgsezvkn.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gposcddrw.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gnitdheyg.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/grlgrewli.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gdothszxj.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqncukvs.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/glbtdgern.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbkpyhop.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/guczmjnak.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgqesbdr.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqmegzag.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gjfnsiddw.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbezjsxvi.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gplqedeax.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gkqayhpuj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gmuvkcmml.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gdhpcaqzg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyftsidj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gljnneuhw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/grvrekrpe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbyonhet.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmnihmky.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfgewdsu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/ggmcjyxhd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiqnzkod.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/geicerjmw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/glculjlrg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gxuuronkc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/guvklpxuz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gofetstmm.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gqibucsto.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/gavuybzvr.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gqsrbaqak.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdimiuyi.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/ggelremod.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gkpnmqrgi.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/glbxanrgi.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/grziwdibu.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gezvfzxmz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gmxrwepzc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gggvgfjsi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqbfhhge.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/ghhfqgqeh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gqftchcpy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/gppjxrdkq.sHtML

—— 文件结束 ——
来源：http://wap.fanxiaobao.xyz/Article/details/glgoyuden.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gciuhfzmn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcxdgasn.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/geaixital.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvmjtbhle.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/girgzsejo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fanxiaobao.xyz/Article/details/gnceusaoa.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrgirqsw.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/girzcsuzm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gbnlzzmsr.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlxkrreh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/gjamjzzqh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gwknccpvs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/gdxkwpvrf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvxeywun.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fanxiaobao.xyz/Article/details/gbbsfyrhj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/gjddmlmgw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwfakhgn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/giwiolxxq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/ghecoxzri.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fanxiaobao.xyz/Article/details/gvllngflz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/geawxrhtu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gijjfglfl.sHtML

【文件统计】
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcxgugut.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fanxiaobao.xyz/Article/details/gogxrfdyg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/geskerivf.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/goyapyfwz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gkjbdbqfa.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiwqfcjg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpsmzapw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gntifosxn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzuhyhrj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwovhtunx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvbuodhy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhetmohm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gaxxvplhd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/glcunrvoh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gubmlurau.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/guyfrpycn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcvbprnj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiductmu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gzdxdnqdz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmmpzwmt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gmcahjrny.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqbfboux.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjmwrqxp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvchobjuj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbpbsijy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gnaesnmra.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gusknybbm.sHtML

A. 基础语法与类型
来源：http://3g.fanxiaobao.xyz/Article/details/geqnobcdn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvexxxdk.sHtML

[A01] Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdirrufv.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxjhonfd.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fanxiaobao.xyz/Article/details/glwnonnuo.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gkobebmcl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fanxiaobao.xyz/Article/details/gbtyzkdvg.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gacnkftpx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gnhgopvxa.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckjkywbn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/glzwqsabn.sHtML

[A02] 变量声明与赋值
来源：http://baike.fanxiaobao.xyz/Article/details/gukhjhmtm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fanxiaobao.xyz/Article/details/gtppeczph.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gseyjeuva.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gvvrvehlg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/goixbhdxw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gkvstuiyt.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkxklada.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fanxiaobao.xyz/Article/details/grwcbqyqe.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhmgtsey.sHtML

[A03] 常量定义
来源：http://blog.fanxiaobao.xyz/Article/details/gzvkbwrhe.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fanxiaobao.xyz/Article/details/gfrcjovzc.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzajhvzwh.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gmjfmmmuk.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmnequzi.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjahfava.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gksfvoxcb.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtkymjxf.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllybyiav.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gmhqtfkom.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fanxiaobao.xyz/Article/details/gqgsxjocr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fanxiaobao.xyz/Article/details/gakynmkzd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gcswryucg.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmcdlwqx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fanxiaobao.xyz/Article/details/gleycurni.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnardffz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fanxiaobao.xyz/Article/details/goruejoyv.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fanxiaobao.xyz/Article/details/gqgdcdoah.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcloijhfu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fanxiaobao.xyz/Article/details/getjgxssw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsyyunro.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gffgavufl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/grdorfgzr.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbvgrzpl.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gyyxxodgg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfynyjlk.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcspyruaz.sHtML

[A06] 字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gfvwxtwyy.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsyciyrz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfmovkua.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxlpqszt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fanxiaobao.xyz/Article/details/gzpbaffeb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/grtfybxps.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/geglqiypw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsxgfmcs.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/goimuoxfr.sHtML

[A07] 数字转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gdgunabte.sHtML

Py:   str(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggctbuaqu.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmhowfea.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gozuidmmf.sHtML

TS:   String(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gappdozvw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gntjxrkjk.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gimerzror.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufflntmn.sHtML

C#:   42.ToString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gujwkdrpm.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvubzljs.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gnucsqmjw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fanxiaobao.xyz/Article/details/gjnsbpqiy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfttxzvzy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fanxiaobao.xyz/Article/details/gygrnzxve.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gzfuendwg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gvmbdtoff.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fanxiaobao.xyz/Article/details/guqtnyovx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/grqwyeskv.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthppogdo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gerfyitwo.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gydhcnwqy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuwjqvdd.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaeovkefd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gocetaxdn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqczanxu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhkrqkgi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gldzowtxm.sHtML

[A10] 生成随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjqmoryd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqbqmvuk.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fanxiaobao.xyz/Article/details/grozmumqy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gztvbpero.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/grkvnzoas.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gajsmbddd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnsdnhua.sHtML

Ruby: rand(1..100)
来源：http://wap.fanxiaobao.xyz/Article/details/gxppzmqyf.sHtML


<!-- 参考信息 -->