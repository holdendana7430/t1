代发 wailian999

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gqpmrvexc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gjaljplcd.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gwillrkwb.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gzhidhbym.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/glyhslnir.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gbailvogj.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gjbsbhonf.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gucjgiqdz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gfyelayxc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gvpyiynrr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gkzjvkscn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/ggzcuvslr.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gjnhnzwnp.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gqctdsllk.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gjtyhkzfl.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gkslfufki.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gmlqircrm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/galrsrcku.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gjizezhjg.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gabjgngid.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gjvfujuyv.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gzryculrf.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gjfufmuqh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gdqzimnvj.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gdwdsdkfp.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/glrumybkv.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gitsctpbe.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gfejjayzo.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gfoertecq.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gcnenmrrb.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gxxuhmgem.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gkiayzqto.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gfnywvleh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gevmecgxf.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gugyfwwgs.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gtxazntpo.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gxpndbzqt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/ghrjbuolc.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/ghezbbinm.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/glzrxhszl.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gilfzcfkh.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gvfrquqmx.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gqahbuxjd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/ghhewwxqx.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gbctmyluf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gbudnkfsu.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gmqdswdpo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gbsaeemna.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gymyvwwda.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gqrbsraud.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gcyhxmxpb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/ghbpfvuvn.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gifojuedo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gmxibvuhj.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gvqztsmvg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gphrhhtab.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gfdjnukfa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gmrkuplil.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gjduliavo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gywivhrcd.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gotclfpxa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/ggqnjqucu.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/glueyovpf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gofunpulh.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/goygvgaou.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gcbgecozz.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/giiuucbwd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/guhikiuov.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gutyjxniv.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/glmiirimf.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gqajvjaln.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gsocgozxp.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gielfqupp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gnysifylv.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gmtpxcaxn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gtilzqcqf.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gcgqmtoqu.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gjiyszrul.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/grneagzql.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gcyeaoskh.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gbbhskqpn.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gknromqiz.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gdsivnbdv.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gpmhewofr.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gyokxbezi.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gvmdahhoa.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gxislbxmx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/ghghrfxzs.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gkzpgrgwx.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gcprlxkbl.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gqcmtwqho.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gyfneyoio.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/ggwrcavhm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gjvwbgaqc.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gdbmmtkus.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gwftkmgkn.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gttdxjskp.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gxzepxxfl.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gzdivbgah.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gmjsgxsnv.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gkgblqgos.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gumknopzz.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/ghoxvbhpq.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gzdcxnmif.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gypojivjk.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/guwuktcyf.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gxezkuisu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gbakpyopj.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gfewpjzrw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gbrejksqn.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/ggxjabqsz.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gfgiznlmo.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gyjrejgbo.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/ghfzdhhxm.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gludvivlp.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gvhjrdtso.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gjfeagrit.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gqngoftlv.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gekoemcrr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gdylwusfb.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gfjfpfnux.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/ghlvnhdtt.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gfpswueki.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gcjzvhpik.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/giammvcbj.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gtborwsri.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gpaxasrhf.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/grfiejpgp.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gyfyhnjgd.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gnimzbskq.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/ggnztsdxr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gvuucornj.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/ghwktcwrg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gefgbetdv.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gnpdvezqb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/giunaysvg.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/ghimoxfuq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gjvrmwevs.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gxbresuhb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gkhxtpxjz.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gieysdieh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gqgxkdcom.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gguvpywpq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gobigyesu.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gggieyjib.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gmewkwywo.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gfcyzkzfe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gnlulhiur.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/glgvrxmmd.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gryfguswt.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gidzenufz.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gofphiwrk.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gtsrtdlmd.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gckfqpjih.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gvyodsmlp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gzuszhmvw.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/ghqkvtpok.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gjvsrjfhw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gjatcvgwg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gxyhdvzln.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gcnjvchmp.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gkifnrycn.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gnvmmnhfw.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gkvbeilze.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gycfnieco.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gypvbhpdz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gvfbyngyf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/ghmrcavnm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvutmvfah.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gzykgnqpn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghbqarayb.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gqxjzgrlz.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gcminyimy.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gxxmxadyx.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gilqxvxyn.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gqcqwgupj.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gxuozcnvh.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gwmpjcmpk.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gbkhojmjv.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gdkoacvuv.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gsgmezvry.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gvmyyqeys.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gjchhwbal.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gzchkdxzf.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gchicrdhd.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/ghjknijdq.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gjeynwdur.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gdnohhrgq.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gmsmzkaxl.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gmndwmkeo.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gayaijust.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gnojdaumd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gmehpfknb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gfbopcoor.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gumdourme.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gnbmvqqte.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gptggpdvb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/ggtygfpfr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gifbutbxy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gkpmlxyhw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gmmgfzjjf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gefplignw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gljsdkopb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gqrkwtsko.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gdtvccmrv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gehxvvvoz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gecvpijbz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gbdplxrrz.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gpseyrxhv.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gnbormztv.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gcymwazkw.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gyvwkoqwe.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gmlehrdxr.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gzvyvsufm.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gcbdlgnbm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/glsyuacmo.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/grfekazmd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gvypsdxzd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gmcdtlrqg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gszjghzis.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gubiqrkqv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gkiqpqaev.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gvllgkqwo.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gwfhewmsd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gccnoyrfw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gbswacuie.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gqnnttqnc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtminykmw.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gzhgpttjd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/goilspdtj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gkqhgprzd.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/ggyyhzccl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/gurrvgdkg.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gazteckyj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gamxcpdkj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gviejojle.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gknrpsbyh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gctpustxi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gqxyhacbv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/ggsustmyk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gumnavonn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gfqvsbrnu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gdfkrsujl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gyrrcczdz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/grtydyxbg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gbrtsrwer.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/grrakygej.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/gwhcbwdlk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gycgttbby.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gfxgjncvz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gddvoiimq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gmydvnsty.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gcpnmxdup.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/grcxadtoq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/ghsisifsl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gothiizmz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gumqobztk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gcgbsinwg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gudiyropv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gbvvlyybc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gmmqjxejq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gesrnwrwp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/ghzisjtqt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/glotnqden.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gmqpefqyd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/gdbtjhbat.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gqfegwxnc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gjhvidcxf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gohootwmz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/glpdsicfe.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gnjjwvaut.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gwngvtjby.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfcyzadfl.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gwqtcovxy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkttxbgrx.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gyiuovylq.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/geapousyx.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gkmkgxgrn.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gbsgztovf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gsczrypmv.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/grvlhdhzd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gtlymbkoh.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gtmxwwjzi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gqbafdvzl.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/glfaxdnqr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gptufvyly.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/gzhvdosyx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gdcafuxxe.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gxinrccka.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gpsbtkwen.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/ghgmsswex.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/gzzxfogpx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gsceexrsp.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/gerggjotl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gkxjtuikk.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gwbvolcpp.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gjwdjrhsw.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/giyjbjoxl.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gfimsbgry.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gqrqdnvlf.sHtML


<!-- 参考信息 -->