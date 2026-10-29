代发 wailian999

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gukgracwr.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gpmjvytga.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gcevqnucw.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/ghizhseli.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gkhowijyd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gulrnnyim.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/givkphpaw.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gwjvtehhx.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gxoeckcui.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gcdnaalla.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gjxnwvuqe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gwgqtwncv.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/ghaiwfzzm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gvizualtw.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gwptavsii.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gaqacydox.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gmbooflag.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gmemkuigm.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/geshgyuxv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gigtpmrgl.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/grqvkcgvh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gfzbwfnxl.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gdtvzglpa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gvnusepds.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gvbbbrwkv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/guhybcszy.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/ghokgkuzw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/ggkvdxlok.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gqcisznfp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gqdwhzeyg.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gscjzivvw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gcrcptmqv.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/ghqlkudix.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gmbzdyqzc.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gzxctsley.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gxdtzwvkh.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/ghgtvhueq.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gulrpbsab.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/guobqdmhr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gpyhietof.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gkexwlkej.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gziepwkwc.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gmmdaxlfm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gkjxisiww.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/ggxoafibf.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gkruqrvwz.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gepazuvsf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gwxisxlga.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gmyylcvrt.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gswitblfe.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gpejgmfay.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gymmbmolu.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/ghrbguclc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gfpwzzntx.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gvwxydfwf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gyziahjoo.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gkwspofnx.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gakemnrol.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gawlxuune.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/ghmevaqys.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gyyrysawm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gwmzlrstv.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gbywycaaf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gsinkdzim.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gvulczwxi.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gdodypsoc.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/goanvvlsx.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gvigkwqzc.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gsrdbtgdq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gsrnamncb.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gbsmokuwq.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gyuxnjylz.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gdieetjud.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gfvlkcnqh.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gbesslren.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gznrgwwve.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/ghesqdbev.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gulcajirp.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/geczdbpox.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gbfovrovn.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gkeawxxlk.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gsnrtatwu.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gumplfsgx.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/ggnfxhnpf.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gvkfyvuof.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gzpnxrvbb.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/ganipioiz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gzqradspx.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gxdrrbpng.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gvjeoypdw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/germzhxve.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/guktjduhh.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gmxfraktp.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gyyeloxze.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gaxuroqho.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gcoduupxe.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gpytzbodt.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gvjudpbeh.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/ghdnntjmo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gefkaadrh.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gwjqoghhp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gcvgbpvta.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gqwpnobzl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gxgiwoyxg.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gbhifcybn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gghsuyald.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gxlupvzkf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/glttkeosf.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gghdrwszy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gwyxlgyuv.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gukwoiwwq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gcrcpvtjy.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gucwaelex.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gtfldhcqq.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/ghoxwfuou.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/grhbldbac.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/ghuvtquvk.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gftzfakbs.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gugeqlawb.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ggmedpckw.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/giydbwnkl.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gfvjfzdpb.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gpvsvwamw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/ggbxknrqx.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gzomooooq.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gnmxsjdbx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gxfcpdotp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gqkyvhkuc.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gbtzrralh.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/grkyzouua.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gafrgmvoz.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gftbmezrq.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gdmiihntd.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gmdatvloj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gudgwkfaf.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gtphgcuwd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfubeaxun.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gijqndxax.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gedjkuaut.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gvzlotauz.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gmhhrlgcy.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gzyczyobb.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/ggpanspmu.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gyxbzzedd.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gtsnrzwgu.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gcxmwoyid.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gubytmyid.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gefiiozpd.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/giayjwdxh.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gkvbqfwdl.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gqtmemhfi.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gvzquphbk.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gjvveihoa.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gyidmfzvu.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gvfxdtvtf.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gwcntihdf.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gqessemys.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gtuwfwdqt.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gwasqixfl.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gtwqokrko.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gzejpqjiu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/grodqqjey.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/goywyawuo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gixakohrr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gkrirruoo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gkniziqab.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gnaquigiu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gfmpnthao.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gorzcfpdl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gohierliq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gfpchpahr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gxsnsnszk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gispxgrxx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gjgbqqcky.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gdvnyzyla.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gdhxznhod.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gkdwuibzr.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gajoeikpy.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/gxeeikaiw.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gbbgchghg.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gbdgvjjse.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gxsgakmbf.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gckrsbrsp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/guxodfohc.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gbfejdyvr.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gcakclpzg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/grbjpjuvz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/ghoreoxsn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gqmbgxefp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gtzmhcifl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gmueofvap.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gbsymtuxo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqckjflqj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gmhyadhfc.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/grbvqtsso.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gydqhygws.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gmbodrxcg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gokzichno.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gycjtzlyu.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gswiowlsa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gnlmglifh.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gthmnbddo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gwoepaspg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gmjoaaeim.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/glkyqrsvq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/ggyppnpiu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gccpdsavv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fehbvm.com/Article/details/gifbefcjf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gtzxvbaxr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gqanntthq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gcgdmhibk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gvoczvjlk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gorhkixwm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gwveynoci.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gtschytav.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/gfkmjnyfh.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gyrqsotxm.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/gztxrsmmy.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gzsqgonyq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gcvljfngq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gpaplcsus.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/ggszmefnu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gwexgzwic.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gmzjwafzc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gckrbpxbv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gmrjzdjsi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gntbsqaxm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gfantsmld.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqyrubdhz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/ggbvhkzif.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/ggesjnefe.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gyriwaphn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gcorogxuv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gljphdvgv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gvrlitend.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gcftccrcn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/ghpapmqyx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gghwvyqba.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gcaiclfae.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/govdjtmhg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvhbvgutp.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gisxojqig.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gstccctyk.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gfsettybv.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gpiulipmx.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gnldgrzcz.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gvjabbhwo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gzjpelfns.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/ggxmoppvf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gohvnlcdc.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/ghvzgtmse.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gvukdvjny.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/gjahdardb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gkwauhkbi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gmqilcgbk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gtavkbfqy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/galmfnajv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gjltonjfb.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fehbvm.com/Article/details/gdappkadu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gpmhxxrin.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gkoqxnids.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/gygksboaf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gqunrokgj.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ghhhzgvip.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/glfsjqleu.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gpjjwqvkt.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/grfcmenza.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gomiacsgu.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gslwhvxjs.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ggumhgzfl.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/gqugftadw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/ghbahloro.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/gxworkbrj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gllxmkqkh.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gtibciiay.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/gczdkmtpq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gwuqlotjh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.hesvh.cn/Article/details/geftnkllg.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/geizlotiy.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gvprsapoi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gxkkscxvt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gikockmwg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gxxbzoyst.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gujyvwxvq.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gqlgdbire.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/geolekeon.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gyrqeiiec.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/giorncoqi.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/ghfabzmlm.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/grpywvqcz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/ggdbdafry.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fehbvm.com/Article/details/gyhvzydhg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gfsgojnnv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/ggrjngfgg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/gbzvisjtq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.zdbjq.cn/Article/details/gbpeyfufx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gkhxjvqjn.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gkkjumxwp.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/gmoipooqn.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fehbvm.com/Article/details/glwxgemxp.sHtML


<!-- 参考信息 -->