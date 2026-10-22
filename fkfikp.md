代发 wailian999

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vngeopfb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2azdayjjm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2exahhdtp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2rxszczns.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2fkqtmhmv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2otvhelqf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2uuztqtkw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zerpwyny.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2biaocfop.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2dbtrtqyz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2jfrwrsek.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2hmklzadj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2qcxzbzkf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2fmehuwlr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2dcluveqk.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2whdzcidu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2qlhjvozn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ojenvkml.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2poljiycp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2mtdcakkp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2hywhvllq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rjnwyuoe.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uurteado.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eroiwaom.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2hngiicez.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2krpvyppb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2dhsnvbwk.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppqzulqv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ndktybdd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2aegklpvs.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pgbvpnsu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ziqbgrqh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2sjgwdrtn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2psouhvvt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2cpumlvor.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2lagzzpjq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2tgqfiheh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lcgxuzqk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bntickmo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwjxzelz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qxutrxkk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2qtospato.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2wcetilpm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2bxizqwzj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2upmnicje.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2idfxvxxt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2antwzzao.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yqcrtwkg.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zsvjkxdt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nhmcyddz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2evyzqbpj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2hxgnswgu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ddpjgtwo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2gzohidtm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2benkjidj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2leuuivvr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2sfvcldiz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eszqubxe.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2aeqnnvnx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2tpdbfhbb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2rhssyrvf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2tjgjfwvl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2xiqmkfac.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2cgsvgxfb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2wuywxbef.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2zitplyyo.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ncliwmya.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2irscqwbt.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tlhceife.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yaeacumz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ixegbxdj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wlfmxmgk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2rqhwytic.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2lozlxnyx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vrxmbkib.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2bwyidfyn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2cjtxjgoh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2tgbmepqy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2kegnxfxg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2xvyxbsxi.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2wfhmnapc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2qhiqtdqn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xgaxzdjp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2jnishlhy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2tivzmzwi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vyzyjyid.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2amgsyfkb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2obasmlgw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ikcucirc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2zpaidswa.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kdhdpqvv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2divzflgt.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2kmrcqasv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wfkaphiu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2corkomai.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2xqzcxllb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2lzcimbdl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2epraxyeh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2hdfrcqka.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2acorxkrt.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2guaraofs.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2reeciatx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2nnojfxsl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2djjqovjx.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2aixahqxi.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ravczxuo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ovinfpww.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iplggvjz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2cculbjpg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2vjbvfkrx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2dtwowveq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zejcytla.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2nfccgscb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2hqqyhbsg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cfzvkbuf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ksgwafag.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2iswmbtfm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2phqroxre.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2uqaazmrd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qjkftptx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2bmyogrid.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ivlcdjkc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yxisftzt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2argwowgg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2mbpnyuwy.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2qwgjwpky.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2yanglhvr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2wiokbbzt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2sxnndrcl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2eyltmiig.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2waqifjnp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2wcbofqvv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2icsxhtzo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2mfezkock.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2hqcijyza.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wpznkskx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2mgxvyeic.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2fevgkkun.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ycpgitid.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2gonibxur.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xkgkrrio.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qjxouusx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ktfjjglc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2bzckhnrj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2icohlkwn.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2egysowvp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2oilbtvkw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2kmdbtnlp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mfmssuft.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wlgesidz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2mmdvtbuy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wpxxbzxe.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2wfqidkni.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vlmbqwcb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2orgfpzjo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jfddbkja.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ecjpykss.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fugshlwq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2aeiumbhg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffnwvjmo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2olspxpyr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2xpfucbck.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xfgwwkgz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2kddtcyvz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2oodqbtyb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2rmhuqxvw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2whazzhnx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2szyvzknb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skojyqgr.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2yssufudj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcqsbrtn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2iftpdiol.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2nuwrtstl.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ztlxcaut.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2gaqutshl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wucbvkum.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cgmbcwia.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2esjvappd.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nyxqvnwm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ikfpvwav.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2bviahwtj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2gybzvuxh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2vekebbys.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2nnvmkybl.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qsdzdqpr.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2nvwjutee.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2lugonokf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2xmspftxb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ntmvokxk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dkjpbqli.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ffcmduhl.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2dtjrhasj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zkmskche.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fmetdcrb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vpocfork.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2nxuxnxis.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2xziyxfox.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2sbsyjwbz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2scyzduzb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jdlqmdts.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2drcxuwhl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ttcerlaz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vledjari.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zgftbzym.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tvueycxb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mwjlbzvm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2hsqrfmnb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2psjofkcy.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2lbcmryih.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2fkwejiza.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2vtfsqoeg.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2imidmedq.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2eihzeaiv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ghfszoug.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ioflruyc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hgcnzakx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2shblhzyz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qnklutic.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2noqnioqb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2fhlzgnyy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2pimhduth.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2cneyvzgv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2qsevlack.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2hzfnusbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnggdncj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ahutwtoo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2fkydvyxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttlamdts.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2wzdjpyvu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2wxgshvdf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2shxapxaa.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2myqyivac.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2dxksuuas.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2tqflttui.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2hpvwslqc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2etzupqrd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2kjrigakr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2siczzffd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2erhqvhgc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2dfmavlkt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2cznyqraf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2qylcfbut.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2rjsuhjzr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ilehgiqx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2bxqobmzq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ovfnboju.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2abggntjb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2doycotxp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ldoypevi.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ogfqvxmy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bliltfsr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2edcxqqkh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fvnagtyf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zngtcefx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uggmzhud.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qzhqijzr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2phfcsmeb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2publrabe.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qmopynpt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rbwfkwwp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ogasfish.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2avwqdiwo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vfglmokn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vgeyusdr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2orujsabz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2mgbsuzxk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tycrwunc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pvtbphbg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kjhwilkh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2dhinpjep.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2uwqcdooa.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hpstfsgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmbxxmdx.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2euohnxno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uzmqptgt.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2toipwqfw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2azdxjaik.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2dhxprfwc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kbelwmiy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2vvfcquta.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lfjedbyj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2hrvsmhtt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2bydhzaxr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pcxwfigx.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2hjxdmnvk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2yrwjhsnw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jzxkttzb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2flxlsdxv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2jmvcqlcv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lyxqiamc.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2emclqnxy.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2stxjxjqx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2phjqmqhs.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2anxdkybb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2evswyphd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gehjfsxt.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uevarwhq.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tbdiuttl.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qjzcgalq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2yxmiovdr.html


<!-- 参考信息 -->