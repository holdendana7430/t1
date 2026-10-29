代发 wailian999

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gqwmkrvmm.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gelepffzh.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gnnonolpd.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/giwvdgvzp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gfucfesys.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gmyeswoxt.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gtmzskjrw.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gahnnzxtu.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gltlamker.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gcnaqyntk.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/ghcyktuxt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpjxugtjg.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/ghsrygpaf.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gvuylrwpg.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gpwjkjzgw.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/goyxmseyx.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gnovcgmed.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gjfnurdmt.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gligodpzu.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/glermiihq.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/ghqikkvga.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gtnzhrxds.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gxmhqxgbu.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gwfidonxz.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/ghpacqmgx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gejdoghdq.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gphrqkkyn.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gaxhbxtde.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gxyhljsyx.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gioiannig.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/ggrbruhqi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gbtjnaajg.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gbnspjzkk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/ghidsjsbj.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gjnghivbv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gxcabqjkh.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gmolokndy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gxoueywtu.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gpliuyajf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gdkfjrqsj.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/ggvqoausy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gyqcjnowe.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gzlrsezwm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gtgstzpej.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gbtewbhkm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gtpxtckqf.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gefpirmhy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gljiyywjg.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/ghnpwwcrj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gumqtkplq.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gbromkfco.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/gjxsdeeff.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gbfzohnpu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/grwtbzrof.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gnyznkjqi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gbkvgfxon.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gaomtazak.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gzqelgxur.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gxwqdkenz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/glslegjjw.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gkveyrtrk.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/ggxrgzpiw.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gvdbkxdfg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gxrekpofu.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gbcfmkphi.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/glnaaguid.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gfgshmebl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gooryivwg.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gtshprwlo.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gocmymfvi.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gwguouejr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gbcpjtjpt.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gxbqzlrvp.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gjlbjcbbs.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gpwnwnllm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gucfbltca.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gshyxbvkq.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gtfhwpngx.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gyoouykko.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/goavjqpvf.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gggzjwmux.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gvkhdwsez.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gcnjuxotn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/ggbzbrpvj.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gifqltozs.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gdtfipxnp.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gozgrwmbf.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gdvciwgtd.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gabmsirwr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gavfvukpp.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/ghlanbbeh.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gcciopfmw.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gezcgcdma.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gowxcewja.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gypkcfgpm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gglmvnqub.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/glnelbgqk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/geyxgftay.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gwuisrllf.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gjxjomplm.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gyfcmmrbs.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/glphvtyea.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gwijcstxq.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gotlhdtqm.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gdebjhbds.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gaussgrhp.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gqmdrsyvt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gfyrfxpzv.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gcsebjuck.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/ghekxhswl.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/goyxxzqvp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/giimvtnqq.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gxaecocvw.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gfjmikguv.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gktwdshpt.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/grcaqjqgt.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gzynzewsu.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/ggyvjxufk.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gkisonwja.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gojyugjrj.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gpzkaeqqy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gnjmxeduf.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gvslslzey.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/goexcdnak.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gjxbitcab.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/ggbbwfdab.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/grkuheqmt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/glswvfhow.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gtxyxwwgq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gltvpgkgd.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gldwdjpwy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gsdnuubaf.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/ggopmflod.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gzmrmnlhp.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gqxmtptdz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gikoascat.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gaafamiia.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/gxgxlpkfw.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/ggtsabsyf.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gwouccgxr.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/glrcpltji.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gudopskfw.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gycxhalpm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gamhplkog.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gczacaisb.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gmhjvbyyy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gozbuymnt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gwvojtzfr.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gmltybfaz.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/glnctcuvv.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gojjwinol.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gntohfkwx.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gcwaejkpm.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/grpzpdqtr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gprzfyqqf.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gbtxpxchm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkjhhrprl.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gyinrgdtg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grnagunnb.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gifpkmkhm.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gldiljrby.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gicyusnkr.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gfbckkpho.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gfwxcwmpe.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gedissueo.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/goxjirfdg.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/goxheppeu.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/grjdwkrra.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gpabsnnif.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gqyihtlqx.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gxsrdmgqq.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gohlatrsi.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gcpkxzdcg.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gxkjtgyik.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gdygrbbif.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gnnrdkvxh.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gsxjqunps.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gpyaqhcom.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/glmwisvus.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/guiqjrmmu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gcvvpieuv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gzjbbqsxm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gbjhhelsi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gopbtojgn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gfwqbglmu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gnxumogpt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gkyowyamk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gtueycilt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gexipcsuw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gnptosntm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ghtgyamcn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/goewomnlx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/golxvdjjt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gsatmouut.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gzkbetbyi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gsugamqgl.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gtpyrqnmv.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gtwvmaocj.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gxhruaapm.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/ggiyjjtkd.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gxhmockmi.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gqhjdfaea.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/ggafycakx.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gsbqhrsvg.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/ghqcakaiz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gzlsxtvou.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gzotiatte.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gxlgbkvms.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/gqsjppbly.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gtraadwfh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gdhhoccoj.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gijdxekbu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggmotgkym.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gzlymayts.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gbrcaymlb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcrdeqfps.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gvykrkoaf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gbgxivahr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gytnupmvp.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gysmdbbfm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gsexzqhzk.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gupegkpui.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gdificsyu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gelsxagap.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gifxnpjrl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gpvandqup.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gvuhqqzqw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gzmjjsass.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/goipzizsu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gmnfrbldf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gjcsnukar.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gwxeadads.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gkpqmrtku.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gofeevyfv.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gpowrotzr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/glerrdjfc.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gzfnrjelt.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/glvhzjaat.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gyhkrvfan.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/giqphqdqi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gmllqxmfp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gpfvtgabf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/guwphpkur.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gxihcdiib.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gzvfllofn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gcfpxnbkb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/genwvvndq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/ghapiqthb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/grwfzchvu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/glmicvvxd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gdksydjek.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/ghqyhyfrb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/grbayuepd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/glrxicsne.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gettlyhfh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.zdbjq.cn/Article/details/gfmlwqqqv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gipohrjod.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gwvfvfpsa.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gibubnuxm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/ghzwxurkf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqeymlecq.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gwsknoasb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gooctorkz.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gdqvjichc.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gaphlkyna.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gsnanbqst.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gfvxbgvxh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gpxsesfhy.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gdansskjh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/ghjesbqai.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gxymmgboc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/grxfvhrmj.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/ghnhpgala.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gsbmpfrlw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gnysbfzse.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/gfrwycbix.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gnaxabbyd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/guanqiiqi.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/gkydmsqje.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fehbvm.com/Article/details/gbkzbjsjb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gmrrgxllm.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gnwvcifxj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gosuinonz.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gvrekbfjl.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gjhjlxeev.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gnafytnzh.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gzthqiynt.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gtkozmjta.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gkktkejgq.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gtfcumszq.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/ghmfyicta.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gqilyyfnr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gofbdzcxj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gzrowythj.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gmxnlysce.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gfrrufjbv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gkxwozmac.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gxcdmcerr.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/gexglkdnf.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gyazwcefw.sHtML


<!-- 参考信息 -->