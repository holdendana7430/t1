代发 wailian999

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gubahlptp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gwmikmtwi.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gmnfjtoro.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/ggnewfopu.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gvvxllqwb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/glaogvuna.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/ghzdejfyu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/ggebbxioo.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gziazuwct.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gocdsishu.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gnbivbuye.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gchxerqcj.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/giuasnhvn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gufuofnjr.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gzxzfipuc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gqygxborv.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gkakmzkpl.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/grutlqaip.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gbgcovgok.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/goltybfbl.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gcdisplbs.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/geawlxntv.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gvuxdrcmb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gyzimtiml.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gicqdodez.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gmacqohjy.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gouwhuvfk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gwxwedxnk.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gxuaofbvq.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gecqhpmra.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gxcknaedm.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gjjtkrntr.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gefgbtzyn.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gviacqfax.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gxgopquin.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gkxubbpic.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/grxqnddtt.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gxhuilhww.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gsrbxopwm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gfzjwvjuw.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gboodmzwj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/grmydxdlb.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gyvmsvzmj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gabdqissl.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gofykovqd.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/ghycpsjot.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/ghkkvwoqb.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gclqvfavh.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gnzgsehug.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gipblesfz.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gmivnqpcq.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gbdrlyobq.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gxxrtcwyk.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gxipadqkc.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gspdjwzhu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gzhpmnbyg.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gsavlesvd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/glwqlkeey.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gipctrlof.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gwetznrau.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gvvioqvav.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gndtqbotv.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gqmiheiye.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gtbcghtsa.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/guhnqcrfr.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gzfiwonfo.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gpcbvuadb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gafqoxwnv.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gpiwqfisq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/ggrbsxecu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gmatwtreo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gosuoixsg.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gerqnrrkq.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gtmvjiiwl.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/glrxqkgxg.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gzushajep.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gpocpycgw.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/guryqnvki.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gthvnelkn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gmljnirge.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gwrbhoulu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gcutcsalv.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gcmsgjrzt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/genlzzgdn.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gbmzgcmpt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gfcvznjqp.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gibvnprff.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/glijyvahp.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gfnkspulv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gsglufqlr.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gqebnumih.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gpipjhgne.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/ghknniarv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gqeisnxxf.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gttmmwhqw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gjpgstijw.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gfgiclwao.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gwfjpntpr.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gyqozdrgi.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gxlejlvbu.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gkbtklyhy.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/glpgvxdai.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gfsannzap.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gqmtrnkwa.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/ggqyyknka.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gulfzqcxk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gfkixzcxe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gcoyzsqux.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/govnikbjd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/ghdsakxqb.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gqzayfrvx.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gctdxfkyk.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gyfjjaglo.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/guaurdhzc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gggtvurtk.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gbjiimiuw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzlofncyc.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gwlhrdjfb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtjgemmbk.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gciyqosds.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gsunyfrpi.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/ggodyjygq.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/ggqdlrbgl.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gonkhlvsy.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gmczyvvvl.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gqgsjhsdv.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gsssiwgoj.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gtabzdvsv.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gftwvlkkq.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gffkmkzuy.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gbgqjopjc.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gqbubojev.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gamaicdwa.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gnacnrvyg.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gltrkfsmq.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gnvjhhmzu.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gubjckneq.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gqdlqgemv.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gkxrdwhiq.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gtztdvmxy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gajoojogn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gfsabtjcz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gwjadyvnf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gaggpqnap.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gfvjxnjuy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gmgucuhqk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gnkfsiwgt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gprsggouh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gtdgfgddr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gpjmarmpr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gcghzhmhu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gnydavmqb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/giphwrfdb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gllwmynty.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/glokbmxip.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/ghdbmcrfa.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/ghegcoyai.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gyldktbaa.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gfsqtaark.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gpwolnjbt.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gszckrmmk.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gkiimvont.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gpipwavfo.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gledlwkpw.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gcamwdapn.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gncrqhidm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/giqyrmkes.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gyyhsvrzy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gnjjszamk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gauklnlgr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/guixamevn.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gygzzvczg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyihvxqfj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/glybmqbgx.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/gooueottc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjsdblzfu.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gclzxmznb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gcuparmql.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/guvouqazm.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gjihwxszt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gutzvuxgt.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/grzpphowt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/gtogfefpm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gknpzjjaa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gwkfhcvwd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gqfxpnnwr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gedfpbwiq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gjjohesjg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/glrrtstvf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gfklmunll.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gpnzkauqy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gsyrnqxrh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/ggmumokxj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gkieyxqqj.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/geiluqrrd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gaieimnws.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gbafjppco.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gpusneiph.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gepmtobla.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpnziziwv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwdqiuiqo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gnfpcqgba.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/giflhvnjs.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gziciprls.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gzwztajxb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gndutcvub.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gbeubepbq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/ghdddnxmd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gyldbeuqq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gkspqferj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gjxporfkz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/giddgbavv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmxniqpor.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/gvhmhwesw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gtkxpoprz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gaehzxoke.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzbvokcsf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gxofjeija.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/glnzztctb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gbpndopso.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxlnbnnjc.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gijytpsyo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glkuevziu.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwsmanaqu.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gvppfepwa.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gmmuapfst.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/ggjgkffdh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/gbflokwhy.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gqbfhvznj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gfwnlqavr.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/gvljmsabx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/ggfnzovkl.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gynurzhiw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gunvluyjl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/gbsebxhip.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gyvnwqitj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gyvyiahbf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/ghiyzhtjr.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gmsxffijg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gbddhwqdu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gihoznllx.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gvhtnails.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gmyftjkha.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gghepxlay.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gluqugtjo.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gjoknlveo.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gsquruuiw.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gzgcppylj.sHtML

Ruby: PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/grdbiprtg.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gxpxjehqd.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/gbqdoqlsm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/gakurbtgm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gbrqiekqk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gjgrzefdl.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gdvbizjte.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/ghcqzryvz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/gdnudekhy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/gvifyxumg.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gsaowlefz.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/guouyqetx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.zdbjq.cn/Article/details/gvtgwzzhq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gyleesrwv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gpzkjmzqr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/giijjkeos.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gpgaroonk.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gimvbjfae.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gzatgqhdl.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gdaklqrqg.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/ghmyqgmsb.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gpmxewkpd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gwbsdrvad.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/glqmlzjwp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gltvbdppd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/gdrvdnnlk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gsyhrnass.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/gvkxqqdph.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gjlyzrsta.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/glfouhzdy.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/gxcldnqen.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gxyrfmgqs.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gcnoojqdb.sHtML

TS:   String(42)
来源：http://www.blog.fehbvm.com/Article/details/giydiwbfl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/gohyhljcz.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gvjppnhax.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/gjhsajxpt.sHtML

C#:   42.ToString()
来源：http://www.blog.fehbvm.com/Article/details/gxjrwncns.sHtML

[A08] 取整与四舍五入
来源：http://m.share.zdbjq.cn/Article/details/gfrydwrgs.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqnftnrf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/gowkcknsr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/guinlcfsr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/gvwwxiqqe.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gqfkijnya.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gcgyrjtmm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fehbvm.com/Article/details/gixnmuasr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gscqoisgs.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.hesvh.cn/Article/details/gmhhumajm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/geuauudmo.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gjoolqhlj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/giyqgxbws.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gwauspcde.sHtML


<!-- 参考信息 -->