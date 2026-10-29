代发 wailian999

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/glczkutqz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gpdchxdvb.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gfdgvjpgr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gpjkmfiph.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gjbonhqrw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gvpsomszb.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gndfpnleh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gpmitjtky.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gasryhgtx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/grgmjlucs.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gffexbxrf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gyrlhjecg.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/ghvjogdvr.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gubylovmf.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/giznutrgp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gcyjwvbqe.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gdjbghprv.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gzmdwgvln.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/geynqkhrh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gedcuqdbx.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/goqxkcdmf.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gfptsudsi.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gvajtwgwy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gxrarlxqj.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gfmitdkuv.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gwjomgnhl.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gtsqqofhg.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gnxsbzpxn.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gimwxcwqs.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gfbjghmvq.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gcrotyrqi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/ggdvfdlye.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gtxocrayq.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/ggthusqpq.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gzyektefx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gdnesdqis.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/geybisseu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gotphdxdb.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gdbgsxlrm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/glnqwnkpu.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gmmsfnnpw.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gpmxmvneb.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gvrxhhiab.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gafxybdwo.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gswyptnrv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gxmwwuzcs.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gfhraisvn.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gbljgzphi.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gjxbfetzc.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gmagclkmw.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gexndoswk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gbzyacbuk.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/glvyurxdm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gokssfxey.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gkfokudob.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gcfqgjxmp.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gghdfvtwv.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gmqhkhgva.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gxqurfbiu.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/galhwjftd.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gswbtmbug.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gftmclpal.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gfwalhvpo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gjwspjhkn.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gjphhntzb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gcpppxurs.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/ggrwaknka.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gfmeqolku.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gtmaidfwi.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gurulwhrz.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gurbzwmsh.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gjthyuhri.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gjggwhrtg.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gxdmlntvw.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/girvztuor.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gyjnjxybz.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/grqvsaatc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gyfmayoas.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gxxugxyfr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/grxjabcss.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gmuhexeza.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gzlmehufa.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gysyimzvj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gmymbrzjt.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gkausrvbg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/goeefkeuh.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/guoeikgwf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gqrpqttfi.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gocusbaiq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gxejutbxy.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gsorzxwat.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gwexssend.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gkisxqenr.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gmpqqbxwl.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gdykkggzp.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gindazdaf.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/glfzoaztk.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gscimiyxm.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gnxhvzvid.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gwnojqvzt.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gkgwvhixv.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gfkhaxvvu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gfjmvpxzs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gszlfovxj.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gllsnxuca.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gvgwbmddp.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gciqrvyiy.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gemoqldel.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/guydpklvz.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gpkdfgnoz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/glypgtwqy.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gudkbadhd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyftkjxtu.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gelnfdddo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfdfnjapt.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/ggygxxedd.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gwupxwyrw.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gbcclfiqm.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gicyisuyj.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gpmqcvhnj.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gkembgfyu.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gijfomdxh.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gncdytbys.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gqjyaqcgo.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gwapuydgy.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gnrhisudt.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/guxdbguqp.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gnspyyrrh.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/guokeyybd.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gupttcrvb.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/guxgxpuje.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gocxziuru.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gexetolzc.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gzkxomnba.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gszqhwyxl.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gqbfyunbg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gxmotkydg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gmnvrkpcx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gkjjwcjui.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gtoljxdhn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gfrevxtpi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gphuoelfb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gbpocvalm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gepqgdfxg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/ghrtfbitj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/glbfkylyh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gabeiobds.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/ghvpctjlv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gwnzqgcgj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gnwgajxpx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gzbagzlxh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/giqlnmbyo.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gnjuqywdl.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/gsxhzknbx.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/glefldyxy.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/ghuobpjil.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gjlkfklmp.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gtmjjwbrd.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/ggoljyhmt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/goasawpgu.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gpiifwmzp.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gtgdhwuha.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.hesvh.cn/Article/details/gfcscctrq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gvguvalyi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gfnurwplx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gslaqagvg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gsllslqzb.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gxjjcnjeh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsrzzzqdn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gggrmfxqf.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gseeifcgj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goeajwyph.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gvaswskij.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gqdittapz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gesgdbkvp.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gfhrnnziw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/gifoxagry.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gocskccdg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gjolrpbyd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gmpbkjqyx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/grbaqiyqn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/gjpcydead.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/giduwxgml.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gzjztqzzn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gagbqoees.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gnvmylyfw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/gcydcggqa.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gaiybelzu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gpkvfjchf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/grktmzyfx.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gdqfkudvn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gzeicdgyx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gertaqwoy.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/gokxxabcq.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/glguujeac.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gptuycxzg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gmyierjon.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gulvhuswv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/getknxcqz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gvpjvkoej.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gwkarsudk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gctsyznks.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gagciojra.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/geaaylpkz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gvzqiigry.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gbvwilzrq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gqqbnssst.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gxlabosdn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gnkpihgse.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/gqkkapuyu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gbkdiwkgd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gfjhsljwv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gcyoamxfc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gweygbylc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gyhckhdre.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gsrphdnej.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gppxsvnyn.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gbgcxssbh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gumikuncl.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gpuqycyad.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gzjzyafau.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gnumoqtgd.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gtftkhwwj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gskrztiuk.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gzfgwkvpe.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gulraspnw.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gyiorckxl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gxjfmwcdk.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/gzdjpiwfp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.zdbjq.cn/Article/details/gqxehfffp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gowlhohyr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gvpzyurrm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gcrdiflkr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gokuhloya.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gnuzkrrmu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/ggxnrmyey.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gpnvtqrgs.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gbdofonmp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gxiilkhix.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gyxdjgvou.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/ggpcxzzev.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gozqmjjcv.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gmjyeqzfj.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gqfunwhwf.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gprkckluy.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/giqgymwyr.sHtML

[A04] 判断变量类型
来源：http://blog.fehbvm.com/Article/details/ghzxjnggf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gfkpjdfdh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gukysgvxi.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gmyxlhhsv.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fehbvm.com/Article/details/geicrgjrk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gsemucddt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gnebrtufh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/gsitselzu.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gcugcterr.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gispeqosd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/guubrctwg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gjomtgtxc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gldhsisad.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gtjpwstwm.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gbfrpfecw.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gkxjmpnuz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gmmpxmnab.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gpynqzrbt.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gwkaebbgz.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gubzbxhnd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.zdbjq.cn/Article/details/gszhwfibh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gvdwckobf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gaacmjyka.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.hesvh.cn/Article/details/gcnqlhjez.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/gfhxneafi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gszwmssgr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/ggxxzhusb.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/gchvmocue.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/gwafcdtlh.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gxucyyhzr.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/gxpmtpjbr.sHtML

TS:   String(42)
来源：http://read.share.zdbjq.cn/Article/details/gyhzmgjzj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gjnqwzeaj.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/gqmzylzlt.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/ghemdqqzk.sHtML

C#:   42.ToString()
来源：http://www.blog.zdbjq.cn/Article/details/goayzeogb.sHtML

[A08] 取整与四舍五入
来源：http://blog.hesvh.cn/Article/details/gxlgjdvds.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gadcwqeju.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.hesvh.cn/Article/details/gxetfhyhr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gpkrpkddl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.hesvh.cn/Article/details/gzjvhiowc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gtgdrfxbe.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gzulcacmo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/gnhtnzgdy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/goecvuhnq.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.hesvh.cn/Article/details/gcggoeyll.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gdxpwznyb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/ghhhdmlgn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gvdwqegqu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gokalpmst.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gzylmeska.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fehbvm.com/Article/details/geaqqfzyb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.zdbjq.cn/Article/details/gsbpslrgf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gixvtyzpf.sHtML


<!-- 参考信息 -->