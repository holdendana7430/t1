代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3cogdraxn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3smwaihcr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3yvxouwlk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zncegiqa.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3jgasgvnq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3kfhkohcv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3bpswxjhb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3cpanzegq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3vkgukgrj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rxevotpl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3gwcucqpb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3cxrsudex.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3rswknaqj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3txpdsjtu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tbcbxiow.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkuakiyy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3exsolply.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3fdjanagc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3iestwksg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbxvjnob.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3qkswovqb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3nqeirdwg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zewcayyt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mhlsvwus.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3xhxykndf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3armbuebj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xsgxhvax.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ezyfchns.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3owmucwth.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3eqlxrkxw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3knfmnlrk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iywigtwd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lpqrjmmq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3azrncjnf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3szrxdgjh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ntcuicdp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3iwvihhob.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ylcluieq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3qwywjrsb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xzdcksgy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3vwsqtzyw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ahavhflm.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3pfrzrins.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3vuhwowuj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rnkclcfc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3zocxaamp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nrzvlyrh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3qontgndw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3mdnylruh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lxhumiyb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3wzntzavd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3npgmzmyt.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3vdxuzenj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3vcejggpu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ffouojfc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qjiphntu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3hmrwkymc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3sraynchx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3svtzdlhd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3etkauwyp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ehoxpmir.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3jzoxzkfv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3gickvxrx.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3eljcubgp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3pnpqlxge.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jafxsjnx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jwnkqvwo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zwcqelqm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3kebhuovn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3dtdppocs.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ghpujaio.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3qmmixnji.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3nqbxsdjk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3jqvymkfk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3mpjeqjdq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3lpjmdeem.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3tdgdjkgg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3pgrixxaa.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3zpushoab.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3dotoeegd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qespcrdc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ktcwjlsl.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3vjgecqvx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3nwyxmpeg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3jtkqhrds.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rnxxojev.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3waibqwxp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3cqzpqjck.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3echpclek.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3sfcgwzux.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3gpwsnhti.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3jnnlqpsr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3emdonfjj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3pmnuvtxw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3cpigzzxz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3sdfqhwzq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3tkgkphxj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vjqjskgq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3dgkpljzz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3utgzqang.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qbvmrtsg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3lbwpngyw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3deinuqmw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3masebwjx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vcoggjey.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3osdoawzk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mrbtckqi.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mtwyqima.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3jftrexxi.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rqeghkyv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3uqtoypis.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjzlgpwm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3lhtlgpgq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lcmsrkvp.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cxhzqixs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qqfjgnup.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3wwpjjkqb.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3nozxzzwl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3smjblita.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3vlhsfyzy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3hzdeqmnt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3kzkiwdah.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3cibiuzbj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3kuwjuclh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3icvzrczz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3hprhvfya.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3jbglgbgo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sqkyszxz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3vsphhroi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fvfjdrqi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sydlpygn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3iwakebpw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rrjhgbks.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qnyqjama.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3mlnyqipj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3lgjgxfmj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3lupkcsnn.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ftrewkzt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3rtzpwbyb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xhxzlptn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3yqwvxmbr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3wmsionmb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3sluiaotf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nitydjwe.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3igwvmlmv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ndreedut.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ikmxftlm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lwasabwv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zahmdzfz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uygraibg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3qnzllkxx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3heuuuffg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3guanhqec.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3jspxkmqh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xnlpwuyq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ippjpaqk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3husumpin.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3dwnvayuw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3zacwtmat.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3qpnzpahw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikyjqgsd.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3cqmxtviv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkiuuktg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3aefznjip.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ysvzmxra.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ylktutxc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jkvswyif.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3tzvgouvb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ljvidprv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ywoicqzb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3akstatvl.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ihsqwwji.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3jmgbwxth.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3prxmvmnz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3slcsiupx.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3yvidakjx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3gdvckyvm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gqrmrgcf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3coxnxnmz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3axkmkwxx.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3nvksjrrw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kwujdwou.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3stuaosto.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3nhpatpxn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3hsrynvgn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3oacsmlxv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gvouszyk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3bqmahsle.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3stetzxhv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3etwtmgnq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xpwotlmu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3msgelege.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uevartbd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hioyhqcw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zgbvfvyt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3agdsigzc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pcffxade.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pkqgtvwe.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3rqeevffg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zlanvwkh.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3xwtnzlyt.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3bafdtcpa.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3psxtmuzk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zstpxvqo.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3jyjhtzus.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3evrdwfna.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3cwioqxkn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yqwoyulx.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3davjhlmf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qyjjclda.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3daufijsx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3vpecdoom.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3zmqaqdwh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3otposjii.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3axsdruzl.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3acbdxyrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agtwjmec.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3aijkosrh.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3oggphomc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kodblwwd.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3irnmiuxc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3hogsgaxh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3zbghmyhi.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3tqydxdoz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3mkciuriy.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3ymuckpdn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3gcsscimt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3yxakyrbk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3uffpmjrv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3bgcnzpfv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3yqnadmlp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3rieasvms.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3mwgjimlv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3uqnvhlex.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3qlkdyfgs.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3vcwciyru.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3pdggiigt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3dwqtihnk.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3dfydbddn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3tqasvgle.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zabtlvcc.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3hmxknufw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3igjzlmkz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3nnrgdlpq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3bddfiqys.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3cujfirst.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dtwhykfq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bpqgskmz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3htdcrkhh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kedecfif.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vaxzftki.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ncvljafu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dsmwyump.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qchwtlbs.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3liijdtef.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3koresfbz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3obxsugci.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vfmtpadr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3emkktvyb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3flmyxrof.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3inhnvgoz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hljlratd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dmgjnpqq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3njmjcegr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omgxtsfu.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3dgmcowfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahegsmoi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3xprotzqe.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qauxlrjl.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3fqncafbe.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tnkuaoac.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3yqulocwq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3flktjybd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3thxttmyj.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3rdwgetzz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3airdsjtg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ojoeuzzs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qmrkjbkc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3snwzvdsx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wbdpxcfx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3fsmnxozl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gzdmrnbq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3cyasdfie.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3txpbsuvp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ekknjyzi.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3rnernzom.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3jjpizhqp.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3menegbyh.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mmantxnb.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nvuphcbb.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qsprvxmi.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3gsdzskfz.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3dzhkpnuu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mkbvimml.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3nphbneok.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3kloscwgl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3uagbfter.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3gcvxjbfe.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3exxnzwfj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3aigqjbok.html


<!-- 参考信息 -->