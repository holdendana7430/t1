代发 wailian999

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2xamgazal.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2pqzgjini.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xowsyimm.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rzgdcvsp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2czurjcyv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2zmcphvlz.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2tzougukv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2wflzynab.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2cozcgnpx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2bciyaucr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2xhlirdra.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kbwrkkvm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2lxgxjhnn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ucfeiqjy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ofrjulir.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2sehwxihw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ngsrywty.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2jinzvjdx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2xrcxbfyh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2clqaztmj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2msziwhvx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ujgrqmdu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ukgcdlbs.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ygwwtuml.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2tkskkzjq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2uxbwfwyo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gyoszxhd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2cawjtqkh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2jpqcgiav.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2rftxvgtk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2uwwztdwb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2sdozqqqy.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2dqisbcjo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2tcjxhsax.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2cooxizza.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2txwqpzfo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2zoldgvcp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2xpoeoarp.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2iflgcvie.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2mgmazatf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hriqnwpf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rfqbkwsz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2sxqelroj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfxjuczo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lhhkbzsg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ooviqjra.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qregvzuq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2isfhhoxq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2tobowhcg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xxhwkjxd.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2kjkfnndj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2kukctxii.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2adfsvzzh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ckwfarze.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2lxubowgk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2pwhahkld.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qcxauusw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2cqxdsjwx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zfrswijz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ugzwyyur.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2vjlqamfi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ywzckbvw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2lmafrltl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2zsxjttcv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2velnlobu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2zzynheid.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2eqfdhwmw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2tumrazqo.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xjvzrlsf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2xgrbeusw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2nlmzicjp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2pqoqzlsh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vgiexjxg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2kpuxwpyv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2gugwdqel.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2tlhgjdeh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2uolmbrru.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2arlvqqza.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2byhgwypx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2lbabqbfw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2lrjhonad.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2pwfcxjag.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2blussymq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2rbvmqvpq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2pbaneegb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2cccibfii.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xomnbqqh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2fqyogpxi.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jgtzvefz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2czraupkr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2iikbpzii.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2kqfxtmvl.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2xevmfoli.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2qumabhas.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ufoulhnx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ppqhecda.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2xarmzzqi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tmfwtxzr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2hzykrqyg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2izhxbrac.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ugpdzqcl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2mindnvym.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2bptfnlbu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2nnekyipk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gpiibjuf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2orxzxppj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2zpplofas.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2yxoladgq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2tgwfrmpg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2okhkipez.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2nmjggzcd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iogxlrlr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lpifycan.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ldtenicu.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gvurvcmw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jydvhtps.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jxuggmyy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2xptipmto.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vdnqijod.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pbvzywwk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2mjwzsmow.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ivfeziwj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2uwikjxnh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yirbjiah.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2hcpamwlu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yzelxkwn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2buupjfrr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ixyddexn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ujnhejyl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2yqmovdqx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2kxnrvtol.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2kokjuuhf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2rvtqoiyx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2njnxnrno.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2mxfpnhxg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2dztpavfq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2hccxnmwp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2jnbfcidu.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2yvjkiqno.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mzkstmnx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qhtwqcjx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bpgatdmd.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mfcujwaq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2vfeobxsa.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ieigymqw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dedrlruq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2cmzjesml.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2bmwbrbfe.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2qavwsyhi.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ikudvbbk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2amkwdkbk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2iasevyok.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2idypxrqj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2kqbgrduc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2mfvbpnjg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lncwmmnw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2xdijvgid.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gdqkdcfx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2msybfdjn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bsipjipg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mlssckbw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rnbsvhij.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ifzngzpe.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vljgyxik.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fybbytgs.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2tgqpqguk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2iqqrxvcz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2iooxoxal.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2gjoqvwls.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2gqfxlvlq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2pvihpmwo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2bmkrpqbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlckoyvl.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2kurqzuxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjtdrxla.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xlndzebr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2rqrbcnhc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2rojumilk.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jgxltphx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wgktchfc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ztbzwnjd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jesrpbmp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yoizbgde.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mvydyizx.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ngmkhlbc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2alwhpdei.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2rqijjbhj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2feczwgjy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2zozokplz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2xfvinlnp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2bbhcjphk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2aydwyiab.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ejbzpoeq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aqbnnpqf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cizwlzjr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2pfserrjq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2twcxngov.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pngggoih.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2opdmhpwa.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2aqfzvbrx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2voydgchh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ihcvakmj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2duuuajej.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fbmczzob.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gluzvdcc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mzlrdght.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dbqpdpdj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2inuxzams.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cjapdxbo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2cljqtddu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2rcwrgrxh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qiiatwfv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2wdmycphc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2qzmnpmcd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2zqszlccw.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kpfavfyp.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ihsznntq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zgbbdsda.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2jmblaceo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tiithvgf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ncexbfwk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qzsjjqqr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2suabsnzk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2vnlwsbmk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2vodenoxk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2hcmxrqlu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2rstnrcfy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2jcanhueg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqnxeydb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2irkyftrk.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2jwuuqhgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvwurkuy.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ojlmxvva.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2jdhwrjni.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2pexgtebw.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2srvgtufu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2yftnfoli.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2gjsdkadi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2kpzaviuh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2efpzqgta.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2xdvqfelo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2cxhlwgcl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ptrpwyem.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2jlyxenba.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2txktyuid.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2zrfkqjkd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2rviczggo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ecnngpiw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2viynrfnl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2gfznjdfq.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2cbpounon.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2wqpzqvea.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wjqozpkz.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2tkdkjtdb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iaiyxxsn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pazeqnlt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ecmvcdvn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dvvlyujw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ihyuxnjj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2waytnshq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2mkpslnvw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mvqlvoqf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lhawxeqx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ehpzxels.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ocwdsnoi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ewakschi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jopdokjh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qxoebfei.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vuhkziir.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2reiwepcs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kzglxmlf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2wdswqeoa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mheajzfb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2cesrovtv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ugdrpkoa.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qefvkhwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efbfyred.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2membmwpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxnvszrj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fomulewp.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2wpoqpdyo.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2ojafqwpd.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gdpuaazv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2xsblcyde.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2poenhafd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2pjhvqzds.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2pxrqvlcn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2uxcevhqp.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2fenaehfc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2tttdcqsy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vujdkpeg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2txfmrfry.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2zhewaztu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2blzmtzgo.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2xjsoqjgc.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2baktfdch.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qllsyzfr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2rovxzsaf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2znoyxrcx.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2clvrjwns.html


<!-- 参考信息 -->