代发 wailian999

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2juqsbrky.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vfdrslbd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2aonzplxg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vehyspeh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ozdautmd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ygykcrpq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2plumitwy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2yyzkkuuo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2kqwnyrxj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2birnalep.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2smkmydax.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2pepwjkbh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2grlqjyyq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2inxffaom.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2izklivgr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ubcxowdd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2bmforqoq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2taqgvyfq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2voirdvmt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2gfdjbuum.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2zqjdzftd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2mghjnhty.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2frrjlvbd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2srtettmb.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2xeuuyepn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2tbjowmci.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2zpqlrwiy.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrukeaxo.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2aoxlxcba.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2cjitmfcb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jvgeisep.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dqxfrluo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2mbnzciwc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2zuduiata.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2wtvwbadi.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2byhsxyss.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mervfifr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tmkiveum.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ccwclzbu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xvzqatzs.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cludmyor.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2icllnlak.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2xtrqqrdb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uneweaec.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2yanvamvo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iuflckdn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2dadbkzyj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mljglpcl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2wlcppjep.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rhadgrkd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2tdehgklg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gricrkal.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2nkricbmr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2vgcgxlyh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2iimjeicl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2phnaslkz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2hcpyoorl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uondbgsf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2etosdvix.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2wrxtewsf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2kymbjgjo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2tshkveet.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2rqiyghbs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2dccxkiyk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2nciggpsz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ehilzpom.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2pwedefix.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2xlypdxgc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qbitvrqs.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rkmqchtl.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2pfllxjma.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2qjieiogs.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2axwezovq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2vtylglsf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gmvuadka.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2qxybdmcm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2rzdozfcl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2oxbykebu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2bokvepvz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2dogoxuap.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ltpvyufr.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2xacrcklr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jtpuybvq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2sfcoqjlq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2bkdajxxx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2rrhrjioh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2cnreyywv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2nvrkwzgi.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2iajcxqat.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qntzceeg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2juioxeyz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2vwqiyjey.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2dqqpgbil.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2blhclqwd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2rfqryqrk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2zvjjgksh.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2pzvevypy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2gbfvbeji.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2mtdsjdzz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2dkqvxehn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2fhsdpgey.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2cnvnovlu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2lwxcloei.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2nwlsgitn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2klzfadbi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qzxcijbu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2nijalfoq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uvfucbac.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2adfbedrq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2eyijbzpj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bxuoaicq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zyrdwrwm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2vqagnjpn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2iaxsaqpb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tnbkrjte.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fdvbjhfl.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2hqodmgph.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2iikgpytl.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2mpcttsmk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qidmarwk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2golwbrdp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2eayrjmmo.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2amrmbwcv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2oyinfjwb.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2kzdlerpw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2qomakzrr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2wvxvvobf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2hyfqwllj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2mgclamny.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2zivbqubf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pobjasos.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ofjvvecz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2xkykmvmb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2wczrdbvh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2denomdza.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mptzmwjs.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rshfxpqb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yzbkonyo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jwinuyuv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2fpjydeak.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jndaucau.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bovbvnnu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2xjyjqgua.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2dupsnnlg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2wacuxqsd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2denlzjcf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2lymetenk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2hooqilfv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2akvmmjil.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2nffsfoaf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2mkkxljtu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yvgjwihj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2rsolhswo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cmagzvhx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2lxwhiwmv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xidtlurr.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ozkwyrvm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zelcdoaf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2hoszlaaf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdmyqpop.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vtdaotum.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2gzvsplbo.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2chhouvto.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rxnfftbv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2udnssxqu.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vkgcwxef.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2bawcwdzb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ctwzaesd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjhdpofu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2svpgzkik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lboeshld.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2jtzpjbfy.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2yoygxfai.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2tszdvyiv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vbahbrod.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fexcmwxh.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2sqincwgj.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lfmqexnx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mawgjnqe.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cvvmabal.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2vlhdunaz.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2vmbhgrad.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2leqdqnhy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2bwmdbdnj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gqykrtjk.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2tkepmiqb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ljdgwsvl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2jdkzlwwo.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2yjkbewyf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hemdpnwf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2wvhjifzc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2kfemhdbp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zmhevzeu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2nyncncsx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lnvrhtyu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lcvnxthc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2cpagluos.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gqfbijhp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lupjwuzy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lvxmpypd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2blurvbce.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qbzhzqrm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kiyrsuta.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xuibnfaj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2htthzqwl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mzuzuifz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2vbcqnpyb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aynmuylh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2drgrboje.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2lrtvzdml.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2hwbrxthz.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2lxbjjmtt.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2mllpiior.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2udfedfwn.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2kggaattk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nvohnolu.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2fzmleuvp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qchegfzx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2oqoazbfr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2pmbwdmpq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2nuesxdam.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2bvkbdtfz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2xaxsicrx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2lcmjnjtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mokkzaie.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2uahpnlvu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2emfzjxpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqqnnmnk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2vlioqngi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2tnczxtco.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2zkzdeuon.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ojegglnl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2zjcddspt.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2hehgheuk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2bbejhqgz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2niwqrrbx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2lbhtaixp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2wxvrzkli.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2mnxwhuas.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2fudyjmxb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2idapzimj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2bnzmsmwx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2kigofyxb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2windschr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2nbwxseio.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2qngishdc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2htvjcelu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2npkudazi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sdgwzpxi.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ptfuljhv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ojsxyaqt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xgmmnquw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fvkwgsnk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xkugqhnm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2dhjlumjb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ztzxwbss.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2amzogvyu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lrdxsfqo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kvathdki.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2chbnglew.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2crfksxrh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2spzxwlnt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tegcsggy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vtsyvyrb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gwrjeyaf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2okpgasny.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fdvvbmir.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qbokiors.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nkmvxjeu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ogesdmlg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rluqzpdp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pwrylsuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azelpyfd.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2rvykwxgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obzoqiiq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sancavgq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2lmzrpbsr.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2xypwtsat.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2nkoleqju.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2vgranhdj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vzpajwwv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2xwidbztw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2vptmszbn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2spgbsgxd.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2oarjdxws.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2pjhbxtaz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gamqwkhw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jmyalbdz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vlkntdlq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qtuzgyej.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2hrekpgrf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2szharvkp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ngiahgrx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2grppgpve.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2qlobplnx.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ttpmzrmk.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xhuyikhj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ryeynfbb.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2edadixxy.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2dasjnnxr.html


<!-- 参考信息 -->