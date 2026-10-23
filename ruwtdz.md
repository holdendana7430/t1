代发 wailian999

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3okfilvaf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ahpudmgk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3vnrmtqti.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkrteaxj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3brzapszw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3gzcsszby.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mlvqcztf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jqweiddh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fuspjcfn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3djizsndf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3gtjsahra.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ddxbjsxg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3wpabspjm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nyurxzns.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3tmzunpic.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nwkkavya.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dslfflto.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3klzqvtkp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ragrhzet.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lkpauccf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3adwderyl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mqkclltz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3blmmsdym.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3reoorpvj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3wxzyjyck.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3gqsxzyud.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3iwkldenr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3lfrkunxs.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3aoaslyla.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ecvflqet.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mmkgzkss.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3srgukept.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ojbxjnec.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eopjhwxy.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3kfnrcnif.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3kwbmesvg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3hwzsdxom.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3uovypsan.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3yeeuqpzt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kssykpff.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3xnfldbib.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3kbpcqekm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3itftgscs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3erritmiy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3meepjklr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tzbsptkh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3lczyczba.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3jnxmrvxf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zvdzxsdi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3vgyunokl.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nublafnt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3nuswhmwm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3fkurrcwz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3mkxcuewn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3aykxtxud.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3yunbnczh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3phrqamry.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gvzylozl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nsizjjzi.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3hxjvppwi.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rpufwejd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ljptihox.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ulfcvfmc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3acflfpwx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3nnefbmuq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3trjldvuz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ufhlkehc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3vqvqfloh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ppprevks.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lrhiwyvo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3hdlenhgd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3hxzzztmj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3egwmgixq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3frwxpimx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3geqnaiei.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3uupwdzqn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uurqcgyg.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3bjuqiqgv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3eadbqkvu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3zkgtppxs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ofampgwa.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kocqpqbo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3unoqhiqi.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vvazdhhe.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3eyvtctsw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3fafeejmo.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3hiquvhbm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3relulxdi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3muaauffx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3wksgcsow.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kwkwtbol.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3dqiboecw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3kxwcryeo.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3cgbmezod.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ftytddst.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejklqqnj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mfajtymg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wvzunydb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3frjtgqan.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3hbynuook.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3tdwsflam.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3arhnbfwc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3okkrvvis.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3yhdbhlwb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3xpzqkljz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3zoqculio.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zhljmdhr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3vnudokkq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3vjjgtsyf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3jtlpehub.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3pehdrktq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hzsxodmr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3nmyiilsb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sqbkmrcz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aocimvek.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3dhowlvws.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vqvbxocs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nzpzgtim.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3rzrnauls.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3kvzpiuta.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3tegdgcrq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xwgyporn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3mjctqoli.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3tfhbcxgl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3uekmisrw.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3roepfuse.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3xmyqiqlo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3klseffos.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ezsgkxkd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3czllvddt.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3anqmvqjl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zuuymgyj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dssoenid.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kbrojpqn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3vmzpeycj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjhkwbar.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3uqjbvvvw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3hkbmphzm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3vkrppixw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3gxgzvnaf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3sbwondmd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3lmoynsqt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3nmuczapt.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3wrojxadg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yleuwuij.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3vpymfned.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3liupyprv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3vihrpxup.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3waiznspo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3hzrptluf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3rqrfuion.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3bjfascpg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vwartslf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lunbhcuu.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jwibnlcy.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3tnkdihtt.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3zipobybd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hlagpyhg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3miqsyhdk.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3mfyynpin.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ifrdvomu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fkueofzh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3bmhadlow.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ugqiagbu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ezhguvuf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nakferdc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3bnlnmwgv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3exkvtapp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3dbwmqxym.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fekkfpfn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pxkokdvn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jtqsysdg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3rvoyatkc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3orzoqzuw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cwasmssm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3lxplbtqu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nvxmxqoz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3lvsfaeos.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ihomscit.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lfeifvjc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3aqjevbse.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tskffcpe.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3srognzkg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fwoinqea.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3jqqfljfz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3skegrfxd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3oynsidef.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tqrdlnnb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3nmatbnpb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zexytixj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3tpapyjkq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rtbviboe.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3djijprtz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gczteeuu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3gpnubjhz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3yjkcryjn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3arpewzbs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3mgobtvnu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3bxlnviqp.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3uksvsdap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mghihxak.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3foumotkc.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3vuzzqvhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oeyanghs.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3kzaoyrad.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3yfdzxsgx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3kmhhfzdu.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3bhycyrsk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ybfepeaa.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ftuhikpj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3igixmfrd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3nqjidmcm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3cyfiyqlg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3xwpwwooi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3nvlglofm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ewmecbuz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3xqhoeayd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3xurkuobr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3smlhhgnn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3bmikdrdq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3gugwrehy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3mwyajuem.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3frtcfvqb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3pglurcph.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3melmpsyx.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3hhmnilfk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qvrwzbnu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xmcuabla.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ukcioovl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aeqxdvgy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ylakvguu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kenyfqku.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gtsstnfx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nbbrncqw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bhsdreib.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pasixtek.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qzzjqnlw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ocdrsajs.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tltybksg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hkggpdfj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mmkmqhur.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3nhzzcmnr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ehdotfzz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3uqyqrtsl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3rfclvmhg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ivycjncz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3afsjbxyv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3unhdwqsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kkrfiddq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3fchkpmdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxrhshge.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3gulxyewq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3jnlwqqhh.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3vlbkvtxt.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zgwvhgiw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3bxibkbdd.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hiubmhhw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ktvnebkj.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3wylddphm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xzpwrmak.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3wrrzybgu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ydrptquq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3oyjjjlyu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3whpigjol.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gcfooqaj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xvampflj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3phtzxduh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3wrfqqxhg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3smjvxirz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ceqeoztu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3tqgkqtxm.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ztgbhpfi.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mzpmsxqv.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wkudemws.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3llbqxmxq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vrfuejnj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3metumzhd.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3egsijgll.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3nbksybha.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3kkhvcbhr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cpbsfage.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3miwhrrpa.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3stntqiki.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3hppiohxz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3gmaqrryo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3werlsvcs.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3tjujowpe.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ojlcrznx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3oqwqwngj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wbgeydxg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3amhihfub.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zmhxrilj.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rmewyjqj.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oukzqsda.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3codabnqm.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3auxxtjhk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yhrkrugg.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3epytntzc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cjvqdbqz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3elofzfdp.html


<!-- 参考信息 -->