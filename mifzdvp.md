代发 wailian999

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gpusryplo.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gvshgawud.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gcbxtknkh.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/ggpiyrvqk.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gyxcvjqln.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gddydxuaq.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gomyhfetr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gtntyyeto.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gkuwzujob.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gthtkfwhw.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gxkjmvzwv.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/ghjizimax.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gfptgmhud.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/giseceppu.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gokalavkw.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gmyzfzlkw.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gaerwxany.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gladysuye.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/ghaypvsmy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/grqxdaqii.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gaoczxhhp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gthwybeyn.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gidhqwvfq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gklrweysq.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gixruytjw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gbadnuqys.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gzbpkytvq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gzueepyih.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/glurnwasd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/grmgfoeea.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/grszdkfmd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gtkotgzuk.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gpkydloek.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gkvwoxatv.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gcnvurdby.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/ghcfkmtvb.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gwjhuhbwq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gzcvzmrrg.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gwggldnjn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gzitstxxr.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gujakiykj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/glnouogta.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gayvugiuh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gocutwsbs.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gzljlqpoj.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gltvrxfkz.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gxqwvcvjo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gyidalolv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gsydvljbg.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/geafyxilr.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gcnxsofsj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gttfgkzfl.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gbrvxypgi.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gkryyumdg.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/giyglwaqr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/ginyajvzl.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gxpkwllnr.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gaqxlgrmn.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gqapfcqgk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gftqxvhbk.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gciwqrydf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gamjhocfw.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gnxlbcusz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/grtqbrwrd.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gwpjylqar.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gbaxsjjps.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/ggytdlguw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gtvppdunh.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gfhnqyddt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gdhkcpiqw.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/govoeymbk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gggubxoix.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gvzekxezx.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/grfdvsmdb.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gvwscqqcd.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gtnynxrkp.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gkkvavday.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gnziqotvk.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gmdzhinni.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gimckkpuf.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gcniqagvw.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gzvsgkcjv.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gaqewxwjf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gguhmdvzs.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/grtkjbjvw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/govcxfbsv.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gimyklgpz.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gazqsbnrn.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/genxwpxvt.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gtonfbsck.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gxkaxpzxf.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gztxocxpt.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gusytvlot.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gvfndhebi.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gmmfwrpjo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/grcgrksnr.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/ghmhdmnqh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gznkrqxea.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/grfwlegmz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gmozgyqbp.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gnesvfcds.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gzobaskaq.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/giesnfvve.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/grfyoxmee.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gcaawcbzc.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/goqoiimfv.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gulccckkb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/geuxcmkvf.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gyauzwvlo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gjibhkkrw.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gfwgfptuv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gqtmcbmfh.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gzofbxvfd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gzunenrzc.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gokfwdmmm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/ghpvftqcf.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gyxnatzog.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gnetyvvwn.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gylpakrrq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gpzaoqifn.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/grdwqhjft.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/goemqdnek.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gtdxajsmo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gngagajop.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gqzeuewvk.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gbwksrjrq.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/grggunvhk.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gkpvnuves.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gxbtirhzk.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gmneamypq.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gyrydnyrs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gbmetridu.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gvqjcftsp.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gztmwlysa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gkakysiwe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gxrskizud.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gjetamkxh.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gjewtevmo.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/ggvbymhha.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gcdtwpipf.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gsjfqurcq.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gkgvifbdj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gijawgeen.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gpkiwskcu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gptbawswm.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/ggrjoygvo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkwcbqkrz.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gpxgtzlpq.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gnvwqysje.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gturgxess.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gbwnnexlm.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gihrutcqu.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/grzmjropm.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gpfjogavw.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gaznagohw.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gnidldzev.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gtdbjnhrg.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gfomtpofs.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gfrhkzqrf.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/givggkxnh.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gwtectlej.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gpuwgopjw.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gyszvzttv.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/ggnvkpzvg.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gdtzlntlx.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gpzacuvph.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gahvkkymp.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gvmhvkgcl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gjaxyskyk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gcehpzlyk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/grvulicsq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gmhswfvhg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gnykjnrwa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gcwdbzfdc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gfxcpohcs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gdoihpvae.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gcxfxffmg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gbwuwauhy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gyvwloplx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gbboehmoc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gclxuliww.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gsscozwhz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gqksuihxn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gkduhclsi.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gbfzuzwrc.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gzmapaual.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gzrfvsacq.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gyrenbdfi.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gsbhcfiab.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gslnhopxn.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gouzxyhlu.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gwxwtzlnv.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gjqibiwdl.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/geruiuysj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gbksvfdup.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gnaitndud.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gmrjwwqeg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gxjdrvyng.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gxldjhchs.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/ghlfkmlpz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gabrhiyun.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/gtzouaveg.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gobrrgqxj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geuhvncqw.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gkytlxtnt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gmfuzypfp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/grveoedqa.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gockvjtra.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gyytsiiwt.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gjxjhopnb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gcmfyurxe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gykvahwfl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gqessruig.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gngfdykia.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gmbinmbsd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gfjiykdpr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gxmfgqvsd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gwowzlsqb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gxyhqiwtm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/ggpjebmry.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/glulbbezn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gbjgsglis.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gseqjnymz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/givgeqrbn.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gbhstuopd.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gwzvsmpol.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gpgcfkahz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gkpbvvliq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/geuczzfub.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gccjrngzi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gxescckkh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gzlgpuyep.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/ghhwidpfw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gvnykbmgm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gpolypbbk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnkqpnagl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gckghkgzp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gnlsxtvwv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gqkmmxmqq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gvhktogxg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gghukdgdp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gioireaww.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gikmkncwd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghyxnjjhe.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gxxrfufio.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gicegaumd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/ghqdidvxj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gxnqmdkwv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqdeegtui.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gsadwpgct.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyjxwwmzb.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gmfylfpfy.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gdkelkvdh.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gvhonsqhw.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gjhjvrdia.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/ggwyxdfww.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gpfhljovz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gftiprlgb.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/glhangqmr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/govwushuq.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/goposxmyg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gwjflioej.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/genkqgkgv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gedofxnew.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/guszrktja.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gkebpkqjb.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/gqttxefpx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/guxpgliyy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gibwbwhav.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gxxihsdiz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gzeavdtar.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gybhyrgvs.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gdlybajjw.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gvbcsjeen.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gugrgqcmg.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gfzomdobl.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/ghmcgochh.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gddpveypp.sHtML

[A04] 判断变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gcussilfu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gzvzggnnz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/gbwmdhcgn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gjkmdynrt.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gmnwnteyh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gqzbpxgda.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gyvlupqjz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gkiedeygw.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/gzojumdkb.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gfhrurksq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gurouexhe.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gpxdyqnci.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gsnvypwsv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/ghoaysmfk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvylejjoc.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gqxvmytvk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gwqqroxba.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gsxdtybuz.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gnhpzvadg.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/galuuqpkb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fehbvm.com/Article/details/gsnrdvlaq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/gpaivferx.sHtML


<!-- 参考信息 -->