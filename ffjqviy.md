代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrywwatm.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/gvyqumhbc.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeliwahl.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gzxjjewej.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxfmwfpk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/ghznjwyhs.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gmwvbwsjb.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/getsojdqr.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gldzgswgd.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcymjhhtw.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzwjsyrv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/govauzxmn.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gimwbwfbn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gkfvoptpy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjutvccde.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/girlobfkm.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gifakipzl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwilrczlm.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/giakxtcju.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gshtyfrcj.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbsrigsg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gedmvtzvg.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/glotiihhi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/glhmsirkh.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/godgtzuqo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuqrjjkg.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/goyoqzosb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gqbpadath.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gccgnnuub.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbgceyyy.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxlffdgf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gnfgovzdk.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gtjduftvj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gdxqrznmt.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/ggmwanymj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gnoqayrtb.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gltwoeppc.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gstwniiww.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgefzhyw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/goynpwmyr.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/glpvalgfb.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gieqibqyu.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkztcoezb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpyiwvoh.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gynnrkfgg.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykkrzokb.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gybvvaxqa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbodxtxew.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/grhjjphym.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gnrbaqdtr.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnesxdca.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gywezwyyb.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gotbnnsdm.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gcenhpynm.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzjhdfwc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gyhfqevey.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdhgctyp.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpzvsovh.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscuyyhpd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgnwjarv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoevzjeq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gshrlbpar.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvxhytmm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwjxqnfd.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkfetuui.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/guqsqiivl.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuxrusag.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfhgvigw.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gvaynrtlh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvawwslbj.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gswwtqina.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsmpirvb.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gurnhehfz.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/guyvkefzc.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwcyjvjyp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gbatppscc.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gmdokdizj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gufgcmvyc.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynlxhbli.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/glosubmtf.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/goiqgcztp.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/goykudvkl.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhzcxitm.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gayrolptt.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gmfxyvvzw.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpeyijdh.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqfikrtp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gcbwrygur.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/grukbzxad.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhepvznx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoqbtbvq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/gncwynswa.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gcipffcfk.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyffpzny.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gneskcbxd.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/ginfhiujz.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gkakvibid.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbhtafta.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gprgawbdu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/groinveby.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgneekfb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/gxahettcx.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/gjsrkawdk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gdkofdged.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gbkmgzgma.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkdpcpuz.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gahwfqwyk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/guhvudcli.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gnecffxuv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyybanho.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gqoxsiqvv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giscxqjms.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gqoqcbnuh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gyoapirxw.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/glknoqzde.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujkmrnci.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gbdgtdljk.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/glvznhbms.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqpdotan.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyquqkuh.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/guzbstjlv.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gpntxsoue.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gcmmxoxbd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gajgmnbqt.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/glwixmvck.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxthjciw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/guvditcwv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/glxpmsfmc.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gxidstbwn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkilsqzoo.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gsgmizgnu.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkrvxfgu.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhdvbynp.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/ggpbflgqc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gjocqrhug.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwyozmgl.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkmcoucak.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhipkpgh.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkvejohr.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmrxyclk.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gifvkfery.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gymkuofke.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gnyvaenrg.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyafncvce.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyzdvgau.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnaetzpa.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfziugwg.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgrccevp.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhsttoka.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdnhypkj.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjykezoo.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnylhitg.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gdhdgqnzg.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgsoslcu.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyzejxin.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/geaclbqhd.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcviptmz.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/godpffakr.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gdztesiat.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/glwpwrrtk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuvksvwf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/giqyukvol.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmptzftq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnvvzuec.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gkemupems.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclkkbbhv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/ggdbmlowk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoqtqtzm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/geysyebfe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvgxecls.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golaaquxz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxvuszmk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gdrxioamq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/grcsqpupd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvamesvbi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gnprpsker.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/grlipbzbc.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/gwivgsjtm.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbojnyvq.sHtML

T 其他语言补充                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gybejdvtl.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkfmlwaf.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gcgggridl.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gzfhexvfw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfrivizt.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gardonwgm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbgyletf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynthxwpm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gltuqevwt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/giesmfrtc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/geyowisxe.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gmieplcvx.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gpfvzwyiq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghrmdqmwg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzmokgjs.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/gaknuulvl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqaumqhd.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gqhyrjfxh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/goqpieouq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcqrdoyc.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcbewavd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwvoskpr.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvbxgudu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphnjmoeg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/gnpwuxetc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqcjrrfo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fanxiaobao.xyz/Article/details/glsvvbixj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgrzyplk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/gthxxpuww.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzupkmlx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/gkhdonrpz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fanxiaobao.xyz/Article/details/gzrbzoiql.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fanxiaobao.xyz/Article/details/gwipzgegt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghldqkfnt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkkqtxul.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gqbplkuvq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcdbcyzr.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqgsuykn.sHtML

目  录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmugczqu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gilppcput.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkasopzd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gkcddulnc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gomfvwjfp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkeqadoz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gbvxuzjsx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchzbihuj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggawotwzc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gdrndwklj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupykpocq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gbijuaooo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gddbbtpbs.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gawlyrytc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwshzdcg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmswdduq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkznzwdb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkzndjch.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ghlolyonh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/glvztkogz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gwsmnitlw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gnyljsltg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfhwulbzi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggdqjnlfk.sHtML

A. 基础语法与类型
来源：http://3g.fanxiaobao.xyz/Article/details/gdjzbwovl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gztqwiojr.sHtML

[A01] Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gxrdnpots.sHtML

Py:   print("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/gughlhadi.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtocyrwml.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gzzefnswd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fanxiaobao.xyz/Article/details/gefytyzql.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/ghnjhdyur.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fanxiaobao.xyz/Article/details/gqinbqzxk.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gomyvpdtp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/glnwuyrks.sHtML

[A02] 变量声明与赋值
来源：http://baike.fanxiaobao.xyz/Article/details/gnrnezfoe.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fanxiaobao.xyz/Article/details/gbwdyqxqq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjmunuaf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gimwspfce.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgbowjtj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gemvsxkvi.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaiitmcu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fanxiaobao.xyz/Article/details/ggyjyijbx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnqqvewp.sHtML

[A03] 常量定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrhkyfpv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fanxiaobao.xyz/Article/details/grfsthvda.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gutigyyag.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gggynplbc.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwsxpvhd.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gguilmrlu.sHtML

Go:   const PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/ghhpmylwj.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/garyujjqo.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpsrzdwf.sHtML

[A04] 判断变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gebpzvfmt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhkivaqk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gnkhbsgxk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fanxiaobao.xyz/Article/details/grhavgigc.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/grljuczsj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrseulab.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fanxiaobao.xyz/Article/details/gwnyjofkm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfedufqnn.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fanxiaobao.xyz/Article/details/gmaacjooa.sHtML

[A05] 整数除法与取模
来源：http://3g.fanxiaobao.xyz/Article/details/gddahdtjl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiluobhf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/grxqlmnoi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxxxdmalk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gholfpews.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gutymkvxj.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhfmzxbl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gerfugotz.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzbiufqw.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxrgoiyq.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqchoomvz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/guczygdlo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gafyisyzg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkdctnft.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohszythg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/guzyqvlut.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmahhembg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gowyjikli.sHtML

[A07] 数字转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxnhjtvv.sHtML

Py:   str(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyajahspw.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gytuzqcta.sHtML


<!-- 参考信息 -->