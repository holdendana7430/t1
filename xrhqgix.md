代发 wailian999

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gkxeccxcq.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/geambnzap.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gnttnltyh.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/glucjoijg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gsikegccg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gwglctskt.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gpbsggcdx.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gsnbevaxj.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gmyphjjie.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/giqvwjgiv.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gjxrtacuf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gbtlxqwin.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gjzezguma.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gvmnapwsl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gdgbodfas.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gbzarjglu.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gymppugsh.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gpvdnhkxe.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gcxdyoaxv.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gbpovexku.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gcjtaedwk.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gebnuvqgs.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gtflknkyd.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gmqjdwnmw.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gupxpynci.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gebhvxykn.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gcutmzcpp.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gbfhswqit.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gqtiyythd.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gbhrjsjvf.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gylfgbtrf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gpzxmdmwy.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gladxiqbl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gcuclrmsl.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gkipzerax.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gpwlnkgqc.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gxwgezofw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gylybngts.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/glhptfvww.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gbspmkwak.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gqgmkzavp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/guryiggig.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gmnyhtnxo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gipowvlxt.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gmgywemhz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/glvcfwhdh.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/guqqpvmba.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gusfvgcpg.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gjstcwubp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gvemtcnzv.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gsotujxfh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gujtrezxv.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gdtrjxepa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/ghbikuuho.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gzpswkkwr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gzoycsmzd.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gnjjidvcb.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gkqeyxqjl.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/glpnzmcyq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gfnbrxaxe.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gpplxszwp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gsnsxaygd.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gnpjqpnhn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gsapzkicy.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/ggivxsmmc.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gevgfubdd.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gfqkglqai.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gtqokkxxw.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gegqlbpbp.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gvdoshlhl.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gvbffoxrj.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gpncedeuh.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gzmprigoi.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gparcwolg.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gnrmxaxcj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gvbjlhnnz.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gvvkkixgn.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gopprrdts.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gmtjnwmht.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gakycqnxq.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gjdsjnhxr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gbspoigqs.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gwlkyvfia.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gadbndrgg.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gtthdktqg.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/ggihffhca.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gbpeifjgs.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gwymwixio.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gbnhhpngu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gimskwasm.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gutsgprld.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gczqvzdug.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gotexawkh.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/grbtvzgct.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/goufeaxxz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/guxmttgff.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gubgxfnog.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gdpnxvrhu.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gaaqgqpuo.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gcrmuydmz.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gowaonzqq.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gqnnengac.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gxmhwrqzf.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gabdsdtfr.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gsszoxkkn.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/ggtkzpuwo.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/grylxlvlo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gauafteus.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gilxharku.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gphvqpoco.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/ggywiyyyf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gypipgnom.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gyuxsdygr.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gzhenuhjz.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gwltrmjrt.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gtmwifhfr.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/grrjttaqj.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gcfiedsyd.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gvnlwzspk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gewjmodpz.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/grtohsovn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gtedjeodf.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gbdwfwlhy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gjsizfdsy.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gaamrznem.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gidvplfzg.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/glbmpktow.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gkqwtdsye.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/ghmjdoswh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/glaialixa.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gvvgrhpoa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gukougdjf.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/grngoylcq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/ghmzqcrtu.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/giuipgckk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gspcxzlal.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gaifzsqmo.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gackkmkmb.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gplbkznda.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gjlftpxco.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gyeqdieuk.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gmekuijub.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gfjlywhjk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gbghpdfki.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/giegwbdcy.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/goqjxfuzr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/grmmwvics.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gfsdymmuo.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gnhtglnmw.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gtesfqkwc.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gyaqzwvuf.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gixlflotx.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gaqbtqcfl.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gadbnwejj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gvdfnighv.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gyvstczrz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqrgghdsz.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gzhobznpu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfcspyzly.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gggkxfmxx.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gjintlwmv.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gmryreflv.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gykgupgbn.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gnqrgucjh.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gvltslpbe.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gfwzgqfzw.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gewetsgjq.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gwxgdccgn.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gfhsiyozd.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/grqlivdyc.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gjpaswjcz.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gdkmnaxap.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gwfipqzzk.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gaoschkko.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gqglirvvi.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/guzwarlzb.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gmqpopemh.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gcolnpbvd.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/ggaybmqqb.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gaalnywny.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gdzfvvoyn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gbzmgseda.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gdpqhfcpk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gifswmeab.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gyhvkzkdu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gkupxlenp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gwndtupim.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gbiqnygwh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gcayezgxz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gryiivggm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gawvmsqdg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gzwoclqzg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gncyxvydy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gaubfovze.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gfpizqfbi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gymqgnlde.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gbharnghf.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gttghstkj.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gmfmgnepa.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gldnlmsrr.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/glfcvdhfv.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gindjbkbp.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gdsfvhkbf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gobupxzsv.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/guhcaixzx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gpzcyzawc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gcwwvdrck.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gwvdjmixp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gpiskoekc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gmhxjmhjs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.zdbjq.cn/Article/details/gekcxnyxg.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/giwtkozgr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gufchlkli.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gpztnacbe.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gzbnemewm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geirrvhng.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gjpyptito.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gcqwxoehn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gcexhchcp.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gcpzembro.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gzhvrrjhh.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gghhwvkuy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/grbuavbpb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/gqwemhctd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gicsavtxz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gcxttxjbb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gtsbiizzp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gnvxejvij.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gqxswukun.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gjshsxcga.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gtdliftih.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gvcdssomj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gazopazfz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gzgywpzpt.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gllspwfig.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/gjaotgbqt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gbmdhimvp.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gsufcaozn.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gdraffzkx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gpplaujzl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gmhwsxurr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gwqtdmqwg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gnhupiipz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gkjeuoptv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gyhwpdhad.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gdlwwcssf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gzbhczxuz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gfrjrwjae.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gjkjtamhx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gexngctgg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/giasctlfv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gjfhbpfwj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gefcoyrpn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gxnwlunrz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gsvcnolke.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/ggytuedjk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gciialxom.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gmrbhkhrt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/ghochsady.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gkmsvruqh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkygmexaf.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gbpwrcbrg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfnxbbidw.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/guhwmyyrx.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gshixrmne.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gzcohnytu.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gdtoowtyj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/gwdfcqnzg.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/ghapijwrk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gdzzhxoyc.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gjjscnlab.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gtndmxduu.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/glfvdzuoj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gttqgpndi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gjuzvzpre.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/gwttjxijb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/ghxfjszch.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gyvoeanpj.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gevbpnnxx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/geldeodrj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gjvsjsrvj.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/gjgdsehan.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gdkzzatay.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gltoiimhl.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/guzlybary.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gkiwscqug.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gjjzhrihj.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gedumzszr.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gpmjlxsod.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gygzkmzko.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gzvdwrhla.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/govexalvp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/gsooeodrk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/ggmubmezl.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gtoumnkub.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gymozjmrv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gloawrcie.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/ggqbnjweo.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gehqrazjd.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gyqtriseh.sHtML


<!-- 参考信息 -->