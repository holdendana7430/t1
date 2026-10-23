代发 wailian999

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ksppdkzo.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3wovmxxtu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3hustcgkd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3vqckuvme.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ecwftjro.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3xffyxcxz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3opwcudqt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dagpydxa.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3jtggdtfg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3uupzlkhf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hzxwzdta.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tyblyjeh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3maypzarr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3sudwnspf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3dgaduoxp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3fzjiqghp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zexojjtj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fugcfkbo.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lkenoszy.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3iymrilnx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yuqurhou.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3lljnyvfn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xtsmitzs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3zzqxfzti.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3batjwtzt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aqofzuew.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vaxqvkxv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ogcgiexe.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3oqzdeurh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3txtsxmhk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3rfxlnmor.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3immogveu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3sjguqcen.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3keftlnlk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3fyzsdkdq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ubvvrwtp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3rmbppqgo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3opvfvgzn.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3scefkvzm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3marcrgac.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3cdniauin.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3wzwfplqy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3vmwnnduu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3txmmcfhg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3wgbadrwp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3lmnzarvp.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3mghosgnx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3jghriefo.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3brixernt.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dirdvkny.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3qomzsiyt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3muvcbyjo.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zdbhivhz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3kzvwdsrd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xawmtpzx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3hmgntrdq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3zmzeanii.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hxrpwzvh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3gqylflze.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3wxeixwbp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ztbdpfox.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3pkwavcqw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3yzbyhjin.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3yqwwuxar.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ozjwnrqg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3frihhyme.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3mgtprozl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3erfyicbu.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3kveuzqrl.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3edptelho.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3gqzyclrv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3sqlyzonj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ezboplbr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kqdibaqk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3hdhyfbzp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3stusqdvk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3pvzfzpns.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xwljjsjv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3tcmklqkc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3gifvktwv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cgprnbcs.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3wrpqdnqc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3rkadnilr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3wyqcpjla.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ljzpsake.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lcvqjjov.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xxdxrefz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nezoazjq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bofvuish.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3glruhyde.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3dteybfkb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3iwcpevji.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3gtyjtpei.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hrixmxsz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3uvyusxdl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ldaqhqqp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3stzujrul.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yerlldql.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3dnuckclf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxalaokd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ozbavadi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ykpkexxn.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3hivbbvlf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3lyggmuuv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3xzcgzxsf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3dhdpyeqt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3psyxgqhp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3jonijcea.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3gihtbytr.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3iqjqxhuq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3vznyxvjd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3yfdvkpwo.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3bhktgjsl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ekojdpjg.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3fjarhmau.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wmsiwqpy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3vbgvadeb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3vjrerxpq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pmddpqrx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3idzsspvl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ncpayhzr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3stxzmcul.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3eilujilu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3jjhmabys.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ajosaycp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fpdobcym.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wchibpdv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vebsdyob.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ekpokqgx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3kzbsqezr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3kwumcira.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3itfqigja.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3gimdvkfr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qdtobosb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3oazdxrdx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uzaefmcp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3eqomyqle.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fnwvzipv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ugzrduvi.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbomhbrw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3mfckkcqc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3pagdiyjk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ypmuqixn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3aftmcfmf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3uvhltwin.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3lzbfqqxg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3xncvejmd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3aotsfxzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpztdamh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3khhwdxmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvgasnoa.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3vlbdcxcu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3pwdxpfhu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3cesbhtee.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3dathicdk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zymfbbqr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zyfcppaa.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hzhwfrki.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vqpxlfbe.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fvhoizls.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3losqmrxl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3lnznfabo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3evcydtkl.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3jqnnkitz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pehnskbb.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3okrpeolp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3yuqybygn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ywcezwci.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3pfsbwdsq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3torlpuoq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3srfvfoxp.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3mtdthtph.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xneqbivb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3diakbvdc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3byfikewo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ebthqttd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ptxsogyz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3miankoyq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pkwhhhvo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3kbzjavvo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zdtdxeqz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3cepvvsub.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xoimutli.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cllcoejq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ehrdbrab.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bcxjcjnn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3daldxnal.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ttpmpgbw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3leyytzbm.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3vskcrdlx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3sptglzkf.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3yaaihcei.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3gofgdibj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bkthprde.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3nolnchiy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qvfkqlyw.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ojqqhdpl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3juhhvryq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3avetpvwi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3rxcvfwln.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3dqxsvydo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3rnhejkvj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3bimgcbes.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3bwxwdqzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubkazosv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3wiqnuldl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3wzmavlwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tokesipd.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3yfixwxwu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3gvivzyoh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3xcusfadj.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3vdiqywua.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3cpqnftam.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3peflkmng.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3uohghxax.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3alvjiiaw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3kyusrjzi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3gkrgcvnm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3mqkvuhxj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3jpmbrzim.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3wtjylmnq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3owenvuri.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ffwirwac.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3engwgjkw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3jjbupzwn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3leupgvsa.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3bjfimxmj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3mfdkjcgh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tcqmfcdy.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3jesmqkse.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3shrjoxzk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ocggonvv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vjbdcntf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ictipqes.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3lwwwatgh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dwmltuhr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ewamlydr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3umgijvkw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fequelyf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hkbksmxt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cazwlnzm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xakdqihr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nmnidqar.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3aoukcrrk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3otakqkzk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3zqgbqdsk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nzldwxaf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ivlbeqyo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3txdbxhbu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3rmzgtroe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3btqthgvq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aejkgceq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnrrcxgj.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3sbniovmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgqjquom.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aggsldfu.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3gqhjwfco.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3wjsfctlf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ydjfznmu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3erhmzgyr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3sozxiplp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3guqnwkte.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3uppdanyg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wnmdiaiz.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3xbexjuvc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3rtfohftc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3giqsdxew.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xgshzjkr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xabmcatk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jkueihlw.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3wsimqyvu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3lnlhjkss.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lqqegnlv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3yncbsoim.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ngdvgkaa.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dsjqbobu.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gyplmoxj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uyvxcsaf.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bcknpian.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gtusmoss.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3oathjloo.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lippurri.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cfpipjlc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3tdakcuwc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3koyykqzk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qkqlekoq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3laogzysj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ducfrzlw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3jcrtuosv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ejlcybqv.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3siuezwqj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3trlxjfee.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ykipkbrk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jgiakxmr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mczwwbkb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3trukemck.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kidfqqda.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3koxqhssa.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xakyiedy.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vzvldnpz.html


<!-- 参考信息 -->