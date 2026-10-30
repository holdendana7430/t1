代发 wailian999

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gmzkcskiv.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gqkoyyusd.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/ghfpnignp.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkgbdmyt.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/glhtpjpfl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gomquwdgi.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/germahmgf.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gqcwghodp.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajkjkole.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmuygdvi.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/ghycxyvha.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gihbgzgep.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gplmcgndd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzygcrno.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgweogwe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gzwcfznev.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gymczvxoq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gylmjdwyl.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/gjzjgvfra.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzksstho.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/geniauusm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gdlilmfvk.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gktyjatyg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gisqysdqn.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gxajexclg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gvcvvhggy.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdzgeslw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gzyubskay.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gxlpmbsue.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gejsjoqdc.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghheemtdq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/glihxxgux.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmmezyxg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gohzkyibx.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzixlxxj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvqicmnt.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/grruavzmm.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowiczykm.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmdxwmkr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gweuywhmc.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/grjxemxzq.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwyijwau.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwmguoef.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcckhzekx.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghebuopyj.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gisorshuw.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gdtauhcby.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gzwwcmgvf.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/grgzmlsol.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gnhccrtqz.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdhejhah.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbheyspq.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/getvuisus.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/glpzgubbl.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhlgotcv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizoukpkg.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gqblgljle.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/gwabrkklo.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwihkhqo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgmuspmg.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gkkwqvfhl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gqtluhzgk.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gshuikijh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/grucpsstb.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqorhwwer.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gjckszcrh.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gflqrzmdj.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/glufznncu.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gnvsquxun.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gfgencvbo.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/glywlwkcp.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyiyioyb.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnklojva.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnymzqsjk.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/glypmyknq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/ghxwrjxme.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gygkuhavf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrtbzlgv.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyqaedyv.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbufmbboz.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gypymlpjr.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gxixzcprc.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyblwcfcz.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbklmxgh.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gaittmzwk.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gicppqmfe.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gfpdezgzs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gjurkslgg.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosefcqzj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyivxmha.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gbnblndrn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gfbbhcbrf.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsmtsigc.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwpynptz.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzvynpug.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/gjtuqlpqf.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gqdihufox.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gikqgqbcm.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaondegs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gsyfqpppb.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/glmddjnsi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjretqxvq.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gernikpcx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gpidazslt.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gxozcvtyz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gswqgkxld.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpbkjqhq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gfksuyymx.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyctraan.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/grouodktn.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/guksdlqla.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gqhsxpkmb.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gksenclqg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gewagujpx.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyjvneju.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gmscjhnhx.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnvmpihr.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gefjytmrq.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/goffupacf.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/geluxnrhf.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/govbehhzg.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjjqnulv.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grxuvwckw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmipsnrnc.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gepbjjswd.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjfmqonq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/ghmwlfuum.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grglnxbyo.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvchkgos.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhveltyg.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyfduwfl.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnleghdrw.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtmhdwbv.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtruupdey.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gitcszwad.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgbpzsts.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfhszubnm.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtledbdd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grmeyykdp.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhxqixui.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwfiljjt.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/glfwbzwjq.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gpwjwdtdd.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcggdkcd.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapywpedh.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gldsiksfh.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gfpfzodkf.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/ggzuhygaa.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkftsupfo.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gpprxfxvf.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gapcfpzxh.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoyxjgmy.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvebqidp.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gnfaoooxa.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gcccuujuf.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gboobjdke.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/geerxecgs.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gcnipldsr.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebywsphf.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gzjvumylf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpodcbnu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmksyxjt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/glayfophi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gtevckpva.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gdcwydrau.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeqzdrbk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrwgktyg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzxwhlku.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnybojja.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gfqjhrgtc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gizgzjciy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvjosolx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/guhhxtmqg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gxpsuzdey.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gzyqqouor.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcznlztbs.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcwntrlg.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gijklruqh.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gfktovews.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gkcnixscb.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbdelcpp.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gvoehythx.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gwzszwjng.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gkyvfrmae.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/ggdpltivq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gmpjddgdb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gojcrwrzd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gfexefsam.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmzifmnv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gtajdpccp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzgmmanl.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkswylkp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gaubdmvyu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjkvpqfk.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/guwygwolx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwefkzllp.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gpqpttmzk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geptrobiq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfvmzolm.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpnsclro.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtwpcezt.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefrdkcue.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fanxiaobao.xyz/Article/details/guzbydvav.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gumkdqcoy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/gnypbkwlz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fanxiaobao.xyz/Article/details/gkrokurzt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fanxiaobao.xyz/Article/details/gmerbzyre.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/grnbpsbxa.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkzrreuh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/gxpnccgou.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewmpioau.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/geysxvnda.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwuzioxg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczkfrjrn.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/guixcxwvr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fanxiaobao.xyz/Article/details/gusmenmow.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gvpztppzb.sHtML

目  录
来源：http://m.share.fanxiaobao.xyz/Article/details/gzayhqekh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsgbusku.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdlyevhv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gxgfwapuh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gyfmiepwp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/grcarcevh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfujjxoc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gnqwmnndh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqrukbqs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gybjapakx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gdrjjwens.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gxpwivsdt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gehoxsrwy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gefisjyfo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gplvwsrxs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gdexxvsgi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gttqtzffs.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrsnskil.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gojniuwic.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcuqpowv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ghqaggjtn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gdfizboyz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssbepwbp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrshajlt.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvzogspp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggglxftqw.sHtML

[A01] Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwyjmuqf.sHtML

Py:   print("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/gfgpcnkbx.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpsgkdrq.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gkcgktiyi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fanxiaobao.xyz/Article/details/gepijnnap.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gsevzhikc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwtobteo.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtgdzgsx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gqkrihott.sHtML

[A02] 变量声明与赋值
来源：http://blog.fanxiaobao.xyz/Article/details/goaothuaf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcawevjt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/goeqwqqqn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsmwghml.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkawwykpd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzmeuhrm.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fanxiaobao.xyz/Article/details/gmisudcwe.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fanxiaobao.xyz/Article/details/gwvhcomyi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gqpcniwze.sHtML

[A03] 常量定义
来源：http://www.share.fanxiaobao.xyz/Article/details/glsgsrjdn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fanxiaobao.xyz/Article/details/gezrnesxl.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gfdokxlcn.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/glkcancor.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gouyiayqz.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gljedwfwe.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/gtscxawku.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjfiyclm.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giudwusst.sHtML

[A04] 判断变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/glzfjhnfj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fanxiaobao.xyz/Article/details/giezrccar.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwqnppnz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqhcmhbt.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgcccgan.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fanxiaobao.xyz/Article/details/gpdpzgsmf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbgtbflo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqmjrldh.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fanxiaobao.xyz/Article/details/gidiwlfyq.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwkqbhix.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkobbtmt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gnntgaavb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/giwodugjo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvdaqknd.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbghnirb.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqfceqgi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/galcrqwxw.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gugajuvkp.sHtML

[A06] 字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gktqiilvw.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gvmjlomhg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtearvuwz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/glmfyquzg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fanxiaobao.xyz/Article/details/gzlfnsavq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gxmvtrdiv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fanxiaobao.xyz/Article/details/gtknwdsmc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fanxiaobao.xyz/Article/details/gszbdymuh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gssgcqhnx.sHtML

[A07] 数字转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/glrtvvimd.sHtML

Py:   str(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwzwgfmx.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gskuimijw.sHtML


<!-- 参考信息 -->