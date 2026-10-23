代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3fyfeemyy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3lodtwmgx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rzxlhjfw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3jrubiiyc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3mghrpdvp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3vqefijak.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ynrhsdhy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3zukpqciq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3xdxyjmhc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iunqmipl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wyyuhvck.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3dnseygzq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3qmyyvfek.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qzoubeii.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dqwknahx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfnvlsad.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3vcrkzwxb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ekmazxnl.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ljewigch.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3cckwsliu.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3xzuekzvv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3fdsfwnij.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wesbfhdw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xmaditxo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3kxrxjhrs.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3brbfdkvw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3juumkyzb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3xozoxaej.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3osykihkp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ntxzjpim.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3hcscista.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3obkztzwm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qgyjoqqs.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ypqlvdof.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wavhnrzg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mxgntmfe.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ejdtscub.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qhfmwfat.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3oqtkucqp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vhqwopes.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3zkaxrahk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3oukklwhi.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3cjboctis.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3alakovgr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ogpotkiy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ehfmcxxs.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mgxodyyk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3smgvgsvk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3hwmwzaxj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gfzjksas.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3vokkxvrj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kcsigxcl.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3wnefaflq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3gyjindnl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3wceaidds.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3jqglxwwt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3pyylkxsg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3fwffgesu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3xlehzjtb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3pusicvvt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3eoobqbuz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dajjpplj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3wlrqqemt.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3jlhgnyza.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3opmdnoah.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3wuaoufdb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dcdgiosa.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3unnmsacu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3bhwhakjc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3jlrxlgok.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3nkxfkhue.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3dboxhiso.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3wrswuutm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3oajymlma.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3txirxxpy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3tnnzuvcn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3dczjddxd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ideptfwm.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3bnwnvatu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ewgkdkcd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3dfogcqcn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zzhprqre.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3hqriykib.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3avqwuiyl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ifsmajqz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hpwrzffy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3rguiifaw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3lccqqyhc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3iacctxno.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3puedimxo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ichrxdjm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3rnovjuvc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cpzgbywe.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3oegfqjgt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3fxlafboo.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gmfpmyca.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3hcolswxy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ijzaozib.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3mbhlvnhq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3asjchkkp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3pdhevxep.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3wdwevhjq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3rbirreot.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3touoblbn.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xdnmovsu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3dxphmysu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lyzzvvra.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3sowbkbah.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ymveiixa.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rdxeuteu.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3obzdcvan.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3isjemqkn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3wrqfyebd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ngxoquoj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3iifvcqci.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3zucmbkhd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3juzlkjod.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3pwagbaex.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3sxpizwoc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3aexxrihm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3bxeikhqc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3butqzjti.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3qgicwuap.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3fhgbgdvn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3sjiupqwm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3xnvyatgv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vsgboahf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3iqhapihf.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3xykzmjqk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3uxdbqlet.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qiwinphk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ajuvsiuf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jpvmxupk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3busamruv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fpibueln.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ixzbfjwh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ilwriqpf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3btdhhmxn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3rehiznti.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3vjewrttv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cfjtqrxy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fufnunub.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ztpiikyl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nnqstuin.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3omfuvqqc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vilpthfw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3bdvgnqhx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nzjcgaec.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zkgfryom.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kxhbvzue.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ivccudsx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jptpmctm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3yqjonrxc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zigoexms.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3rdochjcd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ltbxjnxf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3aklyxlqc.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3sorlpoqh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3wpvfievq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ixzkcwdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aeqhopha.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3qhorvuqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nccfotfo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3okxtgpvq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vbbmdhdv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3tjbfdacd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fakxriky.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3dqlmyzmu.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3yejhraoy.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3kadvcbng.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ehbibxcj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ldxyipeo.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ghbqjnap.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3zxbquwsw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3oxhqwimw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3obasrooc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3vjywodoh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3nyyfclje.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3dibgdxyg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gdxijfil.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3kgxgiask.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ikvrwjqg.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3fqjapmhx.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3siggnfoy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3txrtksta.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fkrojuzo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kpobgsye.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jycvomvu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3wknocjtk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3olshytrv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lumhypez.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hpcuadmj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wuyvxawr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3merfhpev.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yakzzjfs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vddwyzjv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3efqjdnlg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vitovxim.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ugcwxnzq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sxawhnau.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3jsglxxjc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3hxmoeiae.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ffcchrla.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3myteonig.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3yvsznkjb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xcpuagqw.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ubincxks.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vhhkemhk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3dxyhgwjr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tmsyfnua.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3kbrnyltx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3lspclwqu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3uagcajja.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3xaloappa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3arquhkeb.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3nnvpniwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akjzesuo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3xoebqobg.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3mcqzgavp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrqwjukm.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3zevvwynw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3bbzzmjbo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3mcpbcgwc.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3tatkdlcu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3nbsotser.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3rcpyibtd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3mrchwbws.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3frtvjkgf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3fkylvaxx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3dhshvdsd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3voklxhpb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3eocglzcl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3gxgzmtlw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ywigwbqk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3usuqhxnb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3xjqzhngd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3agbuuevz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jercgwbq.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3roywdrcj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3rqtdtauz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3doknzcye.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3xylaibld.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3buktnpvi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nigusezo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gscaimiz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pxojbmns.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3lqolgvqh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3coufywfe.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3giuhadxc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mxuqbbtv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3rlrhtosy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eeljbonl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yruurtaz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nbkkruxz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bolkydvx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ogallwra.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3olxaweio.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jnhjivbc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xvidufwo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pjbctqvo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pbserwvd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3jzexmwhc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xmbzgekf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rgfyvbzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnwwenqa.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3wzqoctxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnlefrme.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3anmbztwk.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3vmusodxk.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3rwuxtehp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zbcpzyil.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qaurhzyk.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3elodyprj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3iupcyksz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3iplmbimf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mthvjifx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3pvyrbsja.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ucidrdny.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ejljxjig.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3syrzljyd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3zvexeyii.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rfktnbbm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3yezgcvqw.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3ouijlxpn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3frwzlgei.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3hjjciisq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3svbvgssm.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jehxgiml.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ljclntft.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cifqgjxk.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vfagivfh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3mcdutcyx.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3mcminzhp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rhtzgfiv.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3snrjulur.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3bwncxoub.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3vrneqgrv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ktdwtwbu.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3taphxmpq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3segmxyea.html


<!-- 参考信息 -->