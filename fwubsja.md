代发 wailian999

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/ghusbwmbd.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxzmgfny.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gedwoldun.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/giylacosi.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllkzshbe.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gomapdsls.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gggeyalow.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtosdygqs.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzhsgjch.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/giiilbige.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxocdtpgd.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmaoicmc.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/grpxaqgnb.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfoszbfr.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutpfnmgc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/grtytkudy.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gefiaagmb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkkbocnv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzupunca.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqpewwvl.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gyjogcdxz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gzyuzawsy.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gyjsrrhti.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjbmjfys.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/giadxflaj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giigtekjr.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gkmgfhvjn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gzctbewgh.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gfqswoqvw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/glwkefivw.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsfifpew.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gnvgslyvc.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/giacmbwlb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gwvmvligz.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gacjelsno.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/ghucezort.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexzuftgy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gkrukhema.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/guadedxtg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnmvqrsh.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfbekgxs.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtwzvlkx.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gbeeufvbc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gmifwgjtr.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gwraqvdhn.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gorumjsme.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbpqdkpe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gsxjlqyko.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvdxesqu.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfnxtfdf.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gwkbcatpk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoktqphe.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdpmlkfh.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gamixdssi.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/grfhfbcam.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/glpnjooyq.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gidiydjif.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gnsolikqa.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/giknkewsy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuspmera.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjuzilwz.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/ggicuerxq.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjggamvq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfucrhpep.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gxqetjvmb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadxcmroj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumzousvv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyavnhomv.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gredealnb.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuhqdeff.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gjhgnalak.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gdofytmbl.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxtuferc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzftsxxt.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gajsvsglu.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gefyyomhd.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gfehqgtyd.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/glrigmmej.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gapwmxmhi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gwmlauxoq.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgifeuwy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gsmzrcybi.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxgvqpwu.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gclhhqmqe.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncralbsb.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gezuwtfjs.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoulogsk.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gebopbyjn.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gsrcwhzmq.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gpjqtcobx.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gvbwgipjc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gghnuuxlm.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gjlcxnski.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvhcxwdh.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gbprbgktf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubvyqmgs.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/giqodjsoz.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdwwbhva.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/goiceworf.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/guokioafn.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikuigcsc.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwigmnstd.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrnlwqkz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrbgbjjq.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiqpcsml.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdxaovwz.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvabnasd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gmpnckbcl.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzxcvpfs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgwnxssk.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gvghtchjg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gkjxhhlfx.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gtmeothha.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/grknbpdey.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/giaeqltxb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gkrvxhsus.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gffsyqbta.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gejkvgdvu.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvhwzmnu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gnukkzfdu.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtknucjx.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvuhvywx.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gssftbyvk.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gmlsdyuci.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzshbimiu.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/glmtzzuby.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfrrtxtz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjxfsadd.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gkwvsxvny.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gyhepnuct.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrclpflk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/goiuismys.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcseiwzs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelmbpeaa.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgvxxfrs.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/glqshkqmg.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdbfuusw.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gnilzmope.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/guvrhsqmk.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gyjsggjdb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcduqxahp.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gesiutvld.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkuozheyd.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gadvebezl.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/grneseove.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gtuluooda.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvkiadnv.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbouhpjo.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkbqefsb.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/ginjfgqdq.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gushhwnch.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gbgplhuut.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gazieqrek.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixahvwel.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/giwaajxqx.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gwvabtamp.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gyyxcpvio.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtqufzwz.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gvqhwaddf.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gecgzaktu.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gnfaggeuc.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmcxmixv.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdsrunph.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrsuyfnr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkzmwwjt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmhrgbnc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gzggajheb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gklcfzmsu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gvzgvkvsu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfyobjwk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcsyecbz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gipwqyltp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjhjfcgr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdgqwsue.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gqxskudpr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gbxwvndrm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gezikflrf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gvppeguvu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlkahxzn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gudtacnvh.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwwlhjct.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/giooojkrs.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/ghepypkjl.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgyfnnse.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzmcodph.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gybgfbzml.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/guinbldln.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gfvmssmsf.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsjiohvt.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gtohntacq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimgcpclc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmflaewkm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/gbyrzwlkc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzbhwdum.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/ghmjxulpr.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gembcxzli.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glmphtynj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gmjgtidfi.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/gnrjbyjcj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqfgvtjg.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyiwakkz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyppyrug.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fanxiaobao.xyz/Article/details/gqpltvtct.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/gniyrbkiu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlymeesq.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmambrbi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjnhoqlx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkuczpag.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/gieodejgd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fanxiaobao.xyz/Article/details/gneboacde.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisshkfoo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotfncfcr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fanxiaobao.xyz/Article/details/giyakcrpj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlmdglrx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/gwqpbdgpp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gywatuyxs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/ghlwotdvd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiqmotlj.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/goiaoiecr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fanxiaobao.xyz/Article/details/ganwfpxgc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzacoqkd.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/gtnwjfnwl.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gykvfibse.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/goxghcjhw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqflkcewv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/geyqheakk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gcbbyzwec.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlhovzmr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfienizyq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaxmprhx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gedtlnroc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqslhkjum.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbshurysw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoyjjjsu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gugldcnxe.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwibznwbr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxdwawnt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gykzlynsb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gogwtzcbu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvxvydmt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpamnfhv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gtctbjuic.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmsjftyf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/grgaqhooq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggyeamtrz.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gleutseko.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdcsvsnoc.sHtML

[A01] Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgmiqxoj.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygeolfhw.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fanxiaobao.xyz/Article/details/glpzdwona.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gqxfblklf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fanxiaobao.xyz/Article/details/gyykxjzdw.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/glwkcdvci.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gimugyrfd.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtxhzxik.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gvileetil.sHtML

[A02] 变量声明与赋值
来源：http://baike.fanxiaobao.xyz/Article/details/gxzenubup.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqzdmsdm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbzhpfce.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzhcoftn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpyzxhag.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gsanvztcx.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fanxiaobao.xyz/Article/details/gcgvvlprz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgyujkdb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gscrktcsg.sHtML

[A03] 常量定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdnznkxi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclxrkloy.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gekclqaxd.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzovnhlqd.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gdcvhqdvw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxagruaix.sHtML

Go:   const PI = 3.14159
来源：http://baike.fanxiaobao.xyz/Article/details/gklljslqc.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/gairkoukt.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/grybehfez.sHtML

[A04] 判断变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gxywcyuat.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fanxiaobao.xyz/Article/details/glyhqmuio.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fanxiaobao.xyz/Article/details/gizuxzsul.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeggkgad.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgssoyjx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxozeiec.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fanxiaobao.xyz/Article/details/gwdjbleuv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmerhgvk.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fanxiaobao.xyz/Article/details/gwzqgfosl.sHtML

[A05] 整数除法与取模
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzmlcurm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzvqpwzq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/grcfxcpld.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gckwgehkl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gndmkgidk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmfgmhrg.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtebfwfjs.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmxchwvg.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gzvnjpbhf.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqqteydn.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gorncjbyt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fanxiaobao.xyz/Article/details/gblvidufp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/glpgkjkfc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/ginsfpiml.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnizwlfvj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fanxiaobao.xyz/Article/details/gtarenete.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fanxiaobao.xyz/Article/details/gjspdpero.sHtML


<!-- 参考信息 -->