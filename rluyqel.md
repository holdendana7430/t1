代发 wailian999

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gkxijynls.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/goveirhya.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gryvntlqf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gwetrgmrc.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gxgegtjlo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gldfiufmw.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gbuphjyph.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gvsiqpjre.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gpfkggdxs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gqzxeavui.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gknurugya.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gutoslqpp.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gqrknyqhk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/gqdjloovz.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gyisqbuhn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gznzqudhh.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gmskkqwqv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gylsdamyn.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gidrqijca.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gzrzxxkxv.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gpxsxbmwz.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/glyegkvep.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gknaljkwy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gyrccpixq.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gibqlbcxs.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gwlulspth.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/ghkulyjuu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gyehlqncf.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gjdsdortb.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/ggrthqplb.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gnqgyytqf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gpjnohoeb.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gwcdkvnbl.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gprllftor.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gpivkoggl.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gdtbfcsth.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gnjwgqzvn.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gzhebbler.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gibrhtxib.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gxbbmugrq.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gyuudfdpj.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gchlvxnsn.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gokcobddz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gwfqztvst.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gxqzixlae.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gwvuadhtu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gumxjcbzn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gpipioleg.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gxgjytncl.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gtrukneul.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gobfstnyt.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/guaeomlcc.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/guefwxwrm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gjmhkdxeb.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gtedtvdcm.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gxgsorbiw.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gljscxqyt.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gxbjpehfn.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gseimghfp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gdgloifyk.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gblxbwujz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gntrgqgdv.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gcnrmmrrs.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gnylchasw.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gtpytnzsp.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gazppctea.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqghcvgdm.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gemhvidxa.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gjdlofzru.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/ghyxwhxxs.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gfrpzqeqf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gdozvqqxn.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gmdthtvkm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/ggyxhrruy.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gtnkqcezh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gawcfgnby.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gkxvrxixp.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gsxutxgdg.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gatiawgjq.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gqaphoobx.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/ghxhsqykj.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gkhefcezc.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gxjgumrda.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gconukubj.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/ghhkwdznp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/grcittneh.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gtwypsqro.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gtarjwfds.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gctfuysjl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/grramdnsu.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/godchulpq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gxuuykbif.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gxkylttfn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gcypuzekc.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gbupidwke.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/givyaokba.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gbhmmibyz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gcelenafw.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/grajmwwqt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gknvnkpbo.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gchypotre.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gzoahqzmn.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gfiacxjku.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/grmorbjnu.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/ggnghhuyi.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gstdyibar.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gdjojvyzq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gvujbpudp.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gqjaffvfx.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/googmtmjm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gwpizfphv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gucenjjaj.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gxrrzyebu.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gpdonlufr.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/grojizyps.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/ghkeuvcgg.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gwxasyqhe.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gstrxwtui.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gtjfzgrij.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gyyzszavw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghcywthuw.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gxrtimrui.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpulukczk.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gjjamchuo.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gdmgrzbla.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/ghddnmztb.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gvptcxufd.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gkcisxtmv.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gvmxfarhx.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gqvwnedfh.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gaiwahcse.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gsojkqlct.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/ghmclhcfc.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gvnepgubk.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gdzfwfnjj.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gykfjahut.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gdkujzvvf.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gfobaahqm.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gyyometcb.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/glgjaspgy.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/glrezblmb.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gtxabmook.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gtllsgltb.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gzxcbtxvq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gdvfshlbg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gdevlfcce.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/glixbifhn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gpjoigkpz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gtqxotuhu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gjbvaevyo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gifwnfhwz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/glggtnpkq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gjspwnlmg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gcnwcfqkd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gdvyzhjhz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gnupmmlkw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gxceveclo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gmjtyghgv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gtppstnkd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/grxdosfsw.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/giytrkgbg.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/gnyayzbco.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gigabbfvp.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gwqbbzeiu.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gziqkennu.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/giqdocsdn.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gnpjoyilj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gboznnlhd.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gpmbkhebt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/guaulopxo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gzihvawao.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gmzdwdlzv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gojkppzux.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gcqoixulq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gzpxpupns.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gbsoyydyx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghnixszfe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gbrmazavv.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gvdybfyug.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gskhcgzep.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/ghxttbvcn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gsosweqvu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gbkgyvtkp.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gxqdtgtfb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.hesvh.cn/Article/details/gcfnegolk.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/guvvuyyus.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gmggilttz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gzfuzuopk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/giryesaml.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gmqmlvxeg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gxxiqmbwz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gvowgzzvf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gmxxfjstr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gojdfcjlh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/gtyvosnhn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gecpuwfyt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gxmqymbud.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gklkbtxbx.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/gtaujgrga.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gbceayznw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gkbsbqdwi.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gcyjrnvvl.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gsceqxxxo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/grhrhkqjs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxcktddse.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gxbfdsetg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gwysvplfj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gdmfbuibs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gmbnzuefs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gdjvafpdt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gpttcgseb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gzhhrzuxi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gtumijrbc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gkxlormmg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gsouqxqqj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gtezhmjmk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gfmupgmpj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/grmaujujd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gzfflsegf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gnrgquelb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gbmyhldkz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/ghiycyipx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gjgzuvzvx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gxmalbmkg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqysiluba.sHtML

A. 基础语法与类型
来源：http://www.m.share.zdbjq.cn/Article/details/gkzmpkuet.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghcxliyrv.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gdqlbbxvz.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gfqjqhcta.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/ggfdmguti.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gphipsykz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/ghskohnyg.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gwiondavp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/giluastxb.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gtswpmlup.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gyxufwyvd.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gryegkqxh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/gyxjbhemk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gufzvwwff.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gqtzetlpl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/ghiyyobga.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gifjmhiyg.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gegacoksl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fehbvm.com/Article/details/gtgpztslq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gmsszrpki.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gcdbenlth.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/gzxtgqslk.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gfzxlmuqj.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gpnrelfhh.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gqymgjcyv.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gybjiycsv.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/guyamwrui.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gqmkawgye.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gokodkied.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gcgxnkiun.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gbmvfkjfv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/gcnsdvabq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gnzqlzkew.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/grgwjbuab.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gojrpokmx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gzieygxcr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/ghspfwirl.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/grqpxgars.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gnjeyjdmp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gnovogluh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gwdwaeihe.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gcyylyozu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gpqinbkez.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/ghqyvzxlu.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gotdztsgo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gabieseor.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gkyxbrlrg.sHtML

[A06] 字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gukznccnf.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gtfhkvpbp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/gdcnnosky.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gmiioqvsj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gmzqyawwo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gqwiwsiyf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/grhcsddyv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.hesvh.cn/Article/details/gwmvthqzc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gwkipipok.sHtML

[A07] 数字转字符串
来源：http://blog.zdbjq.cn/Article/details/gnvlzcktv.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gphoqzlhw.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/gezoukpsw.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/gjirymhvz.sHtML

TS:   String(42)
来源：http://mobile.zdbjq.cn/Article/details/gwxltarig.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/gulyizxqw.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/ggynkinvk.sHtML

Ruby: 42.to_s
来源：http://www.m.share.hesvh.cn/Article/details/gqdylhmqp.sHtML

C#:   42.ToString()
来源：http://3g.fehbvm.com/Article/details/gpykkjabj.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/gdvhiamga.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gcuvnlwsz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/giusbnzlm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/guzkobeuw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfqhuuxr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gsvhvwppy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gfyzeomlx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/gvypgkaof.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gwfqtczpq.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gulerweqh.sHtML


<!-- 参考信息 -->