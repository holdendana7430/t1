代发 wailian999

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3wtobsqfx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3lbnoyvqx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3mhvkenqn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3stuvwwrr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3auesjftf.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3fdxyemvz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qidnilbu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vhztcsrp.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3mzyrycgx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3nbipuwxi.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3mobipbdb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3yticdqze.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zypibacn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3miznsjtw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3gqdwrdfg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wxcvjxbq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hjsghsnv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3lqritgwh.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3jfxpowzg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nmdrtdxi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3pfsetoqt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hlfciekt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ghtvmeld.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3joothyot.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3mxkjkgmf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3riezgaiu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xawvwclw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ztvtraid.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3qrjsmjvn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ofsfyviw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3khjdgwxm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3biuevxer.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ghpywoik.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3foeiwgki.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3rsedqgpw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3vnlatahi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3rliuqwva.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3rsehfkow.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3jiwemyjd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3nuprutye.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3otoeqzti.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3zoxovijm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3bqiztbci.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3hkmppqyt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ywgpjudb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3xlpcppwh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3cqusoovj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rclzaxgm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qpdbewkp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jlzyowbm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3okqhweeu.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3lurkvxvf.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ulkathba.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3igayztub.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3eazfqfpw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3aowtxytm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qbdsnzuq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3tjxpqsvu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xnnbwugn.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3zimksbmu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3aituhgew.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3njaxehwm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3zxmpsfgq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3vwnkvrip.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3sumwopqk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3strkrbkn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3gnyeskew.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3wwfelctu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3zcuqptlt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3uymxxfbf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3lkprhgfq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3yulwryki.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3izxaadtc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3shpeteaz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3gsiczfkz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3yumqfzbp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3bmdrzbzp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3udxkvprl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3dirlvfbz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3fmcnzrjf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3essydjgk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3umbbpjnm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3famfgvmc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jwxbrqzb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3luiqsamb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xdubpixi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3drurxfdm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3pwezrzkw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3skmxxnxc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3irjuusvs.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zjwqjohq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3dtwdojov.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3tvygodlm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3sigrcezw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3kywjliex.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsyrblew.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3tisrsapl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jmvjrkoz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3epwciioc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ijkdabsd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3zogzhhgv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3troiukhp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3sheludba.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3whfgefas.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vxvnidhc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3yjzkwfiy.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3vdravybt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3dfqhblbh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ohxsiznc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3cdvdmlca.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3whvklccu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xnwepjmx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qftuiiim.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bbhnvbnp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sitazkyy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3gnvyrdsd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3foiulpgq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ujkbiipy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3drqkcvef.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3suxewnox.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3omesqusp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zufzxqme.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3uhmayiqb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3nlmhmdgb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3yjstziak.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bnzuvosm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3iqfhheyd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3offhfank.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qxtlzxvb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qzfugotv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3frznmake.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gsialqib.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kzpbzgpl.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yoqlisda.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3pnkhiwkn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewnpkiac.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fohgctcz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3cqjjbmkh.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3aodfjlys.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3varyuhji.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3bdhnhmxc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3anqoxucz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3vymlkasa.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3jobxcpcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxywqwgt.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3djxrkfuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwcuylgo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3fgljgnlw.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3itmksfuj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ksgjgtej.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ugxmbkfi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fgjwpurr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3spmzpxwy.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lnnnwxek.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3kdufdfme.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gumkwzsn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3hjooxslv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3pooosmtn.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3pijpxjjj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3rwmibkqn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qrglklav.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3conwtqxg.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3nryijfto.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3qzgnqglv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3iwpcpxjw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kifvxlqo.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xaopavkg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3oqzupkne.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ahkrynnu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ljhrjhof.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3okfiaeyc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3viiidjao.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3xitfgtbb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3vjvsroqa.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fhbjpriv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vdbtyyng.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pkkfrygq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3svgttetr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vifkacxx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vewyywru.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yjkrjxcz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3wfeagfus.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3kidlcaxn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kdsgbuzk.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3uhfktagm.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3otfiawst.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3pxnzkpjx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3dmykdtou.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3nhpqqnqv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mmrryffk.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3rrifljdz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pvnkzecq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3wslypddp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dcewbmrf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3cbjlnhny.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3aycustcf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3xglimqdv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3uvbhzuoa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ngjuyxky.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ghfzuars.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxkonnsi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3nlqkwjes.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3cuzvxroi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyhujnuv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3dqgqcbly.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ihigeery.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3yhawwqcp.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3lthgavbc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3klemfvhu.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3onfqmspv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3zeruwiub.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3burqgldo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3xqryjrrj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3uhkmrytl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3rivzlgrt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3tslnybzh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3waepytya.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3hpdjoezk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3mcjtxkrh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3qmxlvyec.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3vaxdjiiy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3apgitkok.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3wvsxwtnv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3rgortyhz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3khrlzncw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3cbdbhusu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kifqabka.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3roxeudbp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vsitcoba.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uagplwax.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3rxwgebse.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ctibqkvk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sfopebgs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3irkzatmq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qwafravl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fzymrxtt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vexkqusq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3prbmbupp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zeoxgqib.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ulwyalqu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vyckkgmw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3biiksshn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mfxwavwy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3wxzihajl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hbtbfypd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3emnpeipb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xigototx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3elmrslbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjhuiodn.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3xwrsxtrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3seiaunim.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3nkwfscuy.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3tevjdboz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3dzcxecgm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hcqrkfim.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3zsqduvun.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3cqousplp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ikeyexub.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3szzbnmwj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3maozgxsj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3cxbbjhqx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3vmidqauw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ajiczwvu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fhreodcr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3grmvmdnm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3aiveukml.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3cyivqhgt.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3mkpjsiew.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gkxnlqkz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3tevwefah.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3mlvtllxq.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sbjegjgk.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jvhczmzv.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uzkszvnx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jgtprrfw.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jqhvjxvb.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hzdozlrx.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ukgxxruq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3negxmsat.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3rmcosoiw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjdlpdvg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3yzwvfldy.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xalofzhb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3eyrpcwwy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3gqasoxee.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3svfipgyv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ubethdjy.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3gtafspwb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3axlklyze.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uisbznnz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3epqmpsqn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wgpwoeto.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qmbsgjog.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ixxsvohg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wzjeyfzi.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bdsujlcf.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mgcmovsy.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3onzgnfgf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gvaznkyn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ockgqltv.html


<!-- 参考信息 -->