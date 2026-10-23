代发 wailian999

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3chlmoebh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3tzzczxly.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3uqlelqmz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3gezofqhe.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3eehhwwaq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3rorvakac.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fulcctul.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kpzzxotf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3jtwdmuiy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3evlyvvlv.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3kjlgdkvd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vmkccgqx.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3htxzkbsh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3svrpvqzk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3dsmiztfk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vejswhnf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jtbuwozf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3gatgqtxb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3yhqokluf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3vyvfvazd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3zasyipus.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3eumxpjku.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bktkhlmh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ezmwonhc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jzzznhbh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wovdyaps.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3vwoqbstd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3dmeqdcwe.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3irlvjbhx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3covqgdxi.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3czrpzfoz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3svcmjzbt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3otnaqbwj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cgylsdwf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3tprhdkzy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3mfsbsxwp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3bwssnspk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3xlmngihk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3janmxvig.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3cehdvxtu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3xoqlilif.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3rkbbdyoi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3pjceofhg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3kwweqglm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mtooqxvk.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3knwdqteb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ntgzvpjd.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3tzuowuph.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hjdfhcvm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3rdlqigiy.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fbmoknrk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3fgxjkzge.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3myzgmolt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3raffdvfc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zwrhdybn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3kfvkmdgk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3gykjqqnh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3kmnbdtci.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ekctqnvx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3csajfdmb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3txqwkpko.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3iuocrzgw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3rxpfruok.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3mnrfheop.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3odfwtfks.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3erncfqja.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3deasrlnc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3rbopxmbr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3jkxugrzn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yrowxwtv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3wzlpomex.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3jqjpbrli.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3zytugckl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ezclwxhn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3trustnqo.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3jpdrzvpm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3iideomgt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3tfvvrepv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3uxgmdeqv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3rcnmbohj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ncuilrsi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cblcxeme.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3pcqtbmyp.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zjhaqezr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3htylzwbe.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3mmxabxmw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tpxrthee.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3nclucggo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3txunjxgi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qhoflusc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3twcstwyl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gtelngsn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3gufrwrus.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3iitafjzd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3yfhgxsio.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrqqxeqm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3wxwhazyc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3imbbnums.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xvhmcsht.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hwcxlujg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3hiltrobr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ptcwfneu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tclrbgmy.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zqftcslp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3eftkbrqw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3volgdqbf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3wykgmwwx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3bwbhpicj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3wfytbtgw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3bucjvsms.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ogszmjqd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hsvlmztu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3aivtreil.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3npiaifwz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nrzhlxst.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3vtmspkoi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3prvfybqc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3eoxuyouw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3toenurzy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3opndowry.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ynjoikrz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dedxhykb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3jbcrfkpz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3xxkjjyhk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vllwksmf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qiwptdry.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3foyjbyci.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sadbzoln.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ofrctgcl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dconueir.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3lvmjxisf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tskpzjub.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3acvhezys.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bryixeie.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3vxojwpha.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdujrxrz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vammmpzw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3qqbwmqbn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3uxfnkzop.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3bwtyyphq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3vydueouc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3gitvanrt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3bfxqyrhr.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ailnllgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejoktakx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3hsyzhfnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwgvmmld.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ggsetops.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ipjquncr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3msfuxtpc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3kutkdrfy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3puecycmj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3atwbvvcu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3adtqiyst.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vpxxpafc.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rofexegp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3qraundpp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3mefeevkm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3tzetqqxe.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3nwvqbfpp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3wolylkvp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3aracatod.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ulbsmnea.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ocdhedtx.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ouaolkro.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zzdakqep.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3wahlgkiq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3dgubnvia.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3yrprepfw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hffveqdh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dhrkuvmu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3nktuzgbd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3bhtreopz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3cqaywggx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3betteobf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bfxdjbcr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rdfwnimy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ojjmgvie.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xfcnvdbi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yiobthfi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bzluhlva.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3qtwwtbhi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3whfkazzo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qtfaakms.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3smhefyxn.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3aqcdqacm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zoayphme.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ucrafymk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3gwbhaqin.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xcmpkbbe.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3klgwbcqz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qmextwee.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ywwzlhpl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jgbvbkdx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3zwfktzyd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3fnvqrutq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3tpjasuni.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3kazfwbzw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3blvkinnk.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3mcbhxbjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhbjyvar.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3sdxjfjld.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3bvsxnyre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilsiztny.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3uljvvosm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3hnshbgxu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3fatmxqcx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3xwkrjyhj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ggkfhhsh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ezmgbazs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3eefkayxt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3suntzqpc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3cjnqjsaj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3dzjdyspa.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3hjhcwdwc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3kpsnfvcw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3qaulbcda.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3qzrepxkd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ntohkuqc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3sdogpmiu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3kbgapdvq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jjhuclwu.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ybiveemg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3zorqyrbb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qefkhmlt.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ugqkovci.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hidmxdmt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kzjsqtlz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hgegerux.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3iptgbrcd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3luqpdpyg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yhdsdzza.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fnxxagaj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cxzwqhzo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vopezufy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vfxfwmtk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qugkcdwf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3twwjkhwd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3izxstuww.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3syjdlmjv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3syyxvedo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ajklbgxp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3idtoiuri.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3lmvizbzr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zgiuwjbu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bqcutnln.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3opgonqqx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dgsajhqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gronkgda.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3oxgdaicb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fppexseu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hgvhstxv.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3thgxzcsd.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3morcmxim.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ihnrnqqr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3cdonecjh.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3lphpsysv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3isxpkyay.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3bixjtaed.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cukisfki.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3gamwrzem.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3vgevmedi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mmxwyyfu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jgeyiszu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fvwnabcx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pfpopskd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3aakumymc.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3wxjuylls.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bovskwkt.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3zrlbqcyb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ncvdsphv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yimccuaz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bzxhxpvq.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wjkxdarh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qlgctqdn.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hguejlcg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3wiiqkrlr.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ibmjhdiv.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ieazvtdw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3tsbasner.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3rxmdggnd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3doqfdgtb.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3yekounlu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3oyoipjoz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3mjomspta.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3niqdskuu.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3yfuqblcq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3gozaoptf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3wyizwrgr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sfejxcec.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cqmimpwg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nyfgjgfl.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hbyzwqcv.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3decusbqq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uejmssvn.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kxonzomu.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vwmqtggh.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lpzlkceg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3skdqqnir.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3gcuwwrmx.html


<!-- 参考信息 -->