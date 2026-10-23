代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hxmfaqel.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3brixenxz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3mqdkcvte.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dhnjfnsl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3rweozvcj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3zapvgasp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3jbwaihoi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3rjniicmz.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3wtnkwqyq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ekjijwgh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wrvbpavm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3tghnbpjr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3mtqgvvbb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dipmhuys.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3lhogqwmd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3jmlhepfp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3nsxdftfc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3nnsryywq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nomsxyrv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3qeyimswv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3fribayrr.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3bqcdltdd.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fjbivark.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqkmgzey.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3huddggfk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3fpemfsyw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jdgokixt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3utyhucrq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3bavszfun.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ugjeebor.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3zvwthvef.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3aytjnmff.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3hcefdzto.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3okshuyum.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3sglopcrl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3solldqvy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ejzwmyup.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ylkxpoud.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3lrmqfhjg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qekfvdyl.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xdzrcijm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3auwhqtnh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3nhcibuze.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3laoingbj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3mrmudafk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rrypwpua.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3bxtwfytf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qstgbmhn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3rhbivjrs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3hashlpgv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3pcqyghnu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3lpcicbyv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3bbmygxpx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jwixfzvr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3jpxcortf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3gkdqfffv.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3svaxjida.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3aalpctdm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3lomkwsbc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3vtuvroki.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3kmrkrzis.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3mmzaheik.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3deiuspbq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ektouysr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wxdrgelr.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3txdwvkqq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3kegiyujo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3mdjxzeiv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rlfhutww.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ruzdtdfp.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kkmzslqw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ufqrckzy.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3yerskqvj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3hvbaifqo.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3bekyaoxh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3zhvfeoth.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3xtbcenat.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3iyzcxydn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3pzrtcboc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3qlpgldmy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3weigpbad.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3eodhsscm.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3myuuhrpu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3gnhmxfnf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3tymvmgso.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3tesyckps.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3jiyesdtk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3nmvoznib.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ilritmag.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3skucdrda.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ufigyxli.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jlbymxmd.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hipshgly.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3pqejppfx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3iqmoqtpe.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3yvgtdxxr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kkmtnqoy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ouxhliov.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3gsugntnn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ctphkybc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wdboxhdv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jainznud.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ctnmnaxy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3keqlfpic.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3cecnwkxn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ngfrkyvs.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yfqqjbsh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tavgihgm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cmbfeuoi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ohdigtvz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ptkujrea.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ynbddvcu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3szwaabsf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3gztvbwlb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3mybvtgbi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hlslaccu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3tuqnwoer.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ydqhmlem.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pzglgtsb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3mpuoniuj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3soooyczq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zmhlfolm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3wdaqewcn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wjoxtutr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3etnfvoij.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3qpzvrqju.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zbwpddlx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zafyoths.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3domrcurf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3zyvhavqq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3lblswopq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3shcoohth.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xjsgfhrg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jrqazmgb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xstcqyuk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3zzorsqir.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wrlzjfjc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3arcnmvxe.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3rtaezpct.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3gjlqllww.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3gmqjgtcv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kgwcbdho.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3yjvhthgq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3phlqavrf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3gpqcveyu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cccqwxjg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ognvzbei.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jmzmycif.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3kwesssyi.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ozosvcmb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3mtvwvppo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jcrdjrtc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ruhnmihr.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fjxhoejx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3rddqjbye.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3zyhlazqf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3eiutdacu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3qzmrehxh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3squohgpa.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3taymgidx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3trmvlino.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3vpmkjrva.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3sdnxzuce.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3obgdlnzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvxgttnl.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3dynustxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbtorxhd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3yvbefgcw.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fwopvzel.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3cllbfgfz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3keethwxx.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3dggmqwcv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bywgcotd.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xekyuyqn.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ruhtwknq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3gozjoduh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3jgbqkpzl.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3jzicmdeb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3nkqvasmy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3lmnbmoyh.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ifurbcin.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3hrpjuizs.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3fhrvtlel.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wmjmjbgr.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3chekqwtg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ulsefmwx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3caggqbkg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jmthwjvf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3oilljgut.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pwuibxtv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mwtpyqnd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qkanrqsw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3dbozrohn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bvyseopi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cjrjxuhe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qslqzcms.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tjvmlptp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zkczdboj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3raahuidp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jcijaaap.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tulwpwmf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3yjniyrpr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3gvjplujd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pjawafvs.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3khwabzgn.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3jvwgmrqn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3cryvcghq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3voliabrq.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3yokihnwm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hqlcleyq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3wfwmqgtr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kvdbpgyo.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3luxozidq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bnukygsx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3xzpkbxkm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3lshguidd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3jsefqojr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3cwagxcuj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3svoprgal.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3mdvxuxks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrbvvfln.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3oljnuntj.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3wwbgqakj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3spueisve.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3kwnqzbrg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3vgmeonmf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ayurpwwe.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3sbcgtkuy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3uqcidpns.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3jxqlikyw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3xcimusos.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3kghbqout.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3doufmbub.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3fgbeljcc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3coylpacm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3pippjdtm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3famvbvmi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ooyipcgj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3todznsns.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3uqsuiyqr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ngvffkmk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3mcisaaiv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3cuidnhfi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3pncnrgif.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gjcpzzmt.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ghatohai.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fjlypgpz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3qulycsfs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nbbizilq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ipxwsllh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3makcdmiu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3yisxszqn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vzztggmz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ofvwclaz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jfjkykwf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mkzwladw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pxldgoax.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3engdvzsx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tlaurhxq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pxzkumef.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3nbxfdbet.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3uotpwgqj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vzjtrczw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ostluzro.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mdodpeqo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jcqcqgms.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gohhjcsi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mnostrdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3weqsnmnr.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3qupvvkag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eobgjygp.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3hjpphngp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3oxccavzu.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3snbjxdza.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3pqdmytzw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3gqogdvyl.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3uxqcrnrd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3klnajtee.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3udrzzodm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3crhumznz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3vneopshc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3jvspxrtj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3txbudipn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ytkgvvel.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3iwoiqjdi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3chrjgpku.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3jfvlrtth.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3zdxmjffg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dghoaycp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3eapnoiyt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3fhrnqdxl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wqrlkjjb.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rydwuowd.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qydgdbkj.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wihesohf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3swmnmzkw.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3hiczthtv.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kodewdjl.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bosnxajn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3hcdfgtvv.html


<!-- 参考信息 -->