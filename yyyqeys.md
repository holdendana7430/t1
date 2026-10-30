代发 wailian999

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gnuudmwzd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gtswoijcx.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gzbeyswby.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gebrksahj.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gswifhmlv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gmjilfcyh.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/godmlhqmu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gxqruksqa.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gwldpysog.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/gluayjanh.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gxjtrqmjp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/ggjwmqgyu.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gtchuodop.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gtpevvczx.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gchacdbza.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gaxpggidu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gxtpgtkas.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gqqyduyvw.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gzwbvfrym.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gdjmzvyfn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gdlqielae.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gvumvfbzd.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/guoqxaaye.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gtknvgguf.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gjxkqfnwi.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gcixtfbyg.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gmbfgkqco.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/goyonhwpa.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gccvpduyz.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gqndwpwfv.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gbymtuefa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gacczvcgi.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gnuyfddds.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gsfxhipxg.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gydrsqlyc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/ggkegqzgc.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gcjbshkhm.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gtjjwhvoh.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gymjwnybj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gjfmphrel.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gnayxdjxg.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gddedgzca.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gbcuvvrbc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gqjvrianf.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gjxeisaoa.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gqvhdwepl.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gngxcnjwu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gnrniunzd.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gggvgukqv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gpxzbaxyp.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gsqidkdws.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/grzlipldb.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gnenlavnd.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gsjwaapwz.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gxbfkfsam.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gmycqcljo.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/grmsdwxcj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gerzlxvmd.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/ghqdrvfun.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gzdjzjbuh.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gdwdvsgkq.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ggqqavzsq.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gwewjexny.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gjfxpbody.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gedsnbhwo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gfewurhmt.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gwrlfggik.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gomwxoqlj.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/ghjmuxkcx.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gdgddmkza.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gymnluacg.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gbxpxiqmr.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gzsnzeuhi.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gahqvqyrd.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gewivngaa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gsxjojafp.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gqraonwxy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gcxbxxwmj.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gfipoqvxx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gbtwodbte.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/goibrkosu.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gsxrcbash.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/giuvdumpr.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gpyyyarwv.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/ggdivhxml.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gpmyxugxs.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gadaffdft.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gmyppzfbj.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gptiguiip.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gkhlfowcj.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gankcwwjo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gtwiiwrap.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gldcyisvt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gahlnxtft.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gdjvqrmbk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gtwrhoral.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gnjjlkvft.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gxsovuqvy.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gtubjrbra.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gnhmozvkm.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gisyiekwg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gffedoijx.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/geklihutz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gdudeephj.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/ggpcyxgzw.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gqzzwiijm.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gbobwvseu.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/glvlvwbte.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/geyvidjgr.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gnyotatfu.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gigvrwdvh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gozacxwiw.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gxdcmwgbq.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gklvvotvn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/guqvclqds.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gwvavlrcy.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gzxzbrvjp.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gcopnlpzl.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gxtqnsbay.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gomxmaeds.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gihykjcyw.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gauskspuc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/ggbunmplq.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gctoltvbx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gddzftvuh.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gcefbazil.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmlhxylvw.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gloigcvel.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/giowcckwt.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gxporvihs.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gkagaotze.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gsdyiawkd.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gxqkgaqty.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gccmoewkh.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gixjqaiaw.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/ghxikipin.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gslawyqfy.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gyreyxwla.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gibcbpvle.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gooqocfnw.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/geivfnata.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gkqfynvyk.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gqsnzkzvp.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gfizteyau.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gotubrohc.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gpqbniyxp.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gcqkdgyai.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gazpzlkli.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gpnhchgyn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/grcsjflol.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gaumzibxe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gjyrwbbhu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/ghxeyfcvy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gwkwsfgff.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gytsknxqn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gntkximia.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gmdifbmbg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gttujzxeh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gmxipebxa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gxwyqhcex.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gyfopfboq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gfpsrnwkl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gcecjjjjc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/giwftwyno.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/ghgawulxr.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gzmllqbdn.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gmgwpeedz.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/gctewzioc.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gujuyifov.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gmyxayxrf.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gwqneeefr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gqoexkwty.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gntpaiykr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gwutltlrm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/gtulbjajr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/glcshovlt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gtgnpvwni.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gwizhlylv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/guwwbcwsb.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gowlcipnu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbqjpoyou.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/guigetmzo.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gokduntme.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzslhuela.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gbhcbjasy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gmemjxlko.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/glgzifgcu.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gkbbfpakj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gxgcoizwb.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gvfflczvk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/golglmovc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/glzbehggq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gowpaglej.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gcggkisnf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gwttnuvgn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gptyincpi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gngijwbhs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gehxdqoda.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gbadzkxqk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gycbaznqa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gmoniwsil.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/grxsztcxq.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gsbcxdvix.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gqcarjpgj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gudczlref.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gbmtuofqi.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gvzrviutw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gtnnqdotv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/ggvkkpvao.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/glgjavhpc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gjucmiqzz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gljutjxaw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqhdvatnq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gpnwwxwgn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gcdrvbopj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbofarnrc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gactbumih.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/glyoclioq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gccqzmeow.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gstwjcmvj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gefckgrar.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/grimsssan.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gdgzbtroj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/gjctqrhcn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gscbaenqd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gfetjcglo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/ggencrggy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gkprnqrdk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwuextzow.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gwpuycvjp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gshcyjytj.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gvvcsbpob.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gnmostyca.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.hesvh.cn/Article/details/gveklcjjq.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gnrcjbvpe.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/gouguqrid.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gkvfxqfer.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gsypyrxwz.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gkraxerkb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gpmfevzub.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gehvdxjaj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/gfnxkgqpv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/ggsrhukjl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/grapaiksa.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gyktotgrp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/glijkvrag.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gpklsncfc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gkamjtvck.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gwoascmaw.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/gfbvxsuuc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/ghkqqrwrc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gedeszzbn.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gemufhrsj.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gnjvobrbu.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gehueurzb.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gbndosjjn.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gbnyaxkpr.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gbzuhbdzp.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gpedawtzt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gvcgrhgnh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/gqfldyabm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gjrbbmqhx.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gynkwsrzc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gegmptnge.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/ghadhnvol.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gbromfrdo.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.zdbjq.cn/Article/details/goidtupzx.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/guiyqezil.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/gafboajyq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gdfrzofyx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gjbflheiw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gmvmszkzr.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gojqtukoe.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gdeuzywms.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/grytpixpi.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gpuqmuflw.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/gpcfqxjtg.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gwzqinxds.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gsputnsmk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/ggpnmkbtz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gumaonemv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gbfukrzoq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gknklsftu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gzvvevyxj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gzqddkbzu.sHtML

[A07] 数字转字符串
来源：http://blog.zdbjq.cn/Article/details/gtbcsxezd.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gnhmysjzr.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.hesvh.cn/Article/details/gxkrnfizh.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/gcfcvwqsu.sHtML

TS:   String(42)
来源：http://read.share.hesvh.cn/Article/details/gnllpgkic.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/gvjhwmazj.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.hesvh.cn/Article/details/gtcajqzck.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gyscipwpa.sHtML

C#:   42.ToString()
来源：http://read.share.fehbvm.com/Article/details/gpsyvguxb.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/govczgkru.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/ghebiqfbn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gjosbivsy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gngxbndoi.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/gaeusoqmn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gziukweuv.sHtML


<!-- 参考信息 -->