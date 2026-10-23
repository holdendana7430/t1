代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3nsbtpbrw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3iauoltjf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ekrvfoyn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ldytesbw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gtwxzvbb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3vqecyorg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fwhcoedo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ujctnebh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3vjtbytzy.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3iukolezs.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3kmbaapbx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3spzyfgof.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3xcmirpga.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eziuvatt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ekenxjte.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3eccnkgww.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3cvavkvuc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3kvibsged.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3rbvlfmpk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zrwfkisk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3tyjsjgdj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3virvrbax.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3iyowaeuv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3llfpmfvc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3etbeaihs.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3izqjamso.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vuflpsys.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bgjusjvx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3fniywlay.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qwahfvqe.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3swmwhdhu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xluugjwp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gaimjdau.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jzpucvfe.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3mpeloptd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmgzocbh.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3umdrrhzw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3qhnvyhvz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ancgrzob.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3truywvyj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3dgircxue.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gkuicpcf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3eprgkqmx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3mmlvmyow.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3chwaqxfn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3oubrfvkb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jaopmmkd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3hhvyhhyg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3egrkcudb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3tvpeyucx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3iiornxsy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3mvywqxju.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3gjfsiyry.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dbmyrtvl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3vjoquiku.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3nezintvw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3lnyolrqw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3txxitdnj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3nlflanfi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3vsypbbix.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3odmdcers.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3vsavfcxd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ygjyuggz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3nsybqshq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ipfkkxvm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jvcmyfby.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3jywcweub.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3txkgycdx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zsyentgv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3whxkflcm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fbayfxwk.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3tasbgwtk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3yoxclrev.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ywdmrdgi.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3mvdramis.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ijeuzuur.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3bkmzazqu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3jvyaowoy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xvszusui.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3kofjeccz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ndjcuvre.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3txmikjnn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3qpbzfrhm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dfelfeml.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gnhnjvke.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ubtinbln.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3fbakhqwu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ytncwvrr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3sbnqjpck.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nwtfsqxh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3qzkajlay.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3yqhfcvsb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3cjttyolr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3uefioroa.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3qqtcssno.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xlmbeobm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3xazjgdbx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3xixsvrkj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3quxrptvi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3lhcmqdmu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3hhohpgyq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rbwmblsx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3vqijufie.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ymhtmanj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3paytjuxn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3iiqlrshr.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ndlyywmc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3aveyaubc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3hhqumbto.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3oevojtlz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hrmxeepy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jyplpshs.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ahyacupt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yexhhxzt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3oyslggtq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnlarqbg.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3zxuuirno.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nbvdtbgd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dpfzplnj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qoifqttn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3imzllnsd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3arqemujt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3tblizdbn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3vmjqotij.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3qeotitzo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3gdmxhtby.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3thndllai.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3qrmwuxxe.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3uqtaynuq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3efaoezhu.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3kfqgankh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jlmzlhro.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3jelxflqj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ojttvsyp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3atnsphgz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3oveqgfej.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3agsmrnee.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ygtvtvin.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ircexxsc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3dhiknrjd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3hbxlxswj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kiooengm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3tiqqrqwx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3mphodmgk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rwabrnxz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3maeulfbg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3dexkrwyp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uwiipykq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3phibvwyx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lnsxrlff.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3hpvmcwpe.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zgmdbswj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ksoxmhrj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sesjfvkn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ygkumxkn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqfyjsgs.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hqqahmnq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ffavfeed.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3otraxdzd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3aojsmhqu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3pkwjsnpi.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3rdrlngig.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3iihafvtk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3gclsywhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzkuqjkw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3slpffyob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkuoqkci.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mjxdjcty.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3pzsdbxjs.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3czbwjiik.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3vkqbytdx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3azfsqdrd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zceqaeti.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fqdkeade.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3oobwuwmw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3byuqdgpj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3elhvnaeg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3wmgxjebc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3slbmdqgg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3txbgglta.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3aencezns.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3amhfsctx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3xidszlyr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3iklqoyvv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3atkzkfcx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nozsuneo.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3atbxikgz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3rcyhkctc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3nzxipylf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3thnbutyo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kqvcxtis.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wgrkkiar.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3djizhfvd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gsfzkund.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3efgwhyrq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pducfhwm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hehukaik.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3xyhvalvw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3whnefaho.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fkktazbk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sixznbva.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xheeedch.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3trxgpbro.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qktrliwr.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ebifyrqc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3tztmksld.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gnmjnkur.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3hddrposw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3tklowdma.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bhrcfqqd.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3wqqdomrc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3laxcsbus.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ezgahowk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gkabmqmq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3guroubof.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3cysczgkr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3oxwjabej.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3jnzihzrw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3cmjbbhql.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3rspktvzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irebkpmr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3skeqldgl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3qdormwvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zeynzxvh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ydfgdllf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3oenswfxc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3purxnuzc.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3trgabiut.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3qobwowpz.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3xpblybra.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3lptgiveq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3xyqhrthu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3klvgmnnm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3jrlstabv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3yudcjqyf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3szilnoaa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3fizlfjvn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3pvelmsyv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3zernykcm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3qigfbomy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3bvesgiyz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3juwempag.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3dtobtvrx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3xfxiupna.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ipkahxpz.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3rvljotgz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uparlhjd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3nhvxxkkz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xfdvjyud.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3oqegojzc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3gsxddkij.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tmegxzty.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3njdgrbvc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qdqfcvfk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wasebkmx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3whjdryaq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mtsklxhg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gonitagu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fmrjjkhf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cmliwlha.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3lgvvymkf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fcxpdvms.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3afpdhasj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3xkqqaaha.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fqwyhrgs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rypcwzns.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3chmqstrz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hzoivvxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqabdewo.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3qmmsejmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lredcifa.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3oegbczbb.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3lfldzkea.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3lgywexqf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3esrzypcx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3hnlehljm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3didbwlot.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3hxvpermx.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3pmjpcxyy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vzlgwsib.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3athfembs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3cpguqxor.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mnzsgplu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3omfgsoqn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3piedmkvl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3todaldnm.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3rgytujdz.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3mwjlaucj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fiosfprt.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3mqbvtvwn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3aindobsp.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3unqlmhyg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dnrqvhyf.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gnxnhrxy.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aiqzxdlm.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3lzlmagtc.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mimhowxm.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ymsocvih.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bgcnxnor.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3zktftwip.html


<!-- 参考信息 -->