代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2bqjnbqvh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2rcoybwth.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2bvrqvcid.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2oegorkyn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2vkfvrbzm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hppiamcs.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2apkyxoca.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2nsgpproc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mjzehlkg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2hqgcdwsw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2hjwlpfnm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2yrpnppop.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ogzxglzc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2hdoncpfb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2lkqtprxt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbihzjdw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ufihojao.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2zohsmjmt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2cezixwoa.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yksuxvmp.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2fdljrdtj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2bhxmnfav.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2zxxwtnbl.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2qsiiiaxa.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wkeqityc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2urwzlvhc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bdrgqnoc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lzgjrxat.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xyrddosw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ymqrzexr.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2vltbizyh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2cboyppmm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2uqmysmob.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vaktokiz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2isynvqnb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hkhfwczt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2geuszxom.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2fnwzkvke.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ixdmdahh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2tlcrndhk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ibstcahf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2vujeuezc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2cutidtqz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2gmwbllnw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2eubgofad.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gqjcirkv.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2vlhsrymi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xqdesjfl.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2jviqdalz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2mgmyrodm.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2rdjtzrtc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2qjhizzxi.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2kwbuokwc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2fvijcycf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2feynjxlm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ezokjgyj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2amnkfcxp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zlwfniak.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2peelnlak.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2sjdfjmql.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zhdpwbee.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2wbdybdot.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2orfjhdap.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jupuqlki.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2xftspmjv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2bcqdblcw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2hluxibfy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2usapvqov.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2elefugtu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2bfsgaovo.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fdssbgqc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ibmjrssk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2bkfdyese.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2skjiedmd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2sgjoauua.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2oexwdase.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2fohxfucb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ovdclxjr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kptvckbe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2hcxdtdmh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vyuxztnb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dqyhggmf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2rimobiwj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2dvapisjs.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2gwrlqodm.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2uixhwgwg.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2atwvutak.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2vluzawaw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2uwmqxzzx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2enbsbxfh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2gvaidfte.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2yxfdvlqq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2igbuulfx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gythhwim.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2sfzvuzfb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fhvmzmxd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2tdjfpkxj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2wqxmkxwx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2izhdbcrl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ttwktyqv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ewurdxos.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2bunitgbh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2eduhelso.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2goqbwhzs.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2pscebwqg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2aibkgoae.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2mgxaqush.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vhleedbl.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2jcyzmvxc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2crecjtry.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hzfolisu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2hdrbmrgu.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2buaidbfv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2qvwndpwd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2gcebdbpy.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2jnhojrfz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2tggjpgaq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2dhmukkak.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2phprazfi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2bydurlxj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2tgwzrcpu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2otolmsuk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2pbnpemvo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tvdjgiqm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2yxfppcfl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2clmytglz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ztljikvf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ibfujdcv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2osamusbf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qdrkifyk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2opuezphh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2cgtzfdeo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2dtcrwebe.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gzexmpjp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2scplekrn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2vgwkfrbe.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2flpevpfx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yivbjtpp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2svxcahfi.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iifanzwu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2agvhzxyc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wpehwpfw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2oendduok.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2neekelzy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ybaxucft.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bgihdoom.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2zomlpexz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2psiejrxv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xjeztnyy.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2lhmkxqif.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xiiwytlp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2gmpodzeu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2emasqpbq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2bvugxowj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2icacfmfj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2iitokxvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxtnboae.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ejijzzhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpooqfxt.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2zulqmkmo.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2yfdlxvrn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2snhuvpns.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2maeolxpb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ktpvlxes.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tkuxyuex.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2olxasfbd.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jfunxdbu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2totrzuyu.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2dghfhxwz.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2wmvaikcb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2svmeeiup.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2kcmzpziu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2yirzpsxx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2tpsipych.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2gcwongfd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2bjfluifw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2sxwrsfce.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nzestikv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zcqsidqv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2eoljvhwh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2thpxadwj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kwndqkme.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jrzwxlfb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2baegysmo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2cafbjcbt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2sbvdhbjo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2syrnbvrd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ikzbmuvi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gagcrqjm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xgrkpflw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hujeutbd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gquxdwdl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jlpcjinu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rqurpwzb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2jkizrzum.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yzocztcn.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2pfsyhlkj.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2myarjgad.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2nhhqytbs.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2wgarircg.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2dnwgjobz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rwducdvd.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ujvssduz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lemplqfe.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ierdomas.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2squfigwm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2rzyttile.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2kojkvpvw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2lppskjbr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2rcycxxwj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2mvcggaxm.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2xcnpqmbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ynchbvsx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2exhetmlw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2hpobrzgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2auddujkg.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ldmfprrb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2atrnbrhc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2yanvfrag.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2xikqiaoi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2bdmtdaxi.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2arkcpfhd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2doonkfib.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2jpaylnna.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2oeorjsss.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2jfpkegub.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2wytcwvde.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2vkcxnfnm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2orsqfbvt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2adqiviur.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2pyucmdmo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2xhtbwqma.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2fvwqplxv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2xuvxspek.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2jjkaksko.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2hjvmchdj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wszaioif.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2dkkgkozf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rcufddaf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qzxftujd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2paxslwjv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zlonkvlz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mjajdpxu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ssmawfbf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2nxnxiyjm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qjymkoxb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wqnvbvdn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hugqsnde.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2gjqnymrw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mbfemtio.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2astoictu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hompyzpk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ehwaxfub.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hxtagyzm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xotmxbrv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jswviuel.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rqmikxvj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ewjutnks.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jrefgadb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kbtaqhkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozrnmdrg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2tpcyajwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwhcsnst.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2drdenjir.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wfwmkgag.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2rvbslkng.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ejzkcwjl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2wwslhfrx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2uibfzneg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2egqvubqq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2cerpautm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2snwaoqcj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2tvppejqa.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2qqbyyvbw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sqbitkhi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ejgmcazh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nrthvyyf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xtukwrgz.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2wxarooys.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2fxpdtdfp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ahqbnpwx.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2pnqeyuuu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2gcycqvrk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kqykfhkc.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iwxoycyv.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zmqnthws.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sowwlyuj.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2bczlnawr.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2dhxcusan.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lawrwoeb.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2lmqnsdkh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2xjrkpdmn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2dmcilsfw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ruwoegbw.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nqkbdxvp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2hicnnrip.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ypvrxbqy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2xcbhakul.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2mxseejte.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2qeqopknn.html


<!-- 参考信息 -->