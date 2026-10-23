代发 wailian999

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3wcvojwmd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3kwnlygvn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fnmynztx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmaxlmgw.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3gvfjiflt.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3caafejhm.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tyqjgoxz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ifjrgxna.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ijpdosbx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3wmrhzaki.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3wposgdjc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3bsbilfib.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3rgqerjnx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3katyskvp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3xobdfefq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dtliaxal.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cryxqelp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3iiaymgvj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3aosrxzxo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tbmsjhbj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3pocdleut.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vkxuklke.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vtvfkugr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3swrtxkvu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ejgzduui.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3qupiaawd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3lsrsdred.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3zsuqgsdj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3mrdszvxz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ajwjrsqn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3pjmrkoev.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3swzjsnrt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3modajgtz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nrgelxzz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3jktawmol.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3bpdecqwk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3htpemyew.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3mgcnhdbf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3qrqflssm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3lccxgdnz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3mipmpmaj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3qrykbvkn.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ukbajyvk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3rxyzekkt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ntqpxgpd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dmdjrnqn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3nsrkqsxd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3necvezwf.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3qgnpukfd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3tphoptbp.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hxnrhypr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3vrwynwiu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3susgoaqr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3wafycrwx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3bngfpbga.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3tmblveww.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3czslbofw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3nmyssjzb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rfybtrzr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3shbjiudk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3zfvqcyey.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3cetimhvt.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3xgpheqrb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ghiqxutc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3quckbyoa.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3amrvvmci.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3pqcpelrl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3oqaxvyue.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3wahhukte.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3baeauujb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3jcoyejef.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3objnfyxi.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3uqbkvqzl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3rsokgcyx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3bhwdgcta.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ouyhhecp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3gpdjgsmx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3utwcbzgb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3docmgbav.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xllfcfks.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3tzfkugce.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pitpwnwm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3rbtvvasa.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qzksmlkl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zhobxjfc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xpllczzi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3etttmwox.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3whgnlgze.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3sijwjmkx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3noqhvhfg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3kurlynmu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zeiptjez.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3dxglwggx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3oxiexyxm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3pyudrzyy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3deawtghz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3upbflkkl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vrnyeujh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yqmwjsli.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3mrhezlrh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3flltqgsg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3xhrzoxom.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3wrlkyuib.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3puzfmtvx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3yhuinghh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3mqwiezdi.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3scaoylpp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3vzwtibrd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qqrenyaa.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3riclizth.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3afhnpbyy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yjgovlhu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3anxugtdv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3mqezeghy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qgihwccz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3qetxuyzl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3yemmajyr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3coggubpd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3tlaiotsc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3wgspente.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3xiockzad.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dnotvnrw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3oaaehrdt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vwdlypht.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wzoebvhv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3sqlmzdpe.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3xbsznihe.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xrbltmtd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3lcamcnmz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wzgcinua.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3qqtgtzsd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3majbbztb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3flktiyex.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vfsleclm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3mzjjuidg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydbutaax.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fbzmbitl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3vrwamoef.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3drvsskxg.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3sdaiivxs.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3vghedabn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3vdyddxgs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3gghtsdhr.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3dgqgeejx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bahuljco.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3hiotiwqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3doqorjas.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3nadljaov.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3uvenbeoe.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3niboxlvv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3stzfnnra.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3aatvnofm.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rspmdysx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3cdzrrcau.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3oczboxuk.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3opecvblp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ptcsiivl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ertssiip.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3gxtcesbg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3yqgvmccc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xeahtkbh.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3etvwfsvn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zrcuiwdv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jexwoduo.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3qweggksq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3djgzffil.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ucfsokqh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3egyiwftc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fxnfamck.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bmsrnesb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3smqnlsoq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3psksbqaj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3zfvlkqio.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3guueanod.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3awfriuih.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qddxbvso.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qzahyxns.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ycmrwzhc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3oyimllid.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hakmkhan.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vnoresqf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3sduirfhh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3dlxmkgsh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rkhvwoqp.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3bjzbzhqb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3uveuyvpy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3szbsqrni.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3xvwppjjd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3fhijjist.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rdgkaacw.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jzgojqfa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3synxajel.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3gbqwwuxi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vnafdetp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3bisiyhbd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3oerazorf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3flbygfhy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3yhyuiwcx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3qwheuypa.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3qsopumwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpmgthqd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3blehegam.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3mtyxovpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktezqfhb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3scddjeke.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3kgcgoslo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3yznvtyar.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3rtocohjz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3xkpqtkak.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3nkqqqbsw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3urffykha.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3sqrvzmii.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3itxvnfhi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3lyapdert.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3okrftwoq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3lzdiwfgc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3jioxknuf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3mbwowrjw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3npctrfvq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3nnzizymx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3uuhrsbji.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3uqtoicus.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3uhlpleeg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3kbpyjiry.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3oizcncnw.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3mlmpmefh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cvvusiga.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oaffkgab.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lqoxcfww.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3sbkqrijz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dbovsrsf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yczgwcke.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3uxsjfopa.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ckmsrqqf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fqhlzyzq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nljuacja.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dkfxfypm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3smtcmmfu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uywflauz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3whahuzbt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rniuibba.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3icldfgvl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ypczkcro.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3lrqhpxas.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3micdqnng.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uyqptmav.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qmnnipik.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3yxoyexpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvyszbtj.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3kjdtozzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxicapvt.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3amduwtlh.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3thytgbbu.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3kqzktook.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3bfmtswzh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qhzmwpvg.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vgovqsee.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ezemnlkq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3imfzlunw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3lbqkvoop.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3srjyyyzq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3tzevqtuw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zijbboxy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jooieqmp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3spvdszxk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3aczjquxx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3trgjjxcl.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3grpmarlp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3sjbyobad.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3yiykwbxo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3toaokegw.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jegawdvo.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bstngmmw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yfzezcej.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3buonoerl.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3sesugdta.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3fpbmswix.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3svjqgwml.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kqzokxux.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3qfpjrile.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqjcdsff.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3rxudncgl.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3rypzggjt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3wweprkxd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3hbvfotfi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3zptdddjx.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3luhvftpa.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3itchhdhd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3xrprmfyy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qvfnhxpn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ukvktpgo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pjgumepb.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fyfntqpb.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3arqkhznf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ycibqkuv.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3goucfpeq.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xwdjyxge.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xqhuvjev.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3fuizsctp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3nmglpplf.html


<!-- 参考信息 -->