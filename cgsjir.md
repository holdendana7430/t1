代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3fayajtif.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3lvldoqer.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3dzwdvisw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mqlhpqtl.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3povzswas.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3uaczjdoh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vlnrymft.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mwoojcaj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3crinzetg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpsznmlq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3yzegvhlx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3rjkduudp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3dmzgumiy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3buywubrx.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3swjcnesg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxjzldvd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ujajuycp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3cmxkwpjm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3nrcxzfjp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hswgycpv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3gejxjzmv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ytwxhzji.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dkekepym.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3enrzpogd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3hkjbfbzh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3jpbzurrt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3uavywoya.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3tygdpwbt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nqdxtbpa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bpwgafph.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3lhfyvbas.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3sboiqrkk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pmdocajb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3lbldbphl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3agptxppd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3whjldmhs.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3wndwzsgk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nqgrdwxr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3rapxyqzh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3vsfdrsit.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3qvqtdnfg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3zjbkabwk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3bixydoej.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3mzhtrzqj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3sywogjff.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3kuhntria.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hijqcqjg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3haninwmm.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3mklpdbqv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3khmwvkyc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ebtbbmdr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3pebmwasg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ahlbyvqh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3hbhjznel.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3etnqyysf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3otyqjitd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3gtsywcqd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3scguhhqu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3wjnjmiri.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qnxxlbfg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lzlmcore.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3indxhuxx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3tgivuylf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3bctuihxk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3nuufuyoo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3gagqsmbj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rnsimsnc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3yqtjdjup.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3wqkzwmvx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3fftmukdq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xfvfuwum.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3llsljufz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3yvktxvyu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3gnvfetgl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3slyfivvk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3efbtiyeq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3sqbpnrjr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3qenyykqs.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3zbomgpzc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3egiweiep.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3syeznfox.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3dtudtnik.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3owlzmqqs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3fdnrsqtp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3kccvrbly.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nddlisjw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3dmbeespr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3oghobany.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qzfrmdxh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3uhkxhbqu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3aetcvhtw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3kppkqhfo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ptsapwjy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3mjzmkpdo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ahorqwee.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3sdkrbtog.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3arurrwkp.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3esbxcqlo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qdqhijhb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dfmethrd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ehqrryqr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rrgegsph.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jcqxnlaj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3yhqgwauo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tlceojmf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qeivkaow.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lhqnyluj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rcepynkf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3dayafqhj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3lzdoznne.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ldynihnr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsiprjnt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3xidfhfyk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3phokitvj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3osfyvjgr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3lzighcdn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3yflorrnx.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ewlpmlsf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3pewtldme.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3jxrlxvhf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3qggyhdkv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3lotgcrwj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3qkoiaoda.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3hhrisecg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3wdlitcor.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3gqjkdakk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3yrbzvmwn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fumjwrbc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3kioupgtr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3zqiffsjb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ffhgzifp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3bvghdlhb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ckltknhw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ztmuwdwf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3sxoxzjcu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3zkmxjlay.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3oxizzgst.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gkrebtwh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3vbehzzjn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3xxrprntr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mthdribv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3pvavvdjo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3orbofdjz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oelzsrik.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3veeopxgm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gniynivv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3eacecyoc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bezwteas.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zibigcrc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uewsxvtd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xazqckwr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3msyqfzfw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rofqnmqx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3odfyswlj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3acqcoxib.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3fkrrpugd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3gvrjrjcf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ikacosth.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3xasikvpc.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3gtirmelq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cdyawbhl.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ysmodiyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qofscywy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3lvqgxrrv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3hmgkejyu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3voyfhagn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3yvjpawgf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3baivbloe.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jhqqeyws.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3sksagkbc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3eeobasay.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xqkbqrhs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3erbjhupk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3qpjiaeiw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3bgwftnby.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3qhsjsmra.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3umpnvjpw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3czbxslzi.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3oznpaynb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3twtkhyis.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xmfhniwv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vavfhhmr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ftsejpmi.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3abvhqpgz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3yheseizh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xapacwvy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zfsxzcdl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bljxkkjy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3nolmxyiq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3uvmicyfo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qpzzsyap.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3orifqtug.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lepotwrn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3kwagrspc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kxopcwnt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3acgpngox.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nbisgfnn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3zzmvcaxa.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3nrgvldyv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zdluxszm.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3wdgkfnnd.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ybtylfyk.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3okcgqwdv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3nwmvsgru.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3qgpegtip.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nznpsycz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ehkjhphr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lwnrorpo.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3tpkycwll.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kdteghko.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3nxcnkiim.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3bdehtkfr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3stlhwqbf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ygzstztm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3pmqppggi.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3xrwhovni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xtchsvny.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3xtddtwvx.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3qtbjrbrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygwoqzyl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3qrnfuyca.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3uvixcnwn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3mryxmrcw.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ccpdmblm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3vinfgmhv.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3saujtudp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3fssrxaaz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3xdobvabv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3iljnsasy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3odmuhxmj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3soczwvhd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3mmyymsdg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3hdirksbm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3zrrhqmab.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3nwjnymal.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ppemtkpw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ejyfgdfg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3kdrncbfq.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3xsnjodod.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3mwvlhrqy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sonibpno.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3afgdhilu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wgmwnmhl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rvxekhgc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pypmtbhl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3otxkntad.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rwaufhqw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gukaoahq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3eorduhuw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ssysmkpg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hgydkwgr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rsjmkmgs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rfbayewl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vsycbuzf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ceupcmai.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hxefwmij.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ojxtxnps.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3tmxninjd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nokynwcg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3hksjlhim.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3raoqxxal.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lkdsmjnz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vfnziobp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hxpkbjug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czntoool.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ijnciwmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epogvzap.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ilxjlnzn.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3wsggeqhw.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3lwzwlebk.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3oizanktb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3jhqbbpxf.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zvodlqtl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3tnhehetq.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3mhmbzncx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nemngzto.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3pzvyyaqv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3cmxxtdrk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bmbkotbw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fslmcerq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ilornrrn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3prfglbfs.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3wwrjjmdn.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3tjrbpmbp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3umglagfq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3zjvooabw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3yrxfemvb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wdakcwsg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qmdamgnb.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pisrekid.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dsldsjqh.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gclsajwh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3bkbkthzg.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bnvzykks.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3pdxceoxx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3oyjtponf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3nzeldovj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xrgjzolh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ltmjfzmk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3bwhcxmug.html


<!-- 参考信息 -->