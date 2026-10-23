代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3rmwyjllv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3hmkadamk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fmshlhbd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3bjgzswjq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fveebpnf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3nsykvpzf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3okpqbqmi.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ybevchyw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3mdoderfy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfwltydv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3eulsumaf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3grnvklba.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3lbomwbfu.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3tppidoxz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fdkwxhpz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3moxsojkk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3uhkkospy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3quhhtdfu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3daytvfto.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqhergal.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3oeuvjunt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3wgqbarcb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ztsbiogo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xrfnheft.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qfdmhzhz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3tnoasyaf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xihvshxz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3locmkrre.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3otaynrti.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vfkrdyjb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3jtofzpjq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3irohkoth.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ethpnoth.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3yqhlypru.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xbatgoje.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wvhnrcdd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3dumiuqrp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vmfuhneh.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3oqhluhyi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3jpzvqyyc.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3xmdygygv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ilyezbsv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3hqvwqkzz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3pjhpqvhe.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nlbgszpy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mvqnnopw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3adetosgv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3egmejcdw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3dookpway.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3knmrmgqu.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3vnqykstn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3tuwazgzu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3bqrdlken.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ffhtwstb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ksbytqve.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3flfrgdfe.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3qdemfvxy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3yljfndpg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3bemgjpnm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3bgamfnwm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wngnuzhj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3llzwxdud.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3zraoycap.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3qvsopcdt.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zwejuczm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3divtrvhf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3enddbgbr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ndfmcrqp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3nazhwlhe.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3eqgkppsw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3dgofpmqj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3qosziowd.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ppodlxvp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rbtxiask.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dzeqhgri.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ggpnwypl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3twehxrkq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3iullgcat.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3pdycakor.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3jtmqetmn.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3geyvukob.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ztdltttd.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3sjopezdm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3skmnbfsg.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3sqotgphj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3momhvdek.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3qyuoxxak.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3pzvtssqg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3egrmjycb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3myggwayx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3clvtepis.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3konbmqzb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qmyrfush.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3unhmpxgm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3repltbhj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3rjhqttbk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3zwtzljkq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nivruihk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3aihmapnf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jyhencss.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3svmnavwa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3katryeta.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3clbjkbma.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bxbkglff.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3bzhuqijj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3focdsmxx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vmgembgm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3behklyig.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3xmucnkte.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qpooadbc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3yenuzlic.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tlxhpzxr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3jrdjgebr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3haccsbje.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kgpjjjeg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3scwbsfwd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3argvcbvn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ptgqkbmh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3rmjqoptu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3kkkfdsyj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rmdgzfry.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3yxpehrtx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3akxwtahn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3fcggymuu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3xrntwjfg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ljkiytip.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ipyaztbo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qmuibmpi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ylwuymbl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3tgvythvr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qxmdwbdh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3efckavia.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ewptokqh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ptmawmik.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3iylfphka.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xmqggsvq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3wncfzvzz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ydceiqdx.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3skpjfzmg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3qaxdaxhu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3bgeqayyc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bucudkdd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3niqlbpfd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sdukxdqa.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3caiawgjn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ycfqdokg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ctbryntj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tsllhdyz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cgorruya.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bommyxnf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3godpjdwp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3rpwabzft.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qbwpcffn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3aijzfygi.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3gorvkqbc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3wsdufajv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3zmnezuiy.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3aepwjwbw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3rkfljmdb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3waqkrtiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tuyvqccp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3fwxzlxwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czmwrinw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ybunkuwu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3iyuntyik.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3immycjyo.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3sjkdkbvl.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3urlwhfzo.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fqoztobz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pjwynyeb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3pgcfksxb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ceitlegw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3oazsvblg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3blsmknwe.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3hljjtblb.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3gqjeulje.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qvvyosvm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3svtbswhu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3cqazxxjv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3arxpykmv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3pcxmoyvt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3azfrhcmn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3vxnotkzh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3eserhxqh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3itecivcr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lluwjpgi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hnmimyhn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vijrdbjv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3pqbjafqe.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rzcencvk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bzfyqfsk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3nrosgmbs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mzdfjagf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3gkcxmlpa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3adhtwapx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pithzftd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mgbbwpwu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3mngdosbn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3pekghwto.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qaihskjz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ulguvtap.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3bnzwncri.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3vminmfrr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3mqfnxgbt.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3qoxlivzt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mutggijs.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3kvzwllmo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3makhvjkq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3emalyeld.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oxdqokdo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3lohixwtx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3esumulhb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ofmjvaev.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3fkscobzh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3baimyuic.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3pwhxyvsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bngtaaxo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3rttgmsit.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3vowxiwex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tsqnqpth.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3vezyrebj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3oivnossa.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3dvxxwimr.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3dbxabget.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3wompevon.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3xdfgvguy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3iqypjlqt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3teuvqgna.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3twmowqza.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3dlqptmet.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ajidzrkd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3wlnkjubw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3gtbdesrd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3osugkppf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3dufbtxlp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3nmphymfp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3jskfydvf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3pjhxkcof.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3svqpvqeu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ylegyzgp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sbvuazil.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3wvqijxkb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qporzanm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3mzeajssm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cimwqsha.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dhwmagqr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pnotwxvf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dvblbaob.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vpzldury.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kdtqwqyb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gedtvnyb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jysocztr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vkdzlits.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fotaqdli.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cwfsmkrt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3scuzdynp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gnokrzlj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3lsoefsoo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fcjerwam.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3shayrrni.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rubygyfe.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lebscbvn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rfrukqxo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3kpsvffvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odinjmjd.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ndscyaui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtqddouq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3acanbqpp.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3jimffhyk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3xuolrjwt.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mrlttdcs.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3uwgzilzi.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vhswzhwg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3azbsyyya.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3bxeqqpkk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3djdcsdbo.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ltfobigp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3dwroqkpz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zzkkpcob.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zfmryesk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nyuvvyyg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jistfrfm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3amazozmn.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3knonmijm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dhubhpmi.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3feugqydk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3fjcjmtnw.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yngwmegu.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yxyukwjb.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dekpusyt.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3plepeijg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3lnnjotgc.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3pfbzlclm.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3feschlje.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3etcvdplr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3mnrmtzmt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3doynbxxi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3hgtxunfi.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rgwvlvxi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3neiggqnv.html


<!-- 参考信息 -->