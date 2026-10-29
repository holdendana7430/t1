代发 wailian999

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gvxhvqtao.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/genlnvixk.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/govqutpwt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gudohszrc.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gdmdqkqut.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gzltpxzrl.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/geeuxisie.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gcetefmcd.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gavwwtcdl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gxgprdpgu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gejxtmgtz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gwacvbgii.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gcqgcnjuz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/glehjlfta.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/glbergyzq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gqjolobfz.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gsqgpyrki.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gbxmjidvc.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gjkegafxx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gufpcgwlm.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gcaojeztk.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gsawxfxsl.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gtpewtsyr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gbqotvvjq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gjmbxawcu.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/grzbgdocg.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gvtfjvlfg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gbotywzcc.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gpwfyuure.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/ghxbcqcae.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gxtffmrib.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gxfoanyer.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gbffjwvrp.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gbaekftnb.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gbxtjawco.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gauhooeyb.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gzbqqrrnh.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/guhblyhle.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gwsgouows.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/ghacdayvh.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gzvhysjgu.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gygbskmqm.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gqzvrtjms.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gvsqkaaec.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gmvekeyug.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gyeyxokht.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/ggjqlaull.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gmtjdbudi.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gzjflksuj.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/guxalinmr.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/grkvyfltz.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/ghrgvmovn.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gqemoixda.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gcxyiegzq.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gpogivzix.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/ghyqrylov.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gtjbmsrbk.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gnrrjygyx.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gcewndevc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gperdukaz.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gfgqenhmx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gzgzdrvnc.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gxbcotkyd.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gerhhioox.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/giaqzsaor.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/glzckqyfj.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gfhjhroyh.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gtyxlrngu.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gahzabikt.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gmqyhhkvl.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gjyozaofk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gsilqhoqu.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/guzbetaej.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gdfvzoxgz.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gkxrgbdis.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gzrcsxaqb.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gkkpreecs.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gcpmditnw.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gazkotupq.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gczchblpc.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/glzgzlxxq.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/girywdpnh.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gnhnkiqow.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gcyuepmli.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/ganqkgdaz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gyspobuwp.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gkiwyvmrg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gfetfbmib.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gxhvdelzi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/goombwukb.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gswkvqvty.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gcbbabglg.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/giwwcjaqr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gxsdfzzdw.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gpmhagrbt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gerxnvhlu.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gyvtrqbyk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gdvairzux.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/glnrntkdf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gwmtxqbpf.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gsshovmez.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gaylkfrlq.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gryrbvbha.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gwlpjaryj.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/grghkrlvn.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/glxxmhxjt.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gjdpakrcd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gkeksbdgt.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/ghgllmdfp.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/ghhrtcwgj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gbzjqyxer.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqbomvknj.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gegnggcaf.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gdbfceydf.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gcttbgrdk.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gwehcvldy.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gjdjbmqad.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gqlqhqyqp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gycwaephg.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/ghthfhfuw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvretvain.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/ghurkells.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxyocwncm.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/ghyefehju.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gorowejbu.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/giiokvnmb.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gzgvzbngw.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/grsyziedj.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gnltdwdfb.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/ggqaaewkt.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gmexsxlqe.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/giyikoybz.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gwtsatkgb.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gcoyfimlf.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gmaavysmv.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gpbktiiso.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gscvfwhap.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gcrjjwics.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gjduvcame.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gdkyoicaa.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gkenrnsud.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/grlghiodi.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/ggvrwjaju.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/guwybkirq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gilkjkdjk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gkpbvtvir.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gkicvcrom.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gsozulsbo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gajrlhfmk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gjmcnnofa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gsfzmnjqg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gdlednghd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gqdmeruyy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gtealxgtx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gqdoakwse.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/geojtnpyl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gnvabpohp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gjpaexygb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gpgypavwe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gxwmltupg.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gnvgepdjo.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/grztoetni.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/getybhyup.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gyzycxlom.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/glmkndpxv.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gvuggrjlm.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/ghsqjtlmz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gayqmnzba.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gpeihngcu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gkkjtmjdm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gypqxnslj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gkxauunlx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gukomldjs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gdjeithia.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gmxhidmtv.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gbohgxhwn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmtetzwfj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gkjjllpvn.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gaexupknx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gubimpjvz.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gryelaefn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gazlsbtcr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gdztjstrz.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gfnudkptf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gaovsnxuu.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gxaockbyk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/gkeqefxxw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gochtcoox.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gowtvwtwj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/guzdjqxgb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gptumbrxb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gxeodjgwn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gqylatiiy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gktpiaxqb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gtappsbdt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/gcuvoypca.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gisbqpgzc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gvqcfjmxc.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gsztffxtg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gtmhrfrqf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gmjgpphia.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gibmsnbhh.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gxomdibpp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gqenoyhne.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gqyteocxw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gpbpafvia.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gypcyxdpm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gjpbwheiu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gaexrjkkd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gtjgvswhc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gxqrgqyba.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfcibrgup.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gijqzxrzz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gquuzbrxo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gxhnnshlq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gnxhhvzuq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gcypcffmy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/gczpwovpf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gylisnzot.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gmmldpckx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gqohczeid.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gkfjcgzgb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/ghrwvtllr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gxkjrktjk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goqvexfln.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gxijuhlbz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmnkbyzle.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gydituffm.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gufbujkyh.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gpaslvmgc.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gahltkstl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gudbkofoi.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gskfjfquu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gduegslyk.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gqjrpavcr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gcyoupjif.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gffukqfzq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gsckwtrdi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gympignmu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gdixjdyhj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gmhiprxrj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gczuhuxye.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/gsrlhgbnv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gjkokfznv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gxdmmxrdf.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/gzdizwquu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/gvrhebdnw.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gtkatlakf.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gathuucpc.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gpvotlgnj.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gphynjwcm.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/glmzwbglc.sHtML

Ruby: PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gdjkgbkcr.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gwpfuprdn.sHtML

[A04] 判断变量类型
来源：http://blog.hesvh.cn/Article/details/ghijxjhcy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fehbvm.com/Article/details/gebucpiwv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/giahwvfzn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gexncbogq.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gbgjwyhyj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/glkhimxis.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/ggamwmjgt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/ghmtozpvy.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/gfvvbevzh.sHtML

[A05] 整数除法与取模
来源：http://www.blog.zdbjq.cn/Article/details/gxvqjvzva.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/galkuerml.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gqwsekafi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gymokzrzw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/giwrhjapg.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gkhzvptew.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/glzmdvwnn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/guktxhrwy.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gfesqtujv.sHtML

[A06] 字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gndlfgmoj.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/ghowzmurq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gvubxlnrn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gtvgfacnd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gdvdkvorq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gvqlntbjx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fehbvm.com/Article/details/gtwmguvcd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fehbvm.com/Article/details/gfomyntwt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/giuzkxfaw.sHtML

[A07] 数字转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbizxmhyk.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gblggpgbv.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/gyddzeocg.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/gqzlosfuu.sHtML

TS:   String(42)
来源：http://baike.zdbjq.cn/Article/details/gpejiacqt.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gzqctzubu.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.zdbjq.cn/Article/details/gsnoemvik.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/gypabdriq.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gkywxcelw.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/gymzfzuhw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gebkpatvo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/glbrcrjdd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gvpghzymu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fehbvm.com/Article/details/gblthlsgl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gpxozcyzv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gzgcpuvwk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.zdbjq.cn/Article/details/gyspycaik.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gbekghhjn.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gogqripwe.sHtML


<!-- 参考信息 -->