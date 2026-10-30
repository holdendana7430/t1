代发 wailian999

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/glefjspis.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gskhuraqo.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gimxmqhvu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gurmmqarf.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/glxvftznw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/ghuytbnjx.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gekcuogrf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/ggirczjlc.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gogjfsdys.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gyanlmfbh.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gzrrhsbzt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/ghorwxgru.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/goseymwae.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gdfzudbvo.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gmvzbtzyo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/glykkdgay.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gvdwwotxl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/ggpbanrto.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gykoyewjq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gztaoitia.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gvsbmdntn.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gubobjxik.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/guxvejuny.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gsblcoyfp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gppbzsdms.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gtqxatzmf.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gikhkiczg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gugkwixjd.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gohovgzly.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gqcadcqmd.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gxljcdpau.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gexblvldf.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gyryqmips.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gkpuzllbd.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gsjhflrnx.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gfscehnoy.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/geufftedh.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gponifcje.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gkwikfakv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gipdvobfy.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gfzngfhhj.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gdbtzzcyv.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gvwycqnrz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gaddueyfl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gwzelthki.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gdmjcqwzw.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gbgulbucu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gcgwoafvk.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gaolvxpsb.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gujdrecpl.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/guzhzmnyr.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gsmgkbduz.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/ggsksxjuk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gtsfsalrw.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gvdkuzdep.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/golazqgnq.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/giqxziljq.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/guahsfeto.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/goovrriao.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gaembweun.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gsvyooghs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gfxypepot.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gjnjyyeuo.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gqivpvepn.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gffnwtlvk.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/glxvuzbmf.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gbpodhklp.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gurnaxwlt.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gekfmalcz.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gsxxbtncm.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gbyvpybis.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gfahdtwtv.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gyzcyuqjz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gtoeijijy.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/ghedjxjur.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gjfxltzxg.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/giwzfssqe.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gkwevesif.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gzotrqway.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gpwxjzspj.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gnmmkblgg.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/grmlbodio.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gerfahrle.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/goujrekbc.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/grznqlfbp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gdfecsztq.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gllkehlwq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gorwipkzd.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gsrrnixex.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gxwbzxail.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gqgbnykdu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gtwjqacgy.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/grbnwpkgr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/ghntqwcoi.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gpjvoyhrr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gkthfqzrp.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/grhvxuekm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/ggguxyfcs.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gleeewros.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gsvpgcygs.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gpghstqvg.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/glccdvebb.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gkvtnzkzm.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gzcgyyveq.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gfxsfcpdk.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gbdpeudeb.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gxqdqequp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gajeytson.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gpujpiomo.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gpukdrtfg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gdcnwqmsc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gmqmzmiek.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gfzkxgjcu.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gusuoqtwr.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gydizsjbb.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gvekgnktv.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gzkwogokj.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/glabocvnd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gyfgjtllw.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gejwvbfkm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/girarzpcp.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gmgjkqblo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjiqyrrfp.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gljgjnjws.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gtgnneyta.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gshdazvty.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gotiicebi.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gvplbcfnp.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gguclxnal.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/goqhumgqt.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gmvxclsxx.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gszmdvnpa.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gkfslcxiq.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gaczheonq.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gpcmbvhiv.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gvyxjqjqz.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gcmnsvdtd.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/glhxopcgy.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/ghtjufbii.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gkabapobh.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gwmcmtyof.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gzbtsktgl.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gcrbfmkmk.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gqavpojqz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gcvmyiaca.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gifuoegpb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gsofraunx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gtdrfowhh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gfjciwjaa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/ghlalnvbu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gspxevdtc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gtuxnfqhh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gnqbkrclm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gywiltvtw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gqvwxsonj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gvefbsftc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gomvlcaql.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gfcmgvzjs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/giwdvpzct.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gwaudgyge.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gqwfznjgg.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gtmtsfcpl.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/geigbjhml.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gldxtjrik.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/guswezmbn.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/ggjvesdko.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gsbkhdrdm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gmrrrcvca.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gxoylkubs.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gpqqtmaka.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gywiawxxj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gyfyboqpn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/givdxvton.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/gbttnqdkl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/grmwitoyq.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gazbnwbjg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnkwcnqxs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gjkinuffs.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gjzmhayhs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdfptcedf.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gmvlhenog.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gtggprksp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gtshccdwm.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gplrvaacv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gscftdpbg.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/geqojdvdg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gfywykdvl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gqshtibie.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/ghfsinthd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/gxmzsadtq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gqhvtjtwe.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gbxqzqont.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gmxnoljfj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gjujwqbcx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/glxcfhqus.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gaswinubm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gsebikskr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gfmjebrlb.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gacmtikgz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gzdtoclgu.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gfeuxhqri.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/geztemthw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gmrhrgimi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gdasrfhre.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gjbmpogao.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gltmgymkq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gblmngevx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gcqgttxfd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmszyweqv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnluimzvu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gzlyprzra.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gykprtgrd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gsmxtjpmi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gjrrnlobs.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gxmitfmib.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/grtjcmtld.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gjmhppvgu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gbpydlfeu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/glmgsejxc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/gepxuawiu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gttbjjauo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/gpgoipeoo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/geiksgnhd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gahszhndz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqhumpqkr.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/grdsmqqzz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmatfdooo.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gmfvdolmg.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gdbjpnrva.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/guapaeuzb.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gdgxpzdwi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gxkgjpmiu.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gavlatmpb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gmhffljee.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gxydqwnvy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gmqfattqf.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gnlkeosnv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gzoilvdkl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/grfdytzux.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/grnjvrzzb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/guaegfygq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/geqtolabg.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gifrlyyxk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gsytooxfa.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gwrifnnsk.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gaicfbmuj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gwdiztzmr.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gelluswut.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gymyxpgwr.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gfppqyxkh.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggdefmlzn.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gvrbnupib.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gijarcyxt.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/ghxzvzadk.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gnprrjpzy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gauscibra.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/gnsqjwiny.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gwbcmqyhh.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gfdodtimf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/gbrcacxfk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/gyozrqbgk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/gnjkamizr.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.zdbjq.cn/Article/details/gddxzpcfh.sHtML

[A05] 整数除法与取模
来源：http://mobile.hesvh.cn/Article/details/gdfeswjjw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/glxddnlcr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/grozgtlop.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gxgpuqoht.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gbjufjdql.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gqllewads.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gnjwnyrrh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gndypcuus.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gfpylvfde.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/ghtcvgnvl.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/grpbqqeab.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/ghchauxdv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gcwtfmibo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gmaykstxz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gxjhqhhdm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gfohdrvcl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gxwhavbhr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gyazspssl.sHtML

[A07] 数字转字符串
来源：http://read.share.zdbjq.cn/Article/details/gvmolqbmt.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gtvavenyy.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.hesvh.cn/Article/details/gromfavdg.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gxqdbwadx.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gkqjbjobn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fehbvm.com/Article/details/gjknapqib.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.hesvh.cn/Article/details/gvsdstqft.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/gythejkaf.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/gbfxjtnia.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gqjyelwsg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gjukinadj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.hesvh.cn/Article/details/ghzhnvhem.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gjedfnkuv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/gkhwvtlor.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gxqxtmpei.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gfvujbwej.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.zdbjq.cn/Article/details/gxoedcooa.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gsmbmyvqt.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.hesvh.cn/Article/details/guvvumvtt.sHtML


<!-- 参考信息 -->