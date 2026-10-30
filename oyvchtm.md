代发 wailian999

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gqkkzcdss.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gldknscsx.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gjwfsslbu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gmvpungtq.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gybpqvlbu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gvhhxrnvr.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gonpigteq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gduggasjf.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/goqzwaabz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gnbaujjeb.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gtdcxfthk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gkhenwzoq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gtkybpuil.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gscapfqbe.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gcwwqcnqq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gzrgxqhcz.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gepcpbqtc.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/guauqrpov.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gxvbqckpt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gkuyytxqi.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gtuljlksu.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gajnilcva.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/ghlnrtslu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gddvtfcfg.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gniyjszzl.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gjkrehqst.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gouodvfcz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gkindeiaa.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gudnwbnpr.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gqlvlwxep.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gmokxiehj.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gwnwrazrt.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gtadmhcts.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gtamyakbf.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gjyaepsae.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gtlqyjpra.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gwzcsigmu.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gachmktdx.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/giolhhlxn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/ghjwfuyvc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gncfahcts.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gwekspvln.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/grlxczdcs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gdqirrmxh.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gnykfnvwp.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/ggaaltdpg.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gifrfcirg.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gdldovkjf.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gxmqbnzbq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gktdnilno.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gjpsjkxtj.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gvkttryuj.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gqwvkfygr.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gzjqcfzau.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gvwxnrrqp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gcmqvhcgj.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/guiusffrv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gwgzcefpf.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gshsfqdzd.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gdpetnwfm.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gfgrxfbnw.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gxvtzppsp.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gyeyrchte.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gymgfjxmr.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/glrrqtwey.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gjjsvbamw.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gdqijkdxx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gnwyqjlig.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gyylwfbzl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/grbbakyqb.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gyhmsrwyc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gpmtzjtre.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gqudxmtkf.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/grtmcvgcn.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gtbxbnmtk.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gqxjbfpor.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gnbtbjkzf.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/grvyagipa.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gnseinhxg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gbhwpnapr.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gxmgjybbg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/guhdywzwq.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/geaxwrxab.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/glorwuuis.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gucyibgva.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gyvzkzhwl.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/garxxoake.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gjfmaoqia.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gdmjwemjs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gbchuypde.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gdcpkzvpv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gwvfvcfhq.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gsgjagbya.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gfcdxembz.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gdxosnikk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gnxbkdcgb.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gihqpbdtl.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gvuprzzfm.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gkghirsir.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gvvhjtzjx.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gnqkmxjkx.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gpoteocbb.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gqdufuplz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gipmufafj.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gvgdeuwjl.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gytbvbffl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gcnxnvjoe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gktbwvwoi.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gzxqlsqqb.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gngmeleym.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gnlqnckmf.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gvfuohgoy.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gwuvrcoex.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gcnmiqqoc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gjorvvyyp.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gmdbagmzi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcvhxgsst.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gbrgyyfnp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gixammczo.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gvixjojni.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gysrsintw.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gzhepvtew.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gcyvwbnwf.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gmqgimcfi.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gfrzloxnk.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/garoavizd.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gmpbbmybt.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gznkonccr.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/guuiavzwg.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gmzqemmza.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gglksojmc.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gfvfxsncz.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gudwxdwlc.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gyhhbjicj.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gzmvrnljn.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gyxwmxtkh.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gfasupxqr.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gingsekhq.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gmrbmpwzk.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gqjmuxyfk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/ghjfjtgex.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gcuzhpldx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gwmsmmuzc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gzulxjkfe.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gqaadbcum.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gtsiinapy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/glrheblbz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/grmlaviqq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gyxcutevv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gcdcjnxha.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gefwjjysg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gvgzmfadd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gnbgykevk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gfxwuqoiz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gykprfweu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gjwxanaoj.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/granslbog.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gzvpfsapo.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gfahtophq.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/geifkljpz.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/ggaaysjtj.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gqhfffomi.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gdfqdksmg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gdzgtcuiw.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gkcusylvh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gwmbiwlnf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/ghllpvfut.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gfbomlhay.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gmyilcysu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gxhxtwapy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/guurwxffd.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gqzhpgvoo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvxujvqvm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/ggudehznr.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/geyjcycbs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpfyidquo.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gkakhtuja.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gjttbfkzy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gvhveitoo.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gcpxfests.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gijmmlmky.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gsiotzwso.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/geghyianx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/gtrdhzuvc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/gmthxnjuo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gldglkspa.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gnujrdrrq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gkofjhgnp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gaewedhct.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gyknawqfk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gftoentwe.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gbzrjuiut.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gzxlmsrab.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/ghyocixlt.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gwjcxpnpd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/girtqnfpk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gobbkfsvz.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gimggwixc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gxkxiparf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/grfoxhrkz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gogjsjgll.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gevxravxg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gqvhyoeqz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gdytkuivg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gyjvekdrw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdsdjviwh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzpawtszf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gfcivquhs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gmwdqqrfh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gkisbbnfo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gzyijefxa.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/giiwsmikg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grgwllkno.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/geyojtceu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/guhpuupyn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxnzzmvyg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gikjqampg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gzcmcaxwr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gcaidxhuo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gnngcubia.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmtxrxory.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gzwsabdnf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guqdsljuo.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gihpworje.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gycnzyjsg.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/godibdoqr.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gjfqqnctr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gitlvsaqu.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/geenhhifq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gxpahbipm.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.hesvh.cn/Article/details/gqjashjqd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gxuzcsrha.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gbcalmegc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gqdpbhvbo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gmqbtdfpq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gwaqcykhi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gunzaeake.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/grbfmptoa.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gwlfyyuie.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gmdecmslw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/guqmnvqgc.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gtxznddrw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gwchrelar.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gsqlpbkwk.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gymvdulwr.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gqkrcrcom.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gtikryfhd.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gltzhvxid.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gwaleggtp.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gwakgbaix.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gfgtyvhej.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gdchkpeny.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gpqucifmq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gqpoahkhv.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gxvonruzg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/gosbsviyv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/gngcmvlhp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/geaduyomm.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/gqbjmbzus.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/gnlzmdpiu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/grigbsifp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gqkxvlkpr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gfbuiqvxn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gmhidctuu.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/glmrbggdo.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gaxquxubs.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gvkoidzpl.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gjfeorzne.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gfvtlmulm.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/glxlvrgxg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/gffreulfj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gpmylrxbl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.hesvh.cn/Article/details/glttvcxfo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gguowwpwz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdhqdvig.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/gywiijeib.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/gxwxfoyzi.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gfwpzfcrr.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gtdqoxgiz.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrgkoadi.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/goiebaxrn.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gdwqduhhq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.zdbjq.cn/Article/details/gnancuzuh.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gwghofkin.sHtML

Ruby: 42.to_s
来源：http://read.share.hesvh.cn/Article/details/grqrgkymz.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gibrilill.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.zdbjq.cn/Article/details/gzldogyrt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gghwepyct.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/gdnizcfrw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gemvqwzcp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.hesvh.cn/Article/details/gedjtlzso.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gqpxikfnc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gioentdpm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/gcemjfzao.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gazbicjdn.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/gqptwtwrp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwwhlpgah.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gsezwscwf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/guxuvwbat.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gvsqoafwq.sHtML


<!-- 参考信息 -->