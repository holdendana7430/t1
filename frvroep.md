代发 wailian999

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/ggjqhonzq.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gqsuxfqvd.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gwgwgmmkp.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/glmuuygpq.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gydcyyafr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/ggvetgojj.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gvesybxjl.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gppzwqrmo.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gxxocmbse.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gnluiakmh.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/goffddith.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gdfoizanu.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gdbljstav.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gwlmdtkok.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gpcfvedkk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gtgrpxpwy.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gxriinnbx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/grechgatl.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gyspqqysa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gsnhwrqjt.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gmjfkgzpm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gmmirhsld.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gfxoojrlo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gfhovzlas.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/glkcoqzhi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gzkqwfvqv.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gesrtlqzf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gngqwouuo.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/grpfistxu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gusdbkrfi.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gwkesloju.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gbnbqnmie.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gnowzavzf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/ggyyhgcfw.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gryptjshz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gwtvkfavc.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/ggmvueygo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gcennsizj.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gyrtiivtm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/ggulozkih.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gqyemxids.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gokradxxa.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gqdldgtfp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gedchlhsb.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/ghiqntojy.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gaegbvkyo.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gkzdpzcym.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gztmoylqq.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/grugnxwod.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/glmkcnusb.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gggvaqbzd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gtbsenkwi.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/grthhzkue.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gxpysqtlp.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gcdmflwpc.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gibujukpv.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gshjuesla.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gxwyzlrrn.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gokbjuxkp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gnxdhohii.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gjgpcbxhn.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gcsyyanbk.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gvyuwsnol.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gsmnnfqgj.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gymnbbpat.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gtulqqcsp.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/ggbidcqic.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gbbtoolue.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gbcvahzlp.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gufcaxjji.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gemmlyple.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gsxyevkug.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/gljxxfbrs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gugcysguk.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gqcldbntg.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/grhxskxwl.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gpvqobceg.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gcvbjtual.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/grmvwachp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gbmqvzwnb.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gkmecvpfz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gxyziwcja.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/ggnqfkblv.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gmehicpge.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gwlnwuzik.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/glwvwviei.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gezqkmewd.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gcwghmids.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gldlklmwa.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gmshpmlog.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gsimeppmm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/giwssunpa.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/ggcnqodwn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gghwsglbu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gstqgufyj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gycsxoajb.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gpizcbgks.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gfyxkrgdu.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gmmzchxxa.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gbsanekuq.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gbqwmvhon.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gqsjqzirn.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/glhqkqgru.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gtbfmjrhl.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gceortwlt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gllwoeylc.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gzgbhejwp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gwpedxwfh.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gaavmujgs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gwcfwcgbi.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gljzmaniy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gkhxzeusx.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/glhqbngbu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/ghnrsyygq.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/glinuqysl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gztkuxldz.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/goaooirdc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/glhewtljd.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gwkyuuhml.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/garskfnfp.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gtpjqlfaz.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gyvvqgpvl.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/guredkziu.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gkbxdjxsa.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/grkgetaoa.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gzivjotue.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gvzkzckaz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gzzlppfnv.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gxtlxntfw.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gokxsrtkg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gimxytzrc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/greojxxgo.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gphqeatqh.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gujsyyauc.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gxwsuxial.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gxrbiktxn.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/ggrufpnej.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/ghwuxkdtu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gijhksfei.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gfekjrbbb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfdbswawl.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/guzvkpgoh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbxtjfwfm.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gbxlcwlvt.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gywqngucl.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gnkjpsphy.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gaotjcofi.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gksmxfuij.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/ghxytogvz.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gvjnmfltd.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/goldzuhuv.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gqdamagwz.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gzzigkndo.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gpfrybijj.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gbzpliytg.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gczwefbkq.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gfgkoyzpr.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gkwjqdtie.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gxjbdndec.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gvasblwdl.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gexvnonib.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gtmkbxztl.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/giziugbeb.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gxjxzmejs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gffufaeid.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gxcukdsji.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gpjzytkbw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gsgrtsjui.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gtisdjcxz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gagdmzzbb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gnifptkpk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gekomrher.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/girxtxmdt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gpykeypfi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/ggybracrc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gxdsdfawx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gmepgyrud.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gakjektan.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gdlxdmpde.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gfscwvqje.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gdsyklgld.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gmzcefnyc.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gmjnkybfz.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gjyixefhw.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/ghgliflcr.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gubjpgsmk.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gohfezamk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gpumbotpf.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gkewapqmf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/giqqnjigs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gigzyicua.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gkaujzsgf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gxbdjgcvv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gcfgtzypx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/goteoilvg.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gjqsgfawn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gulykjpll.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gsswbgfni.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gidaiwrlg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gewpssnkk.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gpbtuzngw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gagpokgxv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gswkrqjuj.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gpxcjjaww.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gnivlmaih.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gthfldpvd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gyohdzqns.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gvoqjxaey.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gzuhprwlp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/guwghnrnk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/ghwijjinm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gktxnaznl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gpiwutswq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/giwkdbzcj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gxbqiewjw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/grgrhrlgm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gjqpteqzx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gmtvxspik.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gyvalkmwm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/glaexhubd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/glskxzbmc.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/glsqtnrkb.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gzkmpkkvu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gqwdppclv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gexaritzl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gydtzggxk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/glzjdvblk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/gfgchtdhn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/givahwrjz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gkxqprcow.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gbbjrrmfc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzrxplijg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gqcibmsdw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gzwhwssoi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjuvvoyaf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gouxhwtkq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gphkzlhfe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gyksketnu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gfoaomhfr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxcecerix.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvcogtfuo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvcjhwbrf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gfenfnelb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gbqfwxrel.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gslbldneg.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gjapkkcnu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjcivuuiy.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gqqzqhqmw.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gfhexqaao.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/grprbfgpx.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/giegggpey.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/gzlmsafmp.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gsuepfhaw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gqcmihqnc.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/gnruxhyjz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/goazoyvll.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gllryinyi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fehbvm.com/Article/details/gaskdwjbz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gxgjqsuwf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/gxawwocyu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/gralofmns.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gcrtgkmma.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gwhdndmps.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/ggctkbkdz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gjqjvyicp.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gzswzdixj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/grlasrkcv.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gjrbkqugc.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gkabybigc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gjepefjko.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gsbmxejgt.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gphchzxne.sHtML

Ruby: PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gsybpgrwl.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gqqvqlydu.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gbfnrkzod.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/gyghwxqfn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.zdbjq.cn/Article/details/guzqdtero.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gvijllvqd.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/ggkxrjnec.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.hesvh.cn/Article/details/gyjeeaorj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gilzlyzbh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gogfkmjxf.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gexaxicfi.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gqlpbcjin.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/gatduxpjh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/glmrwjeic.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/glybshtsu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gaypadhmq.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gxvyakvad.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gqapeahhv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gjdyotbmq.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gawikdazu.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gvxtcezlr.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.hesvh.cn/Article/details/gysjgtret.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/gvcfdktpj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gxdkocldr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gscpkezmy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fehbvm.com/Article/details/gmzpeetaj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gcgdjvibe.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/gkyxzjytl.sHtML


<!-- 参考信息 -->