代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3aooasvbi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3zkhnwhkc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3xieslbbl.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3hsedwbxt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3uaqtvcqr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3oacxkbmk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3bzzufycl.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3kyrzfejx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3cbarmimw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3odanljsc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vgdygpfg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3mdmkifnz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3oyveiils.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3pqdzukff.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3cnjbktin.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3yqamzaqi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3mxyqrutf.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3bpufgmzy.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3eabvdqll.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uuvqokzk.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3znyuouxy.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3wtiapnao.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3fxvejlcf.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3rucrhovv.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vxuwffkh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bbtcvvwc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3byuypeay.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbgyzyav.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ftupxlvv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3sbcexaji.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3tgemtbig.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3feevugnc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mkakgevt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zapjmhwq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3yrmplvwv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3uhudnila.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3hutdsltz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3zxzypyqm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jwbxyffr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xxlwbwkd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3obcifwpx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3rdfaietl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3kvbkfxza.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ffxpssmg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ezoajqhj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fabwesvi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3pvkmgehl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3wdxseyzx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3hfcsjorf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3rfkpnpoq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3skguuvfh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3zazjfqqk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3abkchnuq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3zekimkje.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3vuwtutij.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3rdfmjbio.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3eobxpiwx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3jzpprhqd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3uuuvkisi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3zqxbjipy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3vttfsifc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3oekvgure.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vuyjsata.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3rxozrvyi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qzdqgkzf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3nlbqfgdn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3yqzyxjip.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3gtaysbcn.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3lcnzuebn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ajjiwzpu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3imdeqhzu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3epuxgkmp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3dxzjxmog.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3yncyitds.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3zptyetlk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vfapykku.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3rmhojgzb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3uhnpfdvf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3uevjlbyr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3mtflbdqp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ncgwftdv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3iuxrzvfm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3hixbspjd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ooyvyzvd.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3mzglsrrk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3hfwpstsi.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3feyqklea.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3dpmwakit.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3vcardsoz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3xghetvgz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3bxnnsboc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gycmpsuw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3mpuutwdw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3widmpjpo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3jvwpogeu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tghfhyue.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dcahxjco.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3edqkfufw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3lgtfgqsz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xtfswzwd.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3upsjgmbn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3dkswgury.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mazeklie.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rvhiehfa.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3glbwemec.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ipcsrlmb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3bqtaevqx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjijerhn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3uixjobds.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fpbvuxen.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3koycrmnd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3jsbvjasa.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3igdnzhnf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ucgwcgul.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3draacsyv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xwhungaq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3cqopuxyb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3vtriqjwd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3xemvvcya.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3mysrzcwr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ofyrpmrz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3xzkpyaby.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3odqwsvqj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3emzmpcse.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3eytbhpmx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3jgordjze.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mudyuhhp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ntntapyc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pbzerjue.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yppmkylg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3yvdwvanb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3hinhxlcc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3moxclany.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xympgnxa.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3cnpoadmq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ftpggxqj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zxdwowzl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cpqaohbk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3mwvwcnma.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xozxbvqn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3dmnsnvvh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xpxvafli.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3hykrbfcd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ydrpsfxv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3izcyjhbw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zipmxdbr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ltrmayuh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ozubnfvb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ekmemthd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zvlamoff.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3kykygwhq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3tqzxriiu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3tsdaegll.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3oqplseow.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3pyklpxiu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3wwnlvbcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iotcbvec.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3atyutbpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyojsshe.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3xvmvmlgk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3vvedqvuv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3dxebfskt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3bqnlyfup.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wdrdhxqc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cdjoflzx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mkoppvkm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fwcuxpea.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3awjsfnxs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ljppztmv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3rgnjancc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3gxoticzl.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3rodkvwer.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3zjifzzfk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mqwqphkw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3wuxinwlq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3rcowbreq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3mvijpuoc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gtoojwcm.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3zceefrua.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3epgljnvo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vaylcqlk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lwdfgfpk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vnrqqlqp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3iscxcnri.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3zkvvsyuu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3pnzwnhov.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wqclqxwi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ganueyym.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3izwgpicl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3opacskgz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tzbbofpy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3snvxywqu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3siplkpeh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gfixgvvm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3xxrlhkzg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hivihqkt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3tkfxpzed.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3yefqkcku.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3aiahlvtu.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3cyyjbmof.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3peqqoccf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ztievlvj.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3saqzmfiy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kupckiyp.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3piyvumeu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kupgyowc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3fusxfkgi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3hnopwsrl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3qnpeucgp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3txknjwmo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3kmrumawj.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3nfaqkzpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzuduswy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3xohgwwoz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3xalvsppw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ethtvtcz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3lcovmnoe.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3buhvsxon.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3oilwsdmn.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3oiandlcr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3llkjrdhc.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3abdgwrvm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3aeyqabwp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3hmtyqmgx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3oxtbmbxm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3rewkdroz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ewivjmnk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ouqxrhuu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3sxulkahd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3oifqxtsg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3hwtjgevh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3qrjudevr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3xjmuqgim.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3tgwfsvbm.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3mjwwbbxe.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3npoajtvw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gknaqjql.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3dlfkzsum.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wqthwwfl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3udpfihts.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fsihhoxv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3temwbuns.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3dyvawyji.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3lvpfhzup.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3anhwbkiw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mxvbyrmr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3kihrgasa.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mnkazwkq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wwpvhumh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xwecgmaa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gqiqmiji.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3maqtvrgh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gszsmyio.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3luwswqew.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rvgqhnyk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3hfifejgq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rttqfvdc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yvhlnzsd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hiubpqmv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3phweblft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzjaaodv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3zcdkgtty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnubjwhf.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3urkswgxt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xmunzlpb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3fhzdoyka.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rtgxnooi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3vilrzlin.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rtvkhypx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3whgdqlmh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3evccccgf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dxzvukxn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3uqeybjwv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ofckhohc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3umgmbfui.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hghpzzus.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3hrfvytzz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hcdtbhxw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3dkgdfufc.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3wwfmogqv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ewjvliyk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3cdhsyalk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3xlmktdnd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fkxbaiak.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3smwtdszr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3slshdfum.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gvghyetl.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3yfvgtdtv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hktwnjvi.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ayyakhmd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3ubazxkbj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3oafnvsnc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3urdqkxfk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nydppfpe.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3tzaxzfac.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ehynggai.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ypgkcrpx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3jgruiiyz.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3uivekxej.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3gguxfmth.html


<!-- 参考信息 -->