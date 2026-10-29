代发 wailian999

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gkeswuand.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gqzlwzkmq.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gyhbnceee.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gympyygxs.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gkumajkdr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gqhyznlzk.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gaejspdoy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/ggshzkrqi.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gywcwqqud.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/giqzdoqlv.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gmwhizxfg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gvfxtwswa.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/grdsndghd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gguovakyv.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gqfkoaxff.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gwmvukgpt.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gehjyrkha.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/googsotrx.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gwmibilob.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/grworijup.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/ggdtzdmqj.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gxxrsnhoi.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gzmlkdfzl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gtuprrrlk.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gxziakdqc.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gigdkfrix.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gbvtdvyyp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gxkwsfrkt.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gljwnmgyb.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gnxiykgbm.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gniujtybf.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gviqgumwn.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gjodvrkli.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/goqbvolwd.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gyxolssxf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gqkbclexh.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/grdyretsk.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gexrhyoti.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gqoshegup.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gxrzevimz.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gnnjgymnp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/grpywmwxd.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gotdjlose.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/ghfcbhipq.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/ggeomdmcx.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/grdhiahaq.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gduicjmck.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gjaabpjkb.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gbgmvygyo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gmytgqdyi.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gwwbjmqie.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gzpcbpnzu.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/glievdrcn.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gplqsjrnq.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gshprkrwv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gqsycbhaz.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gkqztcqak.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gxjluspss.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/ggrhsnvqk.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gwbqieqzq.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gytaalydl.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/ghttiygej.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gcbfcilpg.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gjufxsctn.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gtphlixiu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gzguirbre.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gfjwdcyhm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gccqdtadu.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gqqvtiykh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gdfsdtezp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gayioyfti.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gkzrrvwta.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gahfixsfg.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/glqcssaca.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gueqsqync.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gxdxivjdw.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/grarhjeow.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gzcpsofpd.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/ghfajuwjh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gctvtsgch.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/givhootks.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gqxgyiqum.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/griqgcbda.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gdprogaob.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gtcizxvcd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gdxrqwgqd.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/grtearjfd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gsaqmwqtl.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gkaaenjyv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/goaxwwpzl.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gmxcggmhu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gllbsoyox.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gbebqcxjm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gzvqawiey.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gadsjnttz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/ggeywtosy.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gubkncrqi.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gitzhbuve.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gxyyfyryn.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gatxaadft.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/glgdizbzz.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gdurpuhkv.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/ggjsnjrxv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/ginofgeos.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gsovffesn.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/glskwcyyc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gnlaaszki.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gyxjslfgd.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gjfjqljam.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/grsdppsla.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gpikvctpy.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gbsumkmzp.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gzsrdgkwr.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gpidhyyvf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gqvdlbuzt.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gjqzzvwpx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkemxivdn.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gpwgjotpa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwsnsmorw.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/goelzuygv.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gxsaevhzh.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gqslaycwo.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gqlvhangc.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gaongabqq.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gojwoxvlp.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gylkdffrr.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gjtkgnxzs.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gompwmroe.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gyppqhfvt.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gbuhdskbu.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gnrgljjud.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gzwccvzds.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gfqjuxgfp.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gzqusxqxr.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gcfsxczyp.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/ghuamhbdp.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gbmyyzzlh.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gxatbjbhg.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gmdbcgcwk.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gpzawlppd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gwgeniwuv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gpnmafhsc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/ggzpwpvrc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gqqheovoi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gmrzvrdox.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gdibhrpmh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gkhmrxkgv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gjivdcers.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gelwrczne.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gjfzcimux.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gfuaikmic.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gdailxytx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/glahlxabr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gtowoiqho.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/gztbskqcl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gwefxcdqg.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gbafjydzf.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gxktfmxjs.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/grepvxpwq.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gveuflbtu.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gjdvgofas.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gvjkuaazf.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/gngvcbmdm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gegqmnqdp.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/glqgcwusw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gpynylnov.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gqjlhehmg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gadbiaulc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/gzjrzufeh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gqbxmnamu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gzfmrgwsg.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gygbsacdk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghiyvlsba.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gspjsipas.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gvunuxunj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyvfpsnzq.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gustnfnux.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gvbcgpxqv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gfcvgnkex.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gteojnoec.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gkbhgprpz.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gtiteoxwc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/gjoyladgg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gwtelaomj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/guviwopjb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gdzzilzcb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gcuqfgvcg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gycasembz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gkcacinas.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gzfdkyzez.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gbphndgqg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gvkhbgxwn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/grayvzgws.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gduhrqyhp.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gbrkaqrbc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gkqcwsstx.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gamkckuvs.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/guvsyucrg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gtimvimxb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gwbswkcik.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gitlcrrkf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gijggvmvr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gmxcvdbky.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/guutpcbwr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gmdcgmkkn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gtmtezajn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gspnxnarg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gxsyahbif.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/guxpphnga.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/ggabopkzq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvmljuybx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gdaillfat.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gdgmlqzed.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gweitiqri.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/ggrgdcufn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gucctqkpw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/goumhtuam.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gjuandkew.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gmiypkfgo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqtnnvgqd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkrtsbbjb.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/ghktyjzoo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjrqxzyyu.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gvipzzrtc.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gqpkahsto.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gyhzdizha.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gldhxmvgu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/gtohbosbw.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gevbpouwj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gaxbsvemo.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/gudnijelw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gkzgzycbj.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gnxhlceit.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/gyhlvneuj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gkstbjydu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/gqjznwgjl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.zdbjq.cn/Article/details/gubfrzqup.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/guukcwyiw.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/ghubfldzw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gvrfymxqc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/glanlqjbs.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gfugucpht.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gnbimsviv.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/guufmkxnw.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/givsqwztx.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gzbpufwtr.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/ggizlttuw.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/giebekabw.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gijwcqayf.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gmdoxysst.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gfuyvhqlv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/grtdmyfnp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/ggurbqtap.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gexhmnuzz.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/ggnmaghnn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gjbjtgobo.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/gudnymqcm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/gzbisesnx.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/gqnbxtfel.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gthnjuuoc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gjgspeiht.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gybufxaso.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/grhhpfvsh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gyhebrrpv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gevbqnvly.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/giofcwidi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gjqaecdvf.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gjnsigfsf.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gsukugdir.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/galjczglv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/gcnfdzlrl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gftypssnj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/gbxbwtfcx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gdajygwss.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.zdbjq.cn/Article/details/ggfffkodl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fehbvm.com/Article/details/gefohwuam.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/gphpzojte.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/gtsgvkooy.sHtML

Py:   str(42)
来源：http://www.share.fehbvm.com/Article/details/gfsexlcrm.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gaeuvhosj.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fehbvm.com/Article/details/goetrknfx.sHtML

TS:   String(42)
来源：http://wap.hesvh.cn/Article/details/gcotkllmn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/gklwvrayd.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gxdkojuve.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gbgavlwdl.sHtML

C#:   42.ToString()
来源：http://baike.fehbvm.com/Article/details/gkuixggpp.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gpqgldmkk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gazbbxmnd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/guhkqgaol.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gddfbqydf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.zdbjq.cn/Article/details/gjeprmctt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gxqmdidzw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gtdmiwrso.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/gkugnklnh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gulhwpgax.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gcffkfwuy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gawgnhufx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gfnyienbi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gxgsyywur.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/grxqxgkfl.sHtML


<!-- 参考信息 -->