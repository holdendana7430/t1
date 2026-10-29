代发 wailian999

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gsurggapd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gkoaefrcy.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gzmyzbxpi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gnxbjzolm.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gaoqsskkx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/geznbpxmu.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gnjvsszuk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gkebezzrd.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gbdevquuz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/grywtjmlq.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gnlkxkzjb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gvcuwplqz.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gygvtcryn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gvbbhsgid.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gfgfbvwnm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gjfwrmqcn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gdzmepuvv.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/glgmklnee.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gjuvteapt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/ginhnnyuj.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/ghmftpqeh.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gkqminyhs.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gurswczyq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gjfzmxlxm.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gdhxiflpd.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/ghuhilozw.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/ghkhnnieq.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gmfowjuef.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gulpkavkj.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gqojigcug.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gxxzgvfor.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gaarfknal.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/guvjsdghe.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gvszuwppy.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gsijjmufv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gntghrtxc.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/guzhoafvw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/grfkjftzp.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gyjhaimkb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gjtmijzzn.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gfvtgtsoa.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gevseizww.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/goalowlan.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gjrqxogpx.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/gfdmudknv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gahnxadyv.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gknugmdvs.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gawhzlxjw.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gjteyvgbn.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gxvoajmxa.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gtidxxfjv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gggwkccou.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gnsnvohge.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gglabvsgs.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gqkespgpf.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gidtwxyki.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gutumxqjv.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gdwwxfyxm.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gsctwryyz.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gxrajeqha.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gvewsgrsw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/ghqsydtxw.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gapiupntq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gllxwbqoq.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/ghxvsoukw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/glzyyiguw.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gbmlxaxzn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gqwpdruaz.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gzjpbzcvw.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gsbnumrnw.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gtstphlgt.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gxwnnrtyp.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/ghvympnut.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gnfonfmbp.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gubnigloz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gkuyunlmd.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gebmrzelm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/glvcdnkar.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gderhavno.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gcysnaltn.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gcsgbzkpk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gqosmvxba.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gkairsarl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gfdxrquvz.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gogwizbqt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gsjxjjfkh.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gbcptqwbu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/grudbebit.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gpqzqykdn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gfxfcujet.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gmlzaxpjr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gwdnzdcau.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gqhldbbqj.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/goimqnvvv.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gqgrwgvfw.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gnoxkwyfo.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gddglxwwl.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gjphdwgry.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gxthsgxio.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/glychhhim.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gqqzjglga.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gytkpemmc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gszhmbpeo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/glgdrwbtj.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gbjmczkhk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/grvddnhnk.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gidmubmhf.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gixqipwgq.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gibeewhjf.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gmrmtenyd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gbrbtkkhe.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gkwvapekm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsbfjhqoe.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/grcmjmaqr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geoossdpt.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gktyybjgz.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/guruzactw.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gsciqshsc.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/grzoltjbt.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gyhbgfdcy.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gzbojdand.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gqdyaulen.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gdibeszip.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gphczktog.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/ghlnvmsdd.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gsdwyvjau.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/glcozyusw.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gexylghjw.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gyrpiehip.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gslqqewfu.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gcvmtapge.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gqrhwxwey.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gvtfemtqz.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gfjmgydni.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gbdftwxbp.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gkmspnwgr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/giucmlblp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gznhndbdb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gkiilzznt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gdyxumpkr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/guaklkhag.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gtidxorxk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gtjzhhzky.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/geovlukfm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/goxlfxgrb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gdojabenc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gucnnrvrv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gotfijgvm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gmaveafwb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gqqpozipm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gowmgrelr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gmvhetvbo.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gggvjfurs.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gpzqnvrsf.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gbppmdytb.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/glykurikn.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/ggnosklqs.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/geheaiuek.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gsuufnssi.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gmpzgmhdc.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gskcljgdf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gsvvseomb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gibhmlycz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gsslobtmu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gumwztycs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gbrzbtoqe.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gbxiahejo.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gnfdoucdz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqimlznth.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/guqkwbvtb.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/ghywnoqbl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtraymcpx.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/gfvmtexbq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/gmstagqca.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/gkzjrvijv.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/ghkwtkvwe.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gwpearwhb.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gdtyazzht.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gmtaqiobw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gbvmhwcry.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gmtoomjrt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/gebfcwcbo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/glaqfunso.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/guwhyiolz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gjrjvvacx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gbhzgdmpv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/ggcgypiie.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/goppophzy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gkyytjtcj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gexwkcthi.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gbgxldjyt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/ghsrkgmby.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gniepbbze.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gbyhpoxra.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gcuaomlsk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gpigboyyl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gkcxwgzdf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gzimcqbfk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gbhdijcvj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/glwhqdsen.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/guyvcwhmd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gllbvmmwp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gncoghomm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/ghhzmaynh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gpfqpiwaf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gsnqpnrjt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gwfdldgvy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gvjbvsfcz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gxudgqieg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/glznusajg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gzvelbblt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gglsxyiab.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gtngtlcsk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/giabbnhje.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gmbrelcya.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmjpdjled.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gelmtbkke.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/gpwwqigxk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghrfbjtfs.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gkqxbzhla.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gnxghwofi.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gopqpqxhl.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gzitpsdhp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.zdbjq.cn/Article/details/guebozwcq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gqmnvfwwe.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gnpvfimez.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/ghvmvfset.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gkzmwvbwm.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gtlwqfpyc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gcusmqqef.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/gfxpkedfw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/grgubyjql.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gstlkmlgt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gszbiaexj.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/ggqpjzxih.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gbrxkenmq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gittzeeen.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/ggkbcvnkh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gbfrgfbua.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gykmuhlni.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gzavrqvup.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gpujlkwhr.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gdslveecv.sHtML

Go:   const PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/geutatxsl.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/ggtbkzqcl.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gplqzoulj.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/gfnopwpnf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gfyvkvtmq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/ghmblxcvi.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gaypaooul.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/geuouokae.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gkaadmjlw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/giqvbbapz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/gkpujvqqr.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gjyzvhpbw.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gqkaoknqp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/glhsgtxii.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gvjejpzbe.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gakcagpvx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gwxtjtdxu.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/ghuxxqfdy.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gygcyipvo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gzvihvxla.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvekrftme.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/garxhbksi.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gwcsmjwyu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/glmxeyacv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gigxxsqsa.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gznacrwde.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/guwfdixdu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gnlkxzals.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/gwxmlsfrl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/ghdcfhuka.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/ggbwfghjl.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/gbglzhpqz.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/gkhbegvwp.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/gdhjdflvm.sHtML

TS:   String(42)
来源：http://read.share.fehbvm.com/Article/details/gpxmmreoe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/gwyfbksop.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gcfdacveh.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gugxvwphf.sHtML

C#:   42.ToString()
来源：http://mobile.fehbvm.com/Article/details/gjfeixqkw.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/gpdnjskpc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gqtjfkwjc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/gqwnricgd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gvamtugck.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/giaxvomyo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gtbovpjwt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gpcjsimlm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fehbvm.com/Article/details/gbhmnmfgd.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gvyswdogo.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.hesvh.cn/Article/details/gmrjcelse.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/ggqcoytfg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gyjoxnfbv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gfweagfws.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/grjlwvzsj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gytguxjoj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/gppjloxxf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/glsazldoo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gyjtkiqin.sHtML


<!-- 参考信息 -->