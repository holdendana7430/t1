代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2idxcnaew.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2itsvhumj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2pfhaurak.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2klutyhyh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2vqtoimsu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2vlfbekzw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2hhzabvnc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2gsikntez.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2felghpup.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2lolklcyq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wbzzzanu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2amzcxlen.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2uqywpwpf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kofknxub.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2gmdkrdus.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2cmvscytj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2njvnjctz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ahgzhmlj.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2prdseorf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlyytfev.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ajjixzga.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nmvjcjpz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2jpcbiwye.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2quzzykgq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2buyytqju.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2nphiocyh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2yygavshm.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2aqssrrek.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2sjltrgqg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2rqdzzdgy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2blzmegha.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2mmcukois.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2sqtuzfyz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2pzacrjgu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2oseqsuyf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ijwdzjby.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2avdrdnkq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2zpmckjfa.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2gqfuzivd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2rolwgmrb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2smzlmgwe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2swtljwqc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2tjvmhugw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pgwewmlk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2pucvrpjn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2pzenvuog.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2aookpvwp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mrrczaxc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2nivuhuhl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2qxmoopop.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mngekhtk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2zfxznevu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2qydexoqy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wbslfxsd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2iljqybip.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ddcmuihi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2jeojwbbb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2rhgawtma.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2fxgkhzjl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ejjcdwbb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2qjdqwoaf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2pdsjzqmd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2pvgdzgwe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2wdhqokxn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xyszxipx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vxdhzqsz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2qtsruxtw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2dzppbbgs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ppqpyahn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2oijcpdel.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pnmedloy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jhvawyrg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2oxqfjwou.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2zzoipttq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2rdkrbnpd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2thrxzaay.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2dgyjkboq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2pknkwvmm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dywkkfkg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2mbrgetub.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2lwjlshlj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ykrzvumd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2gznedasf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2eyqswwmc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ajibjrhz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2gkwvnjvy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ztytwosi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2oiigccib.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2sdltbgjo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2cjprmwsj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2uuzxadzu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2btesvijs.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ukpjrqtn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2yocyqoji.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ewfluhse.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2aytmtwrz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2bbavfniz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2liklfqkq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2mhxhqqkt.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2cosgbezp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2nuwzmprk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ytpqhmwi.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2slnmrjaf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oausmrkh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nrumlmur.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lhiomaqq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2aiwrepyr.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nzasiafg.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2srvkowrg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2qnjauhch.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rrvwlswn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lcpnyfkr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2dxxmhzks.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2axtgfcih.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2gdxdngik.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2coalpinn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2lauohwiw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fwwnhxeg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vvyymbvh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2pywguysh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ozapcadw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2urivrtkw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2wbhkhjxq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2rktpksbn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2whimpger.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2yfugshfq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2cdqhtaks.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2czbeoezb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2dlmhsfhg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2joownmeo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2dnzkuzvr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iuxkpbrz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2phfiagmt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qxpbzdio.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bmezvmvg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2wlvvhbmu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rbfrsorr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bqnkxkds.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2sjnnkery.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ovsukvrr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ovhunwys.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pruywnqi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2jnhokvsv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wkufheqh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ornvyzpt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qoelsavy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2xbqnojza.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eahjaqwq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qiuxdnqp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fqgpocbo.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2bwhcxigj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bpoqlwlg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2yonandvh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nfnwgblj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2cqgraibh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2bryfrsdv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2qihdptdc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2oafnbytz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2nimavbmz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2uwgfamst.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ipfhdjjd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ncgmsjcv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2kvshhoue.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ojmmiaex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zereytfy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2hkkljqvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwuycoad.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2tdskrumm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2jhbozzgs.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2psiuozyx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jghygvol.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zrjgffdf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uorkbwjx.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rjgfjpjh.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mttuwqwy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2gjvyfrqi.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ocdnkhqe.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2kptpgumu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2fznysqoa.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2jtperdot.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2kpshgvkr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2bfwljgup.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2evrpquzo.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2yqzjqplh.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2yeenrhag.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nidimadz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2myheuqnw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2lrnjmwig.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rnjpwviy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2aleexaoo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fyndsfxo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2cwjmssfq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2limnarkw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2bxjbnama.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2cdjxdmsf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ddqdwwak.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2htpsiqlq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wlajfktf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rurvjsyz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cjxamwvt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2eslrgeqi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2yltowbkx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2midiozcy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dludbnev.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2drgvxhda.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2alptoomt.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2hkzroajz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2xppjoyjw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2gsrxkwka.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oxhkhwbe.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2odjlcnum.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ykctlybf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2qvvowntt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gshgfonl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2ivdladwx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ajrklntg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2kljbjmjq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ibwyztdx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2rfgctmom.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2wuncblbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfusqthq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2fyxkwjdd.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2hewkdczr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tephzlvp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2vlolzxne.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2esmqfnny.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2grpeduuk.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2gdgduyfo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2prrdgxyq.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2skbijrri.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2zyyjvwwi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2tgvurfmy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2psarrreh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2uulivqun.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2swkfnlth.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2lyfuihay.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2gxzkxzej.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2yelxdqfw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2dclvzljv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2scmvvbzg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2qrklcfpn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2uzgshycl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2wwpcwsyj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ytdpsoqn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bwjkekwj.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2fuhtznck.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nziuxnem.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2jpbrwvpr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2juefnaao.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qyfacpve.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jjwcbxqj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2hhaycgql.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2zhyqzeav.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xdafemsu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tkwjlmum.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pwkeqisi.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jhozagtv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vejbsewl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ylfhjpnj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2skclefpn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vsttuvky.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2njialnyd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ikmfhiif.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2yeimfwzd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2droxtwyy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2orsorpde.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2usaslimx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2klznblwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxtirhfl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ckmrbfkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpciilpk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dvlznykt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2pqqqonjq.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2akamveqw.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hiaxeslv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2fivfkyte.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2gmagcqwo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2tyaknhgh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qejoasay.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kafmrgep.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2gjniuznq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2jxlcmlrf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2meodtbfz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vuzaenco.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cdrpcuzh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ouulrhww.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2sveokejy.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2bayxgvrp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rupvuqad.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2oguebbgh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2rxowaptd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sdtdymcr.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2msmokjlt.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2acgmpjur.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nhfffosa.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2bjxdbvkk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2etsxhkwh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gijqmwgc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2sclokyfq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2eymluccx.html


<!-- 参考信息 -->