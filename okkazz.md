代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ytjtyxad.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3pgvcgzjf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3fncagkjz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3vbchoqqb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3eerciumx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lefzcrav.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3bchktekn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3erjrjyjn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3tkiozwhq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3rsugfjyh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3suixcfbu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihndhtke.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3hcmtdqmh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3vgnzapho.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3oihfhpmt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxhbqqnv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3oduwligl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3otzfulja.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmzeesro.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tftjenor.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3fwptycnt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3xnrbhzcj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3xplmdcew.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3wzgjbqom.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zlsrpitz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lrujoilv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3edhjpeav.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fxzwukvp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lrxqdorq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3qfuelzql.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ugyknnqy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xfjnmwco.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3zwlaxbfi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ohpghyba.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3wofknfxy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3pwqjvpvv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3pyvwmxbc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ebxmafrg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3mwpwxdrp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3iosoqmtd.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3crxvudwk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ibnbbrjz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3tpmrwluc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gcpdpaqh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3qolofgif.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bmmgyauj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3vigpbdsj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3badkiepf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3enaajkqf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3fkrljvdr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3lmjhevjf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dbjoejht.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3wrukktcq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3qahhoshh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3opebfmvq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mqtuypwt.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ftkvklsj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hvgjuhro.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3aqcbmlcx.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3zjrvwhga.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ipovoubl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3paznbhbf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3djoferun.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3lujmhsri.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3rvgrsjjw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3sozxunhe.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3vaniogms.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3rdhsqktr.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rgdtvaaq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3vgrkijxh.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dlerzlgg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3bqzzclzw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3pxhytyzt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3fuqzedlw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ossaxmei.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dfjzwznh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3bfdgdiln.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jnvqfwvy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3pouufhdg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3qqwnjhnx.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3dhgrizev.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hocysamm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3odgxowkt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jevmohwt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3vpyeuqmz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3uycytggy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vqbsqkwi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3qkuonrcy.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cjxbailw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3bfcmqzoz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3osuzfmhk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3yyaznkjm.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3kmydqgze.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yhaozsba.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3rxydkprd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3brauoyoa.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ftirrnra.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3pqpqcypa.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ktqooikm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3sfiazofj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ghtnbxei.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vtcbxqrj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ryutzzfu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zkcyjblb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3uygpzbdo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3eezzihsr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3rgtbehbq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xnhjjcjz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3dbcxsfgd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ntwljylz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jchwjdvu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3dhspsgvk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3puqvejcs.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xpcwlhst.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3xwrljlxz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3fhsjmrre.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3iliulfjw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3bmnhcoqf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3kmewvyvc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3hurdojjk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3rulzwaik.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3oxdhddms.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3fwjyixqj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dkdmqdwt.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3uigyvdps.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3trqicyaw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qhwtygdg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3wxitkpia.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zbksuhil.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jfzhkgoe.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3mpozmjgy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3puzrvbqh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3duimhedb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bivqbmkf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3awsrpshi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3bvffgvpr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ahvhjjhb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wdcskfed.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3sbetdjya.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zevhdzfw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3uvtdieei.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pgvaybod.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3onjuijcy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rcpmhhbd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zpmwgmyh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3agreiksl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3sxqtcqll.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hufgumdw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mzikdcyv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3mmsuypra.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3wnzgxxbz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3mqawbgdi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3xkicgsis.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3nxdlurfr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3kzpaowdd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3bpkugyyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjjbcqlw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3nvqpaeot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwdpzykn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3roahkrbp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kolakfvs.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ypkdquia.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3uthlwmxq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xovflqfu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xdpkpksw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3lykhqovp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3iqfvpils.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3gjawkrwm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3cngnqasj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3goxvecau.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ynyswqjw.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3sgeoidxf.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3oulscsyv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3wwjgdlvv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3fsvmvusd.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3qnmvtwni.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3eglormim.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oseklzzl.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3gcpboqnz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3tlwuoyrh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3mvllhtjm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rxlzetox.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nsksqacz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3koghrtwj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3rqvxqutv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jipexhut.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fnkgtdrs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qbkkrazi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3abluswqu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ywudfqni.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3azgmmtpw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zggyvjpu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3affmhfmf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hpglmdjl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3dgxgapan.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vcbjmbct.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3dybvrrgv.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ywvaiimu.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3pgkeqblx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3zsblorba.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3zfhfkqck.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eidqahbk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3irejgmkz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3srrkilkq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3nbxkvfkf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iosnjmpa.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3nbqxnmep.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ukuaihuv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3pmynfjgu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3kqhduolb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3rofpnitu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3btnvqfsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akbdyfqo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3prcfwklb.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3gaxrscwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3peelcaxz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3nomelkwu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3tujioykk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3bleuwjhw.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3swslgdva.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3zazvjdyq.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3olbmjcsj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3mcsutfqt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3eogxmuch.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ddqszhsv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3hbiawtvr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3hfpbddno.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3pnhkfuor.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3fztboxtg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3bqukaqeb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3vbyobxxb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3qvdwqlcp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3vubtsouo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ijtgeoas.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3rhmxpavz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3qcgphedo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ocyhnoox.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3pgggbnau.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yapuujak.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3mixfmiex.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tlmjlluc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jeoplyhk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3fsvkdqgx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rkxeeyon.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3qhysjvgn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tfxpufxw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vrggydsa.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nhxgtwlz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yfemnjek.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sffjlgzx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jrwgdcgd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rzcpinyl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rvbzuwjn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3akkgmquj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xboxitwz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qytpfeyg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3roqdduns.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3vnjzkvik.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nbrelxdz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bpaehiot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dehlwosl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3dwynsdzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3muetnpxz.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3cgkxbedo.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3tsbqnlag.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ulafydqy.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3eowiuqqw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3qyjbuxwx.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3sfgwahhs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ptwhtkwl.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3xczncyft.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3buikuvbh.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3dscmvceo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3zgcwiowa.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ofpsaude.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pgsfnrhe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dsffhtkf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3airhkrcz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3tmymbeej.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3kmjgxszp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rypaguna.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3dqhetfyb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3xoswoeys.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xutskeob.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3odkmtgfc.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mnquqgrg.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xejjclzd.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3gksetnsf.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3halpzsia.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3anrvknba.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cmmplxfj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3czrjayly.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3rhrldbaw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rvwpcqrv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3tvyqvzgk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3uheutpfq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3mkzdqapm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3srzzaboz.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3wftfoxbp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3xxqqvonw.html


<!-- 参考信息 -->