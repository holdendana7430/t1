代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3pycfjxrc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qpmesfqg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3fqhlneum.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3cuvaaajn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hbxeooda.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3frdkemdv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3atkbozdf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3xlqgpbqa.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3vcarkwgf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3eregpeqx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qhwqjicn.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofmahrnk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3phjndznb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ktznhydk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vktnnixt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xsnmsjcm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3inzpcogt.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3lsdjuvgu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ffvscejj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3revlxnkk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3vkbwmfzc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tqhqmbvp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3bkxbmpdo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nizcbqtd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yrytetti.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3vsfybxpk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3nnczjbwy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3djocuwgy.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3appcvdwp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lqwfsgmr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ucuwkfyt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3edahrkdn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jccepwxj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ilunpzyg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ifqlnhgw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3irxcfkbj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3vroiskyx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3yzqmnkeu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3eabdzcek.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3czkkhzkm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3vwveypxw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dzyxprsp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3qjgzkrwg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3bbygqpwf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3nbgzihua.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3dilzdhpk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3fvlbodps.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3gpyxsjia.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3anaoeikd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3hjtpvquj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3burstizf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3eznfdiad.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wiyuyuao.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dfjuecuw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3xbvckesc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3alubdaqs.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3prbtjyxz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3dozbaslf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3laxfsenl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3caghccvg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3prpvaydn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3xwfwvhbl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3mlwdhhor.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3fojekbwl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3kxwpwydk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3npgqhxdh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kyrobyxs.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ezyklhvl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3irrsvyhy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3nehpiyya.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3fgovgjht.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3nqdximcz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3juimutcs.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ojmlnltb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3xiwzkmvc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3mjnmgpcl.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3sicuqykp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xxpotlfi.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3jktkigxu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3nkvshzkl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3fjuoiohe.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3cuetblyw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3wxwhoefk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3kzzbsqgr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3hiozfcgv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3qcxtacgm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3pcgaldjr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3vfeestzs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3yumvvawx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ccuxcjkj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mkgsjpxf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cnpghvbd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3arqvjweq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3csmxbzwe.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rccmwapv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eibvufhf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lgctfdla.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3fnbccbky.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3izswfcvp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3axvzfepy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3pcnzswfg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jidgxcwf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ivbqixrz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwvtqqre.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ejoithaj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3msizwatf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3apihvtty.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3dhwlakhi.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3iwjzozdp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3laigqzwy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ntgtcjuh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zkblbnot.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3lybbxdtf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3huvuphco.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ajscjavn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3weiqlray.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3gbtlejmx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3lgkynqtt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3bvsyhfcu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pjxyeqls.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ejapixrc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3makxkcks.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mvizopma.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3lcrhtoht.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3shfsrzye.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mmwemgzk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3uggwgzki.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3cnwdhzas.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3lxuqydic.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3krkhgimx.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hacogweg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3llcocrsa.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3rqsdelao.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ewdamhnj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3mjnzinqd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iqswuqcq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3rzrgrltd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hcmcdenf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3tmvgydau.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3drtetutd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hzuiheem.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lpkobncb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3bacaqbxm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxzpebrk.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3uccvltxc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xmkhndwp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ifquxeml.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3bqturpyw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3wcvlqslq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bfdojjtu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3anleayji.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3zrvvoeqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkruzvvg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3obvqcsos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qcpzhvto.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3iewjuoxb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3qbzrtskt.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3igfjeswx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3audzbwgw.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pbggjsab.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3orhbvpop.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jpbmwsds.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ncwirjur.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3erkuzaxf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3dnybqudl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3fiuxndnd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3kkzqqzji.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3zodgnmxp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tojsjojm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gtasxmdz.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ulfpqkjj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ylxhwldf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3dgufkupr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3denyudop.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3iwqhfzyt.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3kpattcsc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3llgibvla.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3uvuugizw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3puklztuj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hqgxluxw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3nfopzwtw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3caazwdnt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ufdczjdx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bgoxkviy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cusainax.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3oweomaoc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yyqjgtzu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3asfvlveq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sljxzrth.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fsjjtwrv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3lpclghks.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ibldbpik.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3myrllcar.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3qnljirks.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3dfuiuoxi.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3dayajxte.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3hjdhigqw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ipylimfi.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ltlnrllb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cyyjeldg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3vxzsrcqu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wtpjrkxu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3sgjhtswg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ahjtigya.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3afepbdmi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ywwjimbs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3qsjpjklw.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ambwvcjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ozwvdhfw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3visaiqny.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3bvkmrgjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uofewndr.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3xucxfrnv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3cozxsyxg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3avamcbjg.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3yimvcbth.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ntfklpen.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3bmhzrfls.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3yumvycom.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3jfsmhapk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3qcbkxsws.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3taxzelka.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3wckdbzna.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3uhfjqdqm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3dxbuzrtg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3irnwissk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3nsqjrljw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3qycmthdo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3hfvocydu.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3pfyjuxac.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3pimpvyql.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3vqjxipmf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gndajpdx.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3arkiwxzi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ctwmgzkt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dnxektgv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sycixzlj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3secuowrh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3stsfhrgj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3erlrzmzd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ullxetjq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3uinpbocj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ossgfkpm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wzeajefc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mpapppvm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3voafwafs.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jyzqwwlx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vzvhxfzb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ipxydfqw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jcmzegvb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lnmwylrb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ecygykcl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wxmxegwx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3nmgpueud.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3rbqddbmm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dcmykidp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dilkdagi.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3sqaexbic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dyfzwbvk.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3tyzucfpz.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3iikhvlrb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3khbqsphp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jpcutbvg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3bxfmzsuz.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3omlwbyoa.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3miliapxc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3yfawahon.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zyuvqoty.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3pawhlfar.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3cfeoawup.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pgjdhaiy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lnjecwnc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3yulquwwk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ygdnbear.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3sohmtxpj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3iizxdopp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bksqqavg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3duqgmgxa.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3eqtjdase.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qbmhboih.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yaopykuo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ojanwwch.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3inftfdqf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3rqcxkpur.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3uxfmbbce.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jxexopax.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3rlmpgwll.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3tohwatuj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzfvarey.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3funklkkw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3hwfukoij.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ntmrgbet.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3gytqmnzu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3nuyuklnp.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ivjaqlky.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3vzknbied.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ckxjbbdm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hskhpnlu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hireyksb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sryrmarx.html


<!-- 参考信息 -->