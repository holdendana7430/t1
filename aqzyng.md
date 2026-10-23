代发 wailian999

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3skvkaett.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3toeoivkj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fonajkpi.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ooxfdrqj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dlvaesof.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3qktaqfrx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3niafrbch.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3otmdceax.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hwfdtcis.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3tqqirdfg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3gtwihigq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gcvpadml.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3biahfbtz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3iwznomai.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3bkagwvjc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3mvarpdon.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3bjikhjhh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3votejwgv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3tkotnmtu.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3szgedtqo.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3uoqsdcsn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ciuvbcku.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3modijife.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3mendvyxl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3pkxfajhj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3yyjbdiku.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3vezyfraw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3taxbsljl.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3uwlqwdcl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3jgwlgmmy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3rsqipotd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3teubirxi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3amkxgobt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3dubjpmgg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3eslidmqn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yhpeacdb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zizyixec.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3nnqfuyns.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3krxyjxxn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3zdhequbh.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3riunkjiy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hyqltwwg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hpzyzkni.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ebvhqlke.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3saebysqn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3suzcxhyu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3zgmdbdgu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3uzsryeeg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ptlcxijt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qgvmrqkr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3qfzykfyn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mzyiuoiw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3tvoydkaa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3evtfzwxd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3eerbhdyi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3kvzyyfdo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nydydxfg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3rjstachy.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wtkufiak.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3kdvaryfp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3tedwqzxn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3okaecmwe.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3iipwyauq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3eibuqixt.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3lgdujtku.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3pnpngsvt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3bpwhtcrz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3clotxkyu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3illqlcae.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3bsvcimuy.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ulgouidc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3klbmextk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cprmkjsx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3szxwzliz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3dknjylvt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3jjqfhajc.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dwvibbry.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3njozfvmd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nnmhrujg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3nsyjdscx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3mbmqutmp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3tuxidjxz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3gxjgsoat.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3neczizic.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3qtokopeg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3iwknjrpc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jtlomzbw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3qsnwseio.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3kiqdqcxb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3dlpphnza.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3xakccibz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3bymkyetd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gyfalscn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ruxylimv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3gczqtedw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ggjkfbfm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3feipkeja.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kavvockl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3pupggagt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3dqpwewai.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ogabtwzi.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3dcslgkky.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3cuqjlzhf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3hqnsyprv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qsbwyugv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3bsvfwoti.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3rlnxxvpb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jpraowly.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3xcinboep.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zbwdumys.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3bujvsnby.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ftormzfd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cleagwdf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3umdrxyej.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wcnrrlkz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kkljvihc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iqvghyli.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ubadijlm.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pocexikz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hklqhuxa.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3hjyxbmdr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ptzqiqfb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ifmdpirj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywbritlr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3qccugsci.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3twytdshx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3gvnutjih.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3iuwuwdbl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3oqgkwqqf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3rpmnzqih.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3yaimwunx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wqohxjul.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3tlvvwfpd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3mvoytrqk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3roeunmkh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3iwvyfshm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3mleqlgfc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3tiunnvmq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3vuhdyqbx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iispbdmt.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ketlckep.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3cttammsp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pjrxmxmm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3aphtwlbg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pmwtrbal.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ummhwyld.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3mwomaiad.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3hqllclue.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3yebjponi.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jhgxoggk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3pveyvtxe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ljmowfmg.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uajrbyqa.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ktassevi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zhfuircw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sqcyhprf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3cishhloq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hlvxpago.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3acdxdree.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bfuythxy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zffqjwqz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tapshacr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3tjmwmjam.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3xetnuusg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ggmkskyx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3geearqlu.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3hnnbaltt.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3afpoavzh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3kubwqzpu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3kepjdmfl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3jejeylpj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3lblajhlw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hefacxxf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zgbdrfin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewzewwxr.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3wyaxhufy.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3hhejynww.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3gzkiktvt.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xejxketa.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3dtzvbjlm.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vxodpofq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3dgnkjiyy.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3baunisck.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ubftlrnx.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3qosgqkds.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3nzotvbyy.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3dqigpyvr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3lcwyqsly.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cfivhpmi.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3hwuszprz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3fvfatxel.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3cnbnolfh.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3zrnddqej.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jycfpchy.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3smnynjxw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3tnhqaung.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3pvuyhksd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lubaxwgn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xoritrhe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kkbajoht.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3qiozbvke.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zobjydsu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nmbpuovt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3erbwxkyh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fxroqegf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3frnjryqq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3letuotmc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dslxdscz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ltdzpgle.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jeidmcca.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3mefympen.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3riwvskxt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3gxluorur.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ysnvopan.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3qvchcepq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3sgebsalf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3mplmwzry.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3akyhjwja.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zitlxtzt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dvlwkrjy.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3gxorvmpa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nnhxjapf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3thgtvjxz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3udkmbovq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3aqqqhdie.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ctdmllet.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3oxsywzhp.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3kdsdwteb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajiqhsor.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3zscgdwpv.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3qnrlqhsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klczgyck.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3iixgmxga.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3drcrtdpw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3upglyfny.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3nsjiwete.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3audsaiwm.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3munadevh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3xdvdvquq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3tlhxqbsj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3dctymlki.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3kogsdbyg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3stllwisv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3nxpdbjyc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3xukrmhio.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3flpfpihp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3qfhqkygj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ggelhpmy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3bizdoyfa.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3awopkttg.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3jjmpkdsj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3snmbnvyg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eaxmkrvi.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3cdybhewr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qebvdhyb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qazdcrsn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wpuunypn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zinsqicx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3nxdsueyp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3gngwqixh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ylumecph.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ngedxbvb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wecbijkp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cvfgswlb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bygybucy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3steazbpt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bcbtpkny.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dpjrzzwl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jawpleep.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3srzmyxsx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kkwycdcv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3lgjbugsa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nvguwjyn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jroxmkus.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3drdgqkcl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sikiptdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zeeagare.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ymlcsfha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnzjjpgk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eumoyboi.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ppgqhlkh.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ssewpsyf.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fsxykuak.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ytxvnxpd.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3sxpwalok.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3btzchmog.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3qgkkveag.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jxispeow.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3scvzrube.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3iywdyywk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ahgmamja.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hnlrymbu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3cbwsfodf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vhlwmkcm.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3upzvzhrb.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3gzannxdz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kovwulyu.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3vuhbpiyi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3rgbxbeuf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mnjanrhg.html


<!-- 参考信息 -->