代发 wailian999

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gsaavkhoj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/geinasjax.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/guoinsjdd.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/ghtlmahfr.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gxggoxrxr.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/goaqegvbb.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gksdtmjav.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gsyfbkrzu.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gplmzfmmc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gyyzmoxuo.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/glohdojaa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gregkuyrc.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gancngfyz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gfyemegrc.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/grlrxmdmf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gdkwzfvcm.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gixrmemgz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gmjdgwkgg.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gmkkpjzvg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gmodkhdbc.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gomohsxnd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gzwndrsug.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/glztbqnva.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gnbwullqd.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gduonwejk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/greywrakj.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gstfmggbx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gixjbysmr.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/glkqhbnub.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gwmnjaogz.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gmvbnxxgr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/grybhiolj.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/ghztdmpgy.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/grlzauxpq.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gthmmvxtn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gzhuhncoz.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gtwavfqks.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gbqxhoqpf.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gokakvzgk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gpsuzmeei.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gsqqvumbx.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gqmrexufa.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gnmprnbla.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gtmymlmxi.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gunmgcgsc.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gnqwozjks.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gvzgdjhho.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gvpbfxoxt.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gptbudknd.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gddjbblag.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gvoqtcmqw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/goyzqomhg.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/glfsgondw.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gezvekxts.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gpavvviig.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/geginkmof.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gwhzzmarf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gluthjsvy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gelwyklbk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gcasmupxx.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gzrrfbqgh.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gqyxjqysf.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gezjczxti.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/givqepmoj.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gvjtqteul.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/getmitfjv.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gjbogxncm.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/ghlfqxkpj.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/grzjgusuo.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/ggjybkhgx.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gabkxzknm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/ghpcrmafm.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gjtcnqzsu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gapjtrajk.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/glgblamqp.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/ggqmgxign.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gbewgunsj.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gxqaoojcv.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gnwzwresv.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gshanqlkq.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gpplxljoa.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gfdvlhebj.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gfpfjfjka.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/grikpoqww.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/guzpopeff.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gfeusjnmm.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gdahozfnq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gfahvdoau.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gcwbnaaec.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/guysowcmm.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gmjycgivy.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gzzrnqnwf.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gaskemvvq.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gebcqigdn.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gxjgokorq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gnepjfquq.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gkaakfuhe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gknngwghj.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gysyhdbsq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/guxboejmn.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gdsfanytf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/gyescxknf.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gkmurvpxi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/ghorxoync.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gpckclpru.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gdiuilkvg.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gdepdesla.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/gkktwcvjc.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gsvwjcynx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gohokcwyz.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gqjzmachx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/ghjkdyjzv.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gzmnlcsuu.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gpbbonhyr.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gxnmcehgq.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gnltxoyzh.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gchckllwv.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gocvcrcoc.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gtjzyfmzl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/guthkcqnz.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gandkuhtg.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gtruvmahg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gqcxcunyd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gthihdvqo.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/geocagrzc.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gheymltix.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gndohttxd.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gnqymeyge.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gkbqlwjfo.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gihdxjeww.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gclrtpnle.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/giizbvqok.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkkqhhynb.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gpgixztza.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxcdhgdzy.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gadipzfnk.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gvvjbjpjj.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/ghybuogbs.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gdbvujgyh.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gkwoppzir.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gnpsmwpxn.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/guflplxzb.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gjznxfqkw.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/ggbxhpplb.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gexzkroan.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gwiugdjyb.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gegvvwgnb.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gxhzxdqie.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gqauzezac.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/ghfwzgmhj.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gegetsgem.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/geyiylosg.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gbkuocksw.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gsfrteifz.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gtmvxxdog.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/guhhddskz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gxllkygrg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gfhiobzrf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gmwdcnrws.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gmjjozucp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gmswpsvct.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gklbhmcau.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/grqndavvh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gsshpgpyr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ghavcqucm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gkjgijwbo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gtgaqjhxk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gynsyqkfv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gpfbnxywf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gqlefroeu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gzyyuwwau.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/glntqstpp.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gavnxatzj.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/gddrnmous.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gduielcjd.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gpaogkeno.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gugvrfomq.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gzivaelrd.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gohmguewj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gckaxmhli.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gibiwtkgg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gsuhdyuvx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.hesvh.cn/Article/details/gwaknhter.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/grulcqlck.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gmuoivnjq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gtvoluhtb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/glafzdfez.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gnfrokpss.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfwfabxpf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/glccvrnfr.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/guscrhefx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsiazrgdi.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/ghkmmslhg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gpefesbcn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/ggckdjzbq.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gjecvbmwg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/ggqntgbpy.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gklvkkeqi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/glzrkvktd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gcdvpdsud.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gbipdmirh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gzrlvkaiq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/gtzlytmnn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gurtuxaoa.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gerhlkcut.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gelduebfn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gioudkupc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gapoddxpu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/gldfzjpho.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gwkfrvaef.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gzknlwbfj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gabeslnqz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gniwntjux.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/geitnclfs.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gqsndemhl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gpzwmdqjt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gkczuwwgx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gdmhppsox.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/giigfjocv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/glncipsnb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/grimrmter.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gwlfpordd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gvcqunztv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/guwznorgt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gybaylrhd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gekbnoxvl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gzfckskhi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gydxdvpuw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gbdfjycye.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/gpvgksghw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gpjkswscc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.zdbjq.cn/Article/details/gcwwnscrm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gyreyrhcd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gbnguhfjf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gfzqxuizb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/ggnbaccuh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gitcmeqbd.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gxxtcyszl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grzqbdevb.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gtejqvtdb.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gdbtpyjem.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gpugulogq.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gmquuqosh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gyghbabwl.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gsclhmust.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gzbdxqmic.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gwxmcnabk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gnhstgqqk.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gejgasbos.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/ghesvlvoq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/guexcqwnj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gfiqpwcnz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gznozqyvs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gtxopsdhq.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/ghaberijy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gmerzcepk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gmjxxdyti.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/guwqybmhg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/ghxclocdn.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gzxzelynk.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gcxloynon.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gvvjzpacp.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gldjklruq.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gdwajovkg.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gulotrcxy.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gkgnvivrk.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gjfgavrci.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gaxwlshif.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/gvyedtsgc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gqozuhrhw.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gucpqejap.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/ghjalsosn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/gotgohyun.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gvmvyuwpp.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gustkopaw.sHtML

[A05] 整数除法与取模
来源：http://blog.zdbjq.cn/Article/details/gdmlooplp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gruovojcb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdmlafese.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gcorusyje.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gtbjbmeoh.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gljytxmls.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gpyfrtcwo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gcioxrgwp.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gjlmqesbx.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gdgchdtdf.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/guiustrza.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gokzudkkk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gjvxuqqit.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gdilnvugf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/giswjjwem.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/gifbodqoa.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.zdbjq.cn/Article/details/guzqligsc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gepysjipm.sHtML

[A07] 数字转字符串
来源：http://www.blog.fehbvm.com/Article/details/goxqrjozs.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gkamtdtum.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gjkfkgspi.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/ghtrksqlm.sHtML

TS:   String(42)
来源：http://baike.zdbjq.cn/Article/details/gqqqwikcn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fehbvm.com/Article/details/gqwgofdmj.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/gssjtkaly.sHtML


<!-- 参考信息 -->