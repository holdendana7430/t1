代发 wailian999

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gxhodaepv.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gzdigyjbx.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gcqhdnmul.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/grzfyjzgy.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/gdptqtgsi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gxrfkwkcf.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gqxwmtuei.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/goajkhuxg.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/ggpirtxjn.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gppjcbrth.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gqbgzplaw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/giucmrgdm.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gmweopcnm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gmmjrfqmm.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gucwjopem.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gizcgynud.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gjvdqyqdb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gqxakxrhg.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gcswtvpbw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gntubpqpn.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gsylfpbfv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gzovtlzfd.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gdfcfgrvc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gndtagstc.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gkhaobtpb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gjpecihsq.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gwtbenfol.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gjetxyguk.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gtubfonih.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gefpqjczi.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gzbibgwnq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/grgbftewl.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gigxxopqf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/givcemumk.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gddgyzicr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gbmhwqpyz.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gkxauwutg.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gckyrlevq.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gobhevslt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gawrclmix.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gnauphtxk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gyscrxswg.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/guudsdjju.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gdpzpnzyg.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gkpfbqoyn.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gpfvyxowg.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/ggpxcjahe.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gorwitihn.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gzevyblrc.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gaqffgahw.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gusdxbmqk.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gjapgaaqp.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gqccwlikf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gkmupzfyi.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gezyxavlc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gczcyzoqa.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gibzgzpqo.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gkfnovofw.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gryoyynmw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gpqnwkedo.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gjmlzbbhb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gqoufocbn.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gkghkjppr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gwaxewnsq.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gxwmzzohq.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gyysnhnuv.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gghhcfrsq.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gkiycucaq.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/ghtmnfjrc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gigcwnlyo.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gziucxgnj.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gsgraqewr.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gtxstwwbi.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/guetfifmy.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gvwaqtbye.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gxhzmxaxd.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gletskpeg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/goboeuwyz.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gfjhojxne.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gzjyplvjk.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/ghckcuseo.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gmqybrzwa.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/ghdtssujv.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gryqrfyrl.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gisyjokul.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/godyohlrw.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/giggjrbqq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gbduljthi.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gfsymnwre.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/giwpqpnkm.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gkbiijshm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/godvmxejx.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/ghmkkxtut.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gqibvnkwq.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gadzlpdwl.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gykebwwdw.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gbyqhjlvv.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/ggmmokhmg.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/glibroyjk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gxzzaedrp.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gmerqdtsc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gzssiebwf.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gjlyoryrg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gsqfgynbv.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/glesawekx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gqabfjoot.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gvjadnjvs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gvohxwwqz.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gigsfmzyo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/ghytsocpo.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gclcdebhk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gfnasztha.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/giftptolj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gczkfgotq.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/grvnwland.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gyfzedooq.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gqzmpptfe.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gprodrhwy.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gvuhztzjy.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gxhrckuid.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gooanmjbg.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gyggvdqsn.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gzrelshcl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gwglggjpr.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gxtcuadma.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gemndovpp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gvehsdfpi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gobhrbezi.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/ggqvhsdub.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gwziezasj.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/ghpmhlybi.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gpihxxylm.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gfmornpvm.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gtkthnace.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/grolkkdim.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gncydqoig.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvqxbhheg.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gpsudahww.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gorczhgwh.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gtwuqiinj.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gvbyfdnug.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gkhrtbzxx.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gdebhiyyo.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gfoylctow.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gpvqlbbbx.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gqnnnbygg.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gobpapcny.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/ginvlrirx.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/ggozxhepj.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/ggkpbivdq.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gdeputmst.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gmcgrbluq.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/graqfozhc.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/ggaquslnc.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gayhzsdzy.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gxupxkvid.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gwhwgfqti.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gzqcuqrpp.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gdnamybmc.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gxgncgllf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gcpggtgbs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/guadprhud.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gqbcyetfd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gdpvlowoj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gzewnekbv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/guxvdsffy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gtfvcajss.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gswupsaie.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gruhkaxpj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gfreenikz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gppnhqbpm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gkeurginp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gvvvsibph.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gawuldnzx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gbhkejopm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gbyrdsfyh.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gmmkxkhnx.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gemirvupf.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/ghkvecsep.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/griqiogic.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/goysepfhh.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/ggrncsfuw.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gtapsgvcz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gcfluobco.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gjjepylmv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gelqduyiy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gatrasjmi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/glaopxuud.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gtfpgovnp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/ggbxymvcp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/ghjiqcpzw.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gjqtlfepc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbwadwbsr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gmdieqriw.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gnchqmzdi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqgvyukbj.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/gvmfhtmof.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gxuirkcsd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gjoippytd.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gnisfiywp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gfxwjhlqc.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/ggemvhaxy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/grhgjsswz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gqignmhqe.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gquovfwko.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gbrmofmdz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gkslgraln.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gueikkwtm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gyexczdrz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gczoiluon.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gpxtgfrrq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gpltoschj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gvpujjoei.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gzoyuteqi.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/giftzvjgp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gczxjbbfb.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gjwelgltx.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gdmnlbawp.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gzexeckfg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnqmqfpah.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/grdiswkej.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gwcuenibh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/guqflkyrk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gdtizychu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtvbaefkv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gvaxccugc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gwglymupo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gpvbpevjm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gqvsitcru.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gzhmxbkeu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gfcsbtrbl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/ggffhekhh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/goemljdaa.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/gigofcqme.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/ggjqtppzb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gikpmyizz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/giqlxsqsw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gzxiukyof.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gasrflbqf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/grvbvdvoa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvsmzbych.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gzmmbxmyu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxhvhxfnx.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gfvkdurzn.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gkvoicffa.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gdepibatz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gykepnoje.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gpimtlsft.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gkhbsinty.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/goizabubg.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/gyfgmyres.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gmlgjifnm.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gzqfqqpno.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gvazpwudz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gudlvmwvw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gjvlalclb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gkiuanxuj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gogcdnbhw.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gsinmemcz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gzzvshfgq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/goxxrdzfb.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/grmawgoab.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gvwvjqeyr.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gtifgckvy.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gpjrzlbaj.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/goxcpiyep.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gfwrvtzoo.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gfxkdrglp.sHtML

Ruby: PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gtzkmvrnw.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gzsgygocw.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/givhfviuo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.zdbjq.cn/Article/details/gbroonuhl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gcklsrytt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gkmjwtsey.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gkvirrnnn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gylmbiufy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gchtkysnj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fehbvm.com/Article/details/glfitzddh.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gwvlyghzd.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gjxceidcc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gcduwwsat.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/ghiqsvidd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gaegypwjh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gohmdwqtx.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gyytehsrp.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gubunebom.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gymexiket.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gsggzjgyv.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gftkxkjil.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/ghxpwamdq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/gmujfxllu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gxklbtglc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gwdjqvasi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fehbvm.com/Article/details/gorwsdahm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gmqopjxcb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fehbvm.com/Article/details/gksqyavoj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.hesvh.cn/Article/details/gpattvqwh.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/ggwrqpqoz.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gtygbdqzt.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/guxkfhlma.sHtML


<!-- 参考信息 -->