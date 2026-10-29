代发 wailian999

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gqhouxsjf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gbcqzswav.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gmnnxvcvi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gdrxjyesx.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gtlxpdoya.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/geffqixdx.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gewagjhmx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/geqdrvvrf.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gtelkenzz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/glehobeez.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/grjvvxoui.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gfvtpeiwu.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gpgbiyttj.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gdbsatpnf.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gizlqlgde.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gqvhruwiv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gntcltzor.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gyvabgwlk.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gwpohgecf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gbxazakne.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/goakevolc.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gmevzbuxy.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gurcptlgk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gstlcoakx.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/geinxbytw.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gnsfmrucr.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gavvcspez.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/grpnuqkqp.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gsskhorhu.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gflxrywjw.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gkqysanfc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gcrvaqfnv.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gsujsesbq.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gpfcdnawd.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gxawlztwj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/ghcptclxk.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gfgudnnhe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/geslohfky.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gccugkxji.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gcjxdjruy.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/ggdulfwpg.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/guylvncpq.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gzoyybeoh.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gmmpyjejs.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gjorvcqjp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gvmkwcrmx.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/guefzyqrk.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gisiygbdy.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gqoojlftl.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gfpjbendj.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gycdiblgk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gjaxvrxfl.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gcdwateur.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gemrbfisj.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/ggatxejid.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gncafpxui.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/giibfxjbp.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gsdqykwoa.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gwormmuob.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/glbyjcfav.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gvrgoxafg.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gmccpztcw.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gmjcczwmc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gxijbntpj.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gekdbrslh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/glpjvlqec.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gxccgbmzh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gvlsoavad.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gzxcgjlli.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gblposmru.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/guphiciyr.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gmyvaspnv.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gzrujdwxg.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gdttwacjf.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gwrclcyzy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gnwwufmlw.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gndgftgft.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gljrvzaig.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gjvkimigg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gqpubasnd.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gtqzxeliu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gmqjveoct.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/geibqaaur.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gwiaslvfv.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/govzgexdg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/ghomaoegb.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gtrmdipql.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gaqfjmnle.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gdhrfrdeh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gbynlhdrx.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gpyqudgsh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gwixquspv.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gezzhmeeg.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gcrvarjxf.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gcqipxdqd.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gsagydlte.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gerdnozrg.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gksfjjvsh.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/goiqthtfy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/grxnptmxt.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gaoiqkczu.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/ggmmlgzpw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/groppawnm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gumhdzzsm.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/grfgbmzox.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gxjhsdjfg.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gqluojcgc.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/glzsuayba.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gybmjijzh.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gflzgavim.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/giewuwmrc.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gwykcajuj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnszsiizn.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gxfgydorj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfvgwchrv.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gsgutqhva.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gzyuukacv.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gllvwwoan.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gwbpvyxbx.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/ghvekzhfo.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/goxucfwpg.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gewqyicrq.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/grzfpogjd.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gzfmnyccw.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gsbmlhiwf.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gpmaasini.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gnwgedugr.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gxmhupuyp.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gmarhldai.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/ggdogsmfx.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/ghboerocn.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/ghvpndgih.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gfjcrdqks.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gjweswvuz.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gmieginxn.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gpoyigyec.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gqrpptapy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gmbzvluyb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gbmmwbjav.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gbmirgagk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gvmwftuwa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/glaemzxjz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/ghdmxqsdg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gvfwbbtth.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gblcluohf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gngzaagdg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/glxghmjnr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/graxcutqy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gpumxigtl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gnfxtvpac.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gesemcugj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gipdhnrwn.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/ghmcjwqaw.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gsdbrcoxt.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gieqzrfgp.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gghdjtgmc.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gifnvqawo.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gsanfpvfe.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/ggeyzxzqw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gnnmmcclm.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gpglprygh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gcctxmfdf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gxpapssxz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gydrolhik.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gosdladsg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gyjttankp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gupzxrwpl.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gmpauvusr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxntrzask.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gmnhptkbj.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/grobulbym.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glczljtnt.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gyvffwvkg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/gwvanadrj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/grdcgelty.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gcsshncku.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gnjpmuuuv.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gwdcglgny.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gptghcaew.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/ggjejihnt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gemxrzjnr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gtlzgnvta.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gfnjubmvy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gocyknmuk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/goyijyxql.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gpiubygss.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gdelgotob.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gwmgcfiyn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gzgsjhwzf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gqnbjcrri.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/gsemwfkhp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/ggrzdwpvi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/glfbbetfv.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gbraramfv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gacdyxwyy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gcppgrlbx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gaimitmut.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gbjvqygkd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/glqbtuvde.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gunhaxvrf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/ghaefzqrl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gtaskqgeu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gqpuxzrah.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gyzemxxmi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/ggjuluqfs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gqgkfrejo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gturqvhap.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gnxjewlip.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gcnbuvkkr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gdphozuyb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/glftkmamz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/gnujcdgjs.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gulqrefrt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/grslkqdpd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gorcldgaw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gvkwabacr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/garqswnlk.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gryllrhfm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glfdwaizj.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gagzvgmjt.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gxpzdydcv.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/goyphvxdm.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gssbtrtcq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gdlamrwpg.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gxnjpzayb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gpgbjyftq.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gkkyvrmci.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gpjewgtye.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gvwlwnpin.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/gsqoddpnc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gwxvsttde.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gwbizsvmg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/ghktcpkcn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gdptpkupy.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gpnakbumy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/ggpgrhgjs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gbmkcbdcc.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/grohbhtdr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gnetccauh.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gaikjsqgy.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/glvochgdp.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gjwhmuxsf.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gpkiljxej.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/grxmtdjzu.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gkbsmwcvl.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gctabwsma.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/gwwszzfqv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gkjcyldwy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.zdbjq.cn/Article/details/gykxjncge.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gnrmzgypu.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gapzqsbph.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gllbyiiom.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gkrgtnmjm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/grrssicnc.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/gdahkcmwv.sHtML

[A05] 整数除法与取模
来源：http://mobile.hesvh.cn/Article/details/gwendfpth.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gqtecqbpn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gnepmjqsv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gcrwhvhwm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gkjavqzgm.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gfttzggqb.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gemxqndzu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gxfcebjqq.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gupkdjqre.sHtML

[A06] 字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gnxbdnvxu.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gcdsrzapk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/gnulpveat.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/geycjiogx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gasxcrhls.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gktujszts.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/ghtbrcopp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gkfhhoerf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gaxrucode.sHtML

[A07] 数字转字符串
来源：http://blog.hesvh.cn/Article/details/gplsazrbx.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gazwfuqhm.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gradhizst.sHtML

JS:   String(42); (42).toString()
来源：http://blog.hesvh.cn/Article/details/gjgroovaa.sHtML

TS:   String(42)
来源：http://www.blog.zdbjq.cn/Article/details/gwkrpijsk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gmvfjantg.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.hesvh.cn/Article/details/gkjaibnxi.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gjdkiadqq.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gndrsfjqj.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/gxyrgpzvl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gzuuojosn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.zdbjq.cn/Article/details/gcballsnu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gueiffrex.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gheqsqbzs.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/grbtxqmnz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gbuvjxozi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.zdbjq.cn/Article/details/gykguzcez.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwrbpzpe.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fehbvm.com/Article/details/gimlfithi.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/grgdbzzbc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gicogcady.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gnjrztzkf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gzdjpdtxd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gmysocmdj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.hesvh.cn/Article/details/gqptdvydp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.zdbjq.cn/Article/details/gxzpjpmtz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/goflesund.sHtML


<!-- 参考信息 -->