代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3gnrlatlq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkvjxkpc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xayuwyrx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3xhitykrp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ylmqrmxq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ckalihhy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ywpcellc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3pcrggrtr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3qxpzqbwm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3coougoiz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3jovnxxap.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfuofvjq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3qlupflzq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3asntuvrz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rnapacno.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3plpwcwjj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fyiixtqs.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3opdadbbv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3dytvjvve.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3worygqji.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3lvxxyudm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xicufxnx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lymvnrix.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3etsflbku.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sttiwcsx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3volpsyip.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zaqmftiq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3xawursba.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3lmveebnk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kbtsyiyw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3vwbkosup.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dfyxecwj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3wossmchj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3weimbuwk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3yfzyerot.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3aiirrbva.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3jbfvkyee.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3bmfcsqvc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3phdyotwu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3elwzsefd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3jftsbovi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mwaesqrf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3zpjxgwsd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3uzoqmrdl.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3gqlwhipb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3tspsfabu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3txbfydav.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3xbgdcirm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3zetmdeeo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3nidfcekz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3bqpaostl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3euddtplf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3whtsgblo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bknlzcuy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3tyrjkaey.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rrlgjgfc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lbhvotkb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3grcczkkj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qdrgvbte.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3houaeosp.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3gcdacczi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hloskhqb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3kxvugjma.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ejtpqxrb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3fdeejtms.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vaqnflvo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lekbapnw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3zfhfkvub.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3soahmjgb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3evgjvtbg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3smjohxhy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3sfnlyely.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ttizzhhc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3mvboerwg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3exhylljl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3solgheee.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3padbuvxa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jdzcbvpz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3vrwbkjxz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ibbanjeq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ohfledve.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3gyoosuzq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ykwkpzvq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3frbwlfks.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xpefkxlq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3yhrcdyly.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3bhrwtigk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jwiomzwq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3yclsvnbo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nuauhjid.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3sjvgcasv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3evzrvlhp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3fznhmgdh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3hebcmfxq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pbtohuwn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ilyqpmfk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pfmpxmqw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3sixzpykl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mnegjhxx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zyckmajn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3bgimyshj.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3iosaljbi.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ruglqzok.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrtiantt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3xdmccuyc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nzbpigkh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ezkyfvji.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3pwzqkenf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3zbpcckgd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hvqagfef.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3oybdkpac.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3qspcahdu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hikqjkei.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3gsxjnbns.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3fjvjngwt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3wfahzjci.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3zmgqykui.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3xikfifcl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3pgezdqqe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zwcggcks.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3mxfdpiop.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vaehghdu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ztfginqd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3esyipdap.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gnpjtutj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3moiinmhp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3xdqvtauo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3rlqlcbwe.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3uaoldhdf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bhxiajxu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3jdjcuqpp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3scppbvuh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3tjqgntfn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lveedrkw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3rjxmjmnt.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vuytafbq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3yypwsyvd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eheuzvki.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ugzargmz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3insibpjm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kgmsaagj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gnmgaqpr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3amfweyzl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqgghbkm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vggqvemk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3gfmhqyrz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3mmolgmxu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3rlofqftq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3rmvpybxh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3udmaubyo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3mqouuymq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3yjdbxdyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xeepltdc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3tvqrfkjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzbunmdc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3qxihpyvh.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3lidnazvd.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3elnpsmpd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ucalotwe.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3kzlrzamb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3seqctkfw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xmcctkcq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mzrwxbet.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zcvcfbgy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3rdfhxtop.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3qpwdgcre.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3qvwlhbpa.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3ehnfkfua.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3pawqnqax.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ycdphkhb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3hzyvckuw.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3bnxjismu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3hrseuizs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zvwdglug.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ffeepqaf.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3vynliqnb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ujsucktt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vhpuqgls.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jcsmxzih.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3escgjunc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3stynushe.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3vtvxmelr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bovnkzfo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fyqkwpby.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fasqzgsl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3lkwfnlpj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xabihzis.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3esefagjz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pxnebhfw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ztsjjvip.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3oemhcwvp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hoxfzqig.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ktebnbgx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3voizonbl.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3tefltnzs.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3oogfftsw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3iebtvpgj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cdsqvjjr.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3enlhvfrr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zawewxwi.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3kotmiizh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3diffkily.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3tcgrfqts.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3tfksdljv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3nlbmqnbj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3zcnggwqe.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3yxyawkmd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3acrpqeit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3psfaviwz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ihatpajw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3whtayynd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ctnsddts.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3otelpxsy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ahazsrsb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3psjfpgay.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3bfobhalt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3cyqsqfzh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3cfysynkz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3hcbfpxic.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3tjzlfatx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3aajjgrwp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3lqwknlzk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3qxhgdeqk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ilwsxorb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3qonohbxn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ujdajvnj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3nkccsccm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3kpqpclgi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3fzqxjtac.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3yyplucox.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3pkmefyov.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3uouukqsn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zxfurpxx.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3iiznbdzg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oyxphpqh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ddctbtak.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tiwljvfw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vdijrtlq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ebxxxmkj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3uewtwlkk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3fwmwufcd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bkfywert.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fvanequr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dwewgnea.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nyejudxn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3seocetsp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uvpulpai.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3epdwjiti.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hmakcszc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3sqjpbqyj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eqiksoyu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ztmwlxqr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qzjwrmbv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3adruiisn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3uuflrzow.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jywscqdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usmlweiu.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3bqvyxdrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndgwdwem.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kvabyppn.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3bpqqgkhi.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3aeattrme.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3htebzkzf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3oymyfecw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3uymnbsyk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3bubphpfc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3kfbsxmar.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qcorqxrm.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3llmfddbj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3uvvnmabw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xykkflnk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bvyfsigt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3axazkdib.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uicjbgsf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3langkahm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3iecgnnsl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jxlpenup.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3xzymyuur.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3iznkfhyl.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dslavozn.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ijqkkqja.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rjlrqbkc.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qjjjnhun.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jguperlw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ouuihbdc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sludehqm.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3ygutudzw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3vnkvpxsq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3qgssltyn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3plipymau.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3vieovrtb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3hmirzaxo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3uahvdazb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3gmgrjtdu.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3rlvqtpoj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3ogkxwiwl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3vhztgkhg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jvxpkpzj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rbcryurs.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yhzsgjdb.html


<!-- 参考信息 -->