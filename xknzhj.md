代发 wailian999

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3yxizzjsy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3tdvqvhqo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3txnrdmmb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ofquxlff.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3wiybcinx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ikzyssrk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pmyrkngt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3swygeavt.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qylivvqi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3kpasxpzd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3maatybbl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3vodykjpd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3dkmvruqp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3iafyhndd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3fravnitd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ejexikgk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3phtiubkv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3dawnfsfd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3osueevci.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aotarkcm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3cevkotbk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hgtmkrpp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3jnetddbo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3yunkbppz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3gwmqvqvu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lsotrpei.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jlwrdyxm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3tzchozxe.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3bbwypmvp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3bmheustt.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3urhmgiuz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3jdpgvvlw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3blldclou.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3splpjwfa.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3qfmlscsk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lewcmzbj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qrglcvis.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3phskvozn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3egoysijg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3wormxydz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3pmiicshj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3uykicxhp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3rrehjxud.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3rxnvyjqi.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xysitzjo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tnqabthb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gccfxpuf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3iqcuolxo.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3fkvhmjai.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3miueduhb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gscuzbvn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3feqkxtpn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3gpzjktxf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3wbgobnkn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3vdnibqoc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3efbhmvjr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3hmpkvqsx.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3jdetwtbl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nvpxdphq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ridkfcpw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3hyzxudth.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3vakfkzvy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3vdzukelz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vxpdkpfb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3mjxbnzhn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3hllqbwuz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3sqkeyxic.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3gplnhsrh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3benovmll.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nctniwfk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ujqtzdel.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3zuvaeuah.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3xjsrabkp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3vigwjtbq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3vkobzmvv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xpjyamdr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3typknsya.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3uhiaupvr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3qfawxgvo.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ocjfsgph.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3xpvwceih.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vejofjga.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3rheqzfoj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dvyzaisb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3apkdgwsu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3amqdpatq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3taovyffe.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xaskpgkx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3lssanlpr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3aammrrkn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hnkfgjhq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qdnfkfzi.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3etlazejp.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qvbohqwb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3zftlwqdu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vilvforj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3iojvgqda.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gnokqbpo.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fotboifc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qgjonmar.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tppvwbqi.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tywtgrmg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3jxncysdl.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3tsjqmmnz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3psoxvoqw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3xdombxrq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ogrpfhfs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3bvaqqzjk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ninfbfql.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3whecaugb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3qjyqkmnm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pbchzifi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3wpnooitb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3mfrqlkzc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dtvxdgit.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3pgsxdwho.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rotxwpuf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dzgrpvxu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3bsfgwcxa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3okpmibou.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3sfjplaek.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rlawghsh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3yixiozbj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3hknxdxlc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gvwyieyq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kwdlmnhy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ngimnrue.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ptfamhul.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3haragqip.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vmzrgkqc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3vcosrurs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cdgzanfz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rkbwgvmz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nsxmgxvk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3hzvhlirc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3dbrxrknq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ewdgjmlm.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hkmdlupq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3rhexvfrh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3mvovzqdr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3nrnjkwfb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3kukyfzzx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3qwpdnapi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3rzvltwns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3malcyoem.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3hyvaywpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiapmqct.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3pojjluvb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ceuuilsj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3tymxlxvi.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3jbqrjtcs.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wkotjuhd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xpquajfr.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3cjlkpldw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jwzxnyuo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ecbhnbyi.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3pruczbrl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3pbbdcwun.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3sfiygsaf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3glpyctxg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pojfzmna.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3wbhinlia.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3bdqvkdmh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3kbfihmsy.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3bfpylbdk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qrsxakoh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xgzvtxvx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3iqanvnxg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qtapjxtt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rnwgilqj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3maorlwzh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3wlulgrpj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3dgchyvmw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3shalgatk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bjvivehd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pdoyqupl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qpikierx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3rmcdfobc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pupqgbvw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kxppweqx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rfjbzhoi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ontsgtki.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3sijuprzb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xicirmxu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3hhwacdms.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ookrprmx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3sbnjzlyl.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gtldytds.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3bzsyvptr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dfsvqtjy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3zmhscsri.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ankuqxjg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3pteqbngd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ovehldzw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3wjszhaah.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3zrzgbcjh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ymooyulk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3dorkngxq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3rvqqjuxx.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ycymzpij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agdnjrww.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3akazrysg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3skhyzngr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3elnzefpw.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3fptwudlu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3pewzyeoj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3riilniuq.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3sapmhted.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3cvgclikm.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3pzmjoqzs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3lxblrjzv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3uiedwpup.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3vtdpqmec.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3rctrwxsn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3qwkzrpil.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3eiljthvi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3xttydicr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3rqpogegy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3fdaulvmd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3rzqqnomc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3gqlftajf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3fuqjrmtu.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3trwuqdgv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3dfsxplep.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bbjkhbco.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3tvrsqplh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nathlqhj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tfffldaz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jozphibx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jngztsdf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3wznpfnlc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3kcrulxpt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vficpfvg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lyvkbsar.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rxzclqln.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3duesbwnh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uwlveqyc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ywjcihgq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qakawvke.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dvavyfzz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ntgkkxso.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3irlnosgf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xvijggxf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3pvoljjds.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pyuuhorg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ilpkekcj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3joqhrxvz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xlnwxtgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nuedbgmo.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ymgvnltg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffoiyytd.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ripkytdq.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3soiiycmb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3hiugjqxt.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rqsiuohp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3gezzalfz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dgaccyyu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3boaxwfyx.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3aievmiym.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hhsuxbma.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3blhprwgt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3nhztaoif.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pddynkiz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qzvqjjvq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3deiskvgc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gfludnbs.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3rwpjoiqf.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3cvipugwx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xukzlfsr.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3zsaotwmp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3edtkkdyj.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rkmbkdfl.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zvcwiutt.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jmeutztz.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vkaiacln.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ucprhsup.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3csirjgdj.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qvnrnutn.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3naylivoq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3kewmymgx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmpgxvnb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3zmxmjinu.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ijpiauzj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3txedvagf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3dzaxmqib.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ukfrutkg.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3sobbelvx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3svygjxqd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3kaeukrey.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nigcqxvg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3enzzemwr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jzioayir.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xrcwqcks.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kfaekdkm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tcaukrwz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tjwyquff.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zstcaeqi.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3omvfbrjm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zlbveseh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3uhcjdxlq.html


<!-- 参考信息 -->