代发 wailian999

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gwdrerzpq.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gmuoevhws.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gehfcczis.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/grsycpnzc.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gymwvfwkm.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gmhmxtgmo.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gvxhhrrij.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gneoqlqdg.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gjyhbawus.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gfvgcqlsj.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gbhwlojaz.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gwqjtqkgn.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gittxkojx.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gdnqapzjw.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/ghkiajgjr.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gxxcgqacq.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gjhldmdae.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gquaowoem.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gjgycijlj.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gddagdogd.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/ghovnsrqc.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/glvtjeulh.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/grphgpvfm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gkkljgqqw.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gxnjrivqj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/grmrgglzw.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gvtgzqbbs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/greibyvob.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gnupejfls.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gzwurtzqz.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gqugbbtus.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/grmjimhll.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gphnvntlp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gpocgigdp.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gqqforsjf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gvtcxkroi.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gghavholb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/glaqhqght.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gzlphbnro.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gkhotdgpj.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gdugldtxs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/grgxaewsi.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gcpnscclv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/grfneqffo.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/greagvfhh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/ggxdswfww.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gkldvzsjl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/grmufjkfh.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gyxuyafbm.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/grvkapggq.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gutiyrpwn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/goctincnv.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gbzmuaexc.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/grnshuexm.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gvleefptq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gpztaquee.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gedpqwvmf.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/ghbotevys.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gkhrydbnl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gipwqixum.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gwyzullxc.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gqcgcuvef.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gmkwxweou.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/grsnailib.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gsytbmkob.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/ginmqlsmi.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gfcrlpeag.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gbsxccfgw.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gczlunuma.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gdfgleqya.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gosupaloj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gakqtfjtx.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gjckewdnk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gdrgatvxn.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gjwqifinc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gdvvbnger.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gxiwppkhr.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gpflagrdz.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gwiaryhtb.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gommpnocq.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gcmbmfqvg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gshkfkwjh.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gpifvrmxz.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gwahfoysy.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/ggrreebtr.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gueijphdf.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gptvrtnry.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/grtyddggu.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/ggkyuuhyj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/ggankecok.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gwaqfsenx.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/grevysxef.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/grdrgjuab.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gwzjqnurz.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gaoukcvim.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gylxstfhj.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gyxartnet.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/ghpteffjh.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gquejznxc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gmiuxgwqa.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gtqlwokue.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gmrmuorss.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gtxobvqhi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gvvaukfrs.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gcpwewwsb.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gxxsndhfr.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gypdnlpwe.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gnfqcwqmk.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gwxbjoxfr.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gbiasteou.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gxzmlzwrd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gharpvhkq.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/glavpuyiy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gfagxraii.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gbxqhqidu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gvoqrmzvl.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gqzydlcmp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gzzzcawst.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gejckskaa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/givhebsil.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gkatkusij.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gpkwqngim.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gcczmztve.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gcofivryh.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gupmtgtim.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gxknuxssn.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gopskcrme.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gvfeodcrp.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gbndmaikz.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gsmfxkhnh.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gnvbhvfxo.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gdqerpgmw.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gspsxpuhp.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gqnlsbuwx.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gofhtqykz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gehennlte.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gokwpgsmp.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gzvcyujvu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gylxjrqyj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gqojfiqnh.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/ggmqgzsix.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gbxrufwfe.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gnbcfbmgq.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gaxbbqujr.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gdzlxzfnw.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gseleouth.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gmvvwtavv.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/ghcznqufz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtillppha.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gneaajrrq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdpzhumae.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/grlcmeqpg.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gxzulswrs.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gsbetsxki.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gsyprwpaj.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gltusclgf.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/giaokcztf.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gjnyoobrl.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gvhvhxxwf.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gunhkiqrw.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/ghztzieyk.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/goarriiqq.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gyvxhijpz.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gitwasbdv.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gzgctqeoh.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gkzbihzim.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gppqgemws.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gdbniqova.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gtoosuzjw.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gmxpcgzhh.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gqesawnjx.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gcddslxxv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gquoqikyr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gebcbjivp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gavujmdyt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gkwqxfgdc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/getujaqxz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gktihiwps.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gjybvslzd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/ggoncemtb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gkmeziyxl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gwgllqlhj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gbvyckmtj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gxespdcic.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gygbsrsvg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gudvfhadj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gmlqpexap.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/germhorwk.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gtyxjpnmt.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gffmnxfbe.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gwbvoxpcd.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gghqzsmlm.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gbmaoeqqb.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gmukammyo.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gebsiuvsm.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gjbtkhnvr.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gxnitlpht.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/goazprebc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gckbrpval.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gfqgazzki.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gbpvkosbb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/gmemungdg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gtxmvfirh.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gqovfclvz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfidsooil.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gthkovxkx.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gxcxhvuik.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvtezzmzf.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gnvbudrdb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gjzrnhmps.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gmwcfbjca.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gjxlkqvoa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/goqdqoduu.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/goqvkvdxp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gnfshecuf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gvvvimfvz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/gsngjoqeo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gsgguffsw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/gghxoawnb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gtzucptln.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gjmwtxitq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gvqegbscv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/gbwtbcsvm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gqgpnwrck.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gpcjcflpp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gzaytgrdw.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gvafovypz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gwndxfgfv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gcgfvxeqn.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gbvdljjiw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/glkqzxano.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gvlrbiemi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gtbobzucc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gbyqawdej.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghagkwfxx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/groamipsx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gkkzwzrmr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/galfggkos.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gdvbgkvrc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gpgyfgvkk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gedeqbkqo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ghwkrhhtt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gygxbvmbx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gpkohqfwb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gtkgsdeif.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gctvubxjl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/ghefjlkus.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gwfpghbku.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gioncbvyd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/gkitzcoem.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gcuznallu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gsdovbydc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gonttlmsf.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/ghufxcbmf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzopebyef.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gjweiazje.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gwfjarxwr.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/guvoormdm.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gqwrrywma.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/ggbslgfvg.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gmtsakakp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gjekdjzwn.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/galqyegqs.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/grhadyvth.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gctftkfed.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/gkunocnao.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gbnbpewix.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gxmobsqda.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/gqfvbqssw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gmdczyiww.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gukxmpqkf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gvxceknfc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gcdrsnxqg.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/gacfbhgwf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/ghkxurlnd.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gbfefcdvh.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gmprirjcv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gxrvvccgu.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/geidoijlv.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gtocxlplh.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gzqgmdber.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gscrgsknj.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gtovnmrdm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/ggzmtypod.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gvogpqfhe.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gzoleyxvv.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gpaypxuga.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/gpevtdbdk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/ggmnsivup.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.hesvh.cn/Article/details/gfhckwuar.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gojrmmcjm.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gmssntkmp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gqnhhvkuo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gfnaknuti.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gybayyepe.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/glqrjndde.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gkzpwwuoo.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gbzrswpql.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gnaksqixh.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gwwnelnxb.sHtML


<!-- 参考信息 -->