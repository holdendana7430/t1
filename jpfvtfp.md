代发 wailian999

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gaqmfnotx.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gkzzwsgjb.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gpxskzelt.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/grbohbakj.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gkbtnzius.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gcmwwpbnu.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gectjpjxm.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjfjaarxt.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gvsvdovnb.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gyfbubbcw.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/grcvpufpd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gznewxqgp.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gphduhzgq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gqjtebhog.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gjvoxyxmr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/grlzafoyc.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gcovhjkum.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gtbfoxyqr.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gmkdgszyh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gmnmnsrvg.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/ghbzzjsso.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/geobknfhm.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gfptkssmx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gebbjmndc.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gmffmjddw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gpyvzpwjy.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/ggupgpmmt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gorxurswo.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gtddpodcd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gdtbhpmaf.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gkxgsqafa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gjnspgszz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/grkiwjqvx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/ggfxchhmj.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/ggkahefeo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/ghwfmkdgx.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gxjmwvozw.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gxpwamdba.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gmqxonpne.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gwanqlwhe.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/glzbxquit.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/guoedbqzo.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/geahgferx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gsvbrpsil.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gozfrszlf.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gqapflxtq.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gttivgzss.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gggooosfu.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gnjdwjxdk.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gwdrsoxqf.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gyjhbwqes.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gunzzqdba.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/garqdimbe.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gvnhtjgbl.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gkkoowyww.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/glxzazoli.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gnmloqfzs.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gzlphrarb.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gthtsstrz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gdblrrxwi.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gvyoneyni.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gwgvdufon.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gsawqivad.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gjytfdedt.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/glebjkwom.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/glsmwnnyk.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gboygegrp.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gtqsbfyys.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/ggsaaqczq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gnnjqulus.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gidbomkdz.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gbyvmtlxb.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/glaaukvbh.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gktkantvr.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gxwbrzxqq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/grgmwbpcd.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gvczupvyd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/ggawlqixn.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gatbrzvfc.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvcvefajc.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gkmbxyife.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/grnkfwanp.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gpzwexdbs.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gcicfaxtu.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gscctnzlm.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gzxnamjei.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gkdtghgev.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gktnxxujx.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gwvnqazva.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gfozcuevc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gfknqbuzl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gbggtzhor.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gspquwqld.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gpxjrjsbe.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gbelwxkgw.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gciuvjggz.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/glnyqaoyh.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gcmvskyfj.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gwkqphbdm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gswlozuqd.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gvcvpsufr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gwhdefmls.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/grqowgmmr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gtdivgwpf.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gkjethwgr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/geyhzmgfc.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gzxnqrgqt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/garfwcfwm.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gahviowqw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/godyfovws.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gvqjyczvs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gzqzoupcm.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gryyubejj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gkvgeftkl.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gfzalmnfy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gydupdedc.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/ghgvhusyg.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gplofjxis.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/glfpbpfqy.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gdjhphyya.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gfsgklkja.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gymmvnprt.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gstysxngw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gghcferhb.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gxxurtpqe.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gifjppixn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gatqsiygv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gxxutzgbd.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gldicvcrf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gspbjnxzv.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gpvnctjoq.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gspwycdim.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gnhpscxto.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/ghmdczszm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gpbxpfvvq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gzyjdoopw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxzvuiezc.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gczaqhoya.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxzdpjjej.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gowuqjoik.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gmsbywbbz.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/ghsqbnlmq.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gdmmhmxjk.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gxugvzvuw.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gjgbmzqzo.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gmfstbcys.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gqnjvjyez.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/ghlbjzeko.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/ggevxaqfi.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gbucbcnlt.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/ghednwdtu.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gtdzsqify.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gbijvsedi.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gohyjdbfy.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/ghedqhlvz.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gohxeegbm.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gakziemyu.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gxwddexsf.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gefwmxewp.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gvowbiwkt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gtnzzxqjh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gdoybeebu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gwcvtrncm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/ggmqjgaur.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gusgidpqs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gcytbhitu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/guhmgubdq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/geojkxctu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gidktdhfz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/glgbsofrd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gzxotjyop.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/ghmnzipbl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/geuiltavs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gpxkecqne.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gaschsmmg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gylmudtse.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gzjljublv.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gvbcfsoit.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gewockfmg.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/gyidpoybd.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gkcjfutqf.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gpghwnzgx.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gyettyqcs.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/ghdeqrofj.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gauapvocb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gzwgfuesk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gxvioxpxa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gmlxqohas.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gzyecnttt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gyubudqcx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gjvatkbya.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gnhinxkra.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gljvkfggj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/gbojmqibq.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gwpkuzavz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaocjvuuy.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/grhvyogtl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gfloucldl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gedhsxynw.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gbllxyalf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/gkdnfpflq.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gnmjokmpb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gfpasyhse.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gajdvamgz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gvrohckwa.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gkemypcpo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gvnllufrr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gmaauiqxz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gbxqtzprv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gizpbqcls.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gjyopggwa.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gskwpwrfm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gpkhzqoix.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/guinirlcp.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/giuhfeqgg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gnydnhgev.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gepvompei.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gzrkhncal.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gqzqaztyc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghoyhnefy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gtlnyacvp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gupeyrbuj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gyzjvefpg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gpipictxp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gvhggpkop.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gcvyymmfq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqqewyjoj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gtkzdgazd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/ghygrdzae.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gsennkvpt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gdwhmuqkf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gonhrerfs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gqjcqispu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gojwgfisp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gsdbzstla.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gfyedcamg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gfxzmdqrk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gygmxwwiu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gczczazqh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gzgyhtxfr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvbbqzgnp.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gisbuxsfl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxnfvfoaa.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gdzaumlrf.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/ggwonixok.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gaflkhqdc.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gzyfewfyt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gxybeqhng.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/grbtjprlr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gqdmbxfiu.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gokbsfhub.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gelyeugwo.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gbcpyiqzv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gdgrgiugs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gdfxlykqp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gqudlcplq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/ggiqbhsio.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gtfewwvci.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gaizxlqza.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/gcdikvtdw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gvhodefog.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/ghllfteej.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/glrldyqph.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/guqeqkkfs.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gbcytwwug.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gdxntrsik.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gywomqaob.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/ghruckqvy.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/glnbnekrs.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/ginsjyafh.sHtML

[A04] 判断变量类型
来源：http://blog.hesvh.cn/Article/details/gwrqzyxpx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gigxpwvma.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/gvdafeenm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gnhiojzuw.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gopcjchbr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/glzgcxeuu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gemqbkefb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/grcucywom.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/ggojvivdi.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/goxiqilbd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gxjdqrglm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gcpgwrzqe.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gpllbgntp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gxzqwcltk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gjxwuoedx.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/grhrimkpp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gmwkkqbub.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/giecakstq.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gshpnnacs.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gkecshrqi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/gujpbxbiu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/guzomztnq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/gmarydmup.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/gwyoybdfd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gdizudpkc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gmwtigjeq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gmcfagysx.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/ggzvqqybd.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/guihbljfm.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.hesvh.cn/Article/details/glcfahgba.sHtML


<!-- 参考信息 -->