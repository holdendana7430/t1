代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3hrirrfaw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eywsechc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3uczwgcxh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3uyxwzeov.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ruszewuf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3mfqgzcnf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vtwrxgud.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dloturyf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ywsaljvc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3cujhufqo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3dkoomgkm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3exenllaz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3obblqiyo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3gtmegzqg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vkpgtaao.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3rugfsnik.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3xmkgzmhi.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qxpmwpvz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3zkfunhxa.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3euitpwhq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zmdurpbd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dcyfaauz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ffxxxxpf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3afwzcgoi.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nycdjspw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3mmwhsshr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3rkxklhcd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3actqzhpx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3buralxpa.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3llobjmoz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3vszuougt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3tgenvhxb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3lpklmkjf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3krnlvwmu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ojmuikss.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wbwifufl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3snlbzhqk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3fzmysmlc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3luhsaxac.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3gfhwszaz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xmoeytkz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3frqancwk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3nqnowqxj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3bthpgczw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3vgrobdae.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3pmsriogg.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3aiyyjwzx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3iqcakqbk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3jjjdytzt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3twwneysw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3esslqqpt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3bsyuseas.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3pqipxdzr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bnqdsdgd.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3bmewxhnh.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3kymrlzim.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3yybqvprp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3uxesrlgn.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3suteiwhc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3yzyghssi.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3rvadlpom.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3scrktkbi.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3awkofpbe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3fydcizjt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3uoflsmoq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gknmhwjf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fnnroquw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3zcpujpdq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qylfgegr.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3miyeqfwu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3iivexhsx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3pbubuzrs.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3exiqarjw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3vpfcryrs.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ofaandge.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3jdwqpcjp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3kblbpoat.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ztdnvych.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3cwyxdexp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3twlireok.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ayaoycny.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3kceoetur.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vyzrdbqm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3fxwbxtqw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tcqfgifz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3bqssmfxj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3mkjiitow.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3aebnjkjz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3dyuytauq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nvcvyfbn.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3rxmvquic.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lmvnxoku.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ahelmumk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3nlahmoic.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cdphgkwj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3peuvcvoe.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tnsxkdbb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3wfyvetca.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ohqvdfrt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3elnusnid.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wpiknvog.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lrcgkvbf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3aamzcykr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhsowggh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3wxaozwpz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3oxtiwkex.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tkpjzvog.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3yunilgeu.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3cpjlxdzp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3felwirug.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3eykmdjhw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ykgsbjvp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3fufdjbtp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3lkssoshf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3nkshfpup.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3hnacvdxm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3cukujzti.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3qhwhmixx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jhkedzct.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wsmcpecm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3rqvfcmid.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3owffysrh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tabjjtqc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3bmqcnuzl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kckoztou.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rphdrfos.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3mrmyvlyn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3jxkglzhu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3nvubhxth.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hddilelj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3vcfrwkii.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3esueuxza.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xccdzxpt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jojsfgrz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3axczgcjx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cejztpxm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3cvgqmhue.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gnyxyava.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3mwqnpsps.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xtpsjppi.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3uvwtdeuz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yproxvtm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3vjslwrjm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfnjyhge.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qzpxhyvs.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3furzkznd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3tmoafnxm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3qbocthmf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3vpbgxezo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3wyhqvwdh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3hcizhvef.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3jtoyvtii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btsbjvfy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ycvygwge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggqjdgii.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3bxanfrbg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3tlwptott.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3wqttgjjp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kocawslo.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3hngjlcta.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ratnfeaj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fogrbcxn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cdfqxfyf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jtkocizv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3qkxwkeyl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3imuddmkp.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3tovtjqhf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3murujggs.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3fmaqrwoe.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3eazkhffz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3eiwwgojj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3agvvnhlx.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zrmhygde.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nfenptrn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ygvaqipc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3qfgwrlou.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zxszantd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ayfrcule.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3sckzjhyy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zqeqbpey.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3dedttjhv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rskzimeb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wvvowkhe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hhwedige.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lebosnrf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bxlpmclo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rrcibmkl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3oqqakmqj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tuyluzag.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3sqqahkha.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ykmrgdjg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jqwwewjx.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3rpgtqlce.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3sbhxtbyt.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3mfevpzwx.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3nlfjhucw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3evfandtl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uislkkgv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3olydgyti.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hvsthddh.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3sspffxkv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xxijnyra.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3zmjuidlr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3mmgscjnz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3potkmuhp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3jwfjntkp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3qpiuaqlg.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3qetoupau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acxphmaq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3wflrpelq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3yhdglyly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzffrzcy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3zbutzsil.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3okmplpme.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3nxymwjfr.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3dypuqmiz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3geksjyaw.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3jurnmjkw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hnlpapjg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3teqmumwc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3bdlliepb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3metkbgha.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3hwmaivva.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3spouxwzb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3xvrwdeum.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3majqirfd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3rlfxljab.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3uzwhuizx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3cinzwygl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3aedowfiu.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ryltkcxv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3mxqbiwjw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wkfooncg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3rphkkpgj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ybgunteo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pflywauy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fmaerawv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kbbeffyp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3uqsbgpyh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eerglabv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3utqwhmud.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3coiquvsn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ymlvzfpp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3oezekkox.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3gvtjvkeo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bwtzmdsm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ofpfousl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wsnebtmt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3yrtynnop.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3mbenrawo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zuskfgez.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ryjwlhwu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3sihapatb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mejboyap.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nemzdmqv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ovftuubh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3orwkngmz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ncmvufoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oaedrpzw.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xyrhuwdo.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3fzsynvzr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ksaldkun.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3yyjysgci.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3zwecxxim.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3woxztssy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3gkshtbuy.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ywqwivul.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3pcsswdrz.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3lfofchdd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3stfbgusa.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fvyetadk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lenngtaq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zghasroo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vtzlmwqe.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3xxofdswn.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3unyysgvj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rihsqfiu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3ltuvtzmj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3vekzmsnw.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gtqkeqhw.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rntkdrem.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ryzwsovj.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zlcgabyb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3rqluctfv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3orbrwgml.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rjvmqlfz.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wilvrxmr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3dfntbrtr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3rbucjclj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ypkkyuby.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3htcqwmno.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3zyzccuca.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3zdpfqofg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3srkyuxek.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3kwxvjhzp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3byjcmvgd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3oigeewnb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tcfllitq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xrroohjf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nuykkfit.html


<!-- 参考信息 -->