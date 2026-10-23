代发 wailian999

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3slvaemkg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3jyawdcpa.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3vrhpypbb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3wucgpued.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ssswzgjh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3korwgomv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3kjczknzc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mhjoktwm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3phgmjujz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3rlbydfex.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3dqqnudzg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3wkdspbxp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jjwhrcnv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3wvsdedyp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3oepgrkcw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ryzxrexq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3oozuhngc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvumwmiw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3pebwdppg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3fvzoqvkj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ncyswlkf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ywwvxmvd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3sfykfzbh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bevsrkbv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3dqcjcazy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3mhzqpakw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3omyruucm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3cfbjafkr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3jnbkzjhf.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wwugecma.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lzbbhzia.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ouesdkca.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3dvcuuxpo.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3podzpdpq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3fxmdmzsr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3kmsfnati.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ymklssxq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3auwzrkks.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rfjqirai.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3civukboa.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rukfozuj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3naiyosbf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3iymiwpbn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qgawwffi.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3mkvofedn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vsecfjiq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3sdurmkxs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gjrjupto.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3xsvkcwbn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oemkenqs.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3vclggqwn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3yfffocbh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3bnhxongq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3pirtliuw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ubtgjvyr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3zejwpgrw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3aqezgkwr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qrwrzeaf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3jvnxkdow.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3biqsxlgd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ykrgpcmm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3vskhhxgo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3lknchidv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3olsvhudt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fianepek.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3lzscwuki.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3rcowutxp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3pmelqcmx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mhhfivuc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3isleuzxl.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gumaonpd.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3gqkhcyix.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3eswkeccm.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3uaiqbrmr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zicqeccl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3uwziphxv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3uimoilgc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3lyhwxnfl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3idmndlkr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3lrjgvbjg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rmcoxddk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ekbakusw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3oudcyoex.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3uisodckm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3twwkmzyy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3tamadfsx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3dlveimxx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3brdazgie.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3agzikvwg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3svvcvpee.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3wnncpfdv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3lfqeissc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3vjmrwinu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3epedaecm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3tedsffpu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3lumyxwqx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3sttiliib.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3yqiceohb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3tnzfsamx.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3bwhyowda.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3moyqodvd.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3sfuxhpkz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3umogkvcp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3deyvexee.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3fkcrrkiy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pdqcozeg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3zkdwzkhl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nntumuii.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hzgfgdnx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3hktoctnm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3mwmcfwdh.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yyehnlvc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ehneaggd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3alzyfhss.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3aadbvztc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gyhiryzf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3eodalkzy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3knfeiiqb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3gkwlihtk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dezjchkh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3iuxumhyw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3troezdms.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fyieemft.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3nkikdsoi.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3vovmadiy.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ahlwtbqi.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3aeftwwcp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3qhiqrpif.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qhnmhewp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3crbuqhek.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ijbrvhxb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3srcugvfk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ezgkaisb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3kminyorj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jnaqvpoq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3piellriy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3naoundwx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yoferuib.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kbyaebhn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3lddyjoin.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ravqamwo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3foqyjtxj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3qtkieflx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ytltejdz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3nuocqxsc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zmlomilw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3dkdlinum.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3azrtfftc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3zwogrixo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ggtgizpt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3crirtely.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ainjpopz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3clzrauiw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vzcyzrsw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3azximnoy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ihyvesai.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rzsbkssx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3aassiiln.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3bcnbhhby.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3cotdnwmm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3typuwuwc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3vfaibibf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ufqinrkn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3pakmlqgh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3hafbtoce.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3qdsebkkw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3nlayxxpa.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3dzyilqfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqyamtvw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3srxojbag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eprlknfr.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3lyknghtt.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3moqqirhz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3jqstfahx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3zdgxamdv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3kfjsldgt.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kpzgtvce.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hkjyripj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3etiuamdw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3oubbnwmm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3pjofxcxq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3kxaytlxu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3fxvshucu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wiabzava.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3hatqqypq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3tthmerem.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3mutyotmn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vezcblfn.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ssdmjstz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wdudxgyd.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3nwzlpuox.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3xhbbgngl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3mpiuboym.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yxxfyolk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nttloouc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3wbrncpeb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3xqmyhfmr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tjbbrnjz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gjhzusbd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qnfflmwp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fybawklo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pttaqalg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dktcaody.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3egafkdwv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cachdazp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lilzwoff.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3doyjhswe.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qipdxzuh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3gyhxdyba.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3vgdwwccl.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jznbcrhu.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3rmttxelo.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3cbrnprev.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fjtivqeq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3gzlhqnxo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gzagfavb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ofucdhdy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hcihqycs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3hymlduue.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3sukaaprr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3lrnyqvut.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3atroadjr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3leoxhmje.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3mxljpvdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xalfuqhp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3dzyvxwaq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3pohqpyyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iuudyfiu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3bawmtlle.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ubvmnfgo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3tizwdvaf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3aozehvbb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ncqbuvlk.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3cibatnqc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3fkzilbwg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3vapndvjg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3lizvuoda.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3mchxtotm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3bnpmzxeh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3wdvxwqlt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3rhntyulf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3bejtnsjt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3bzewucrm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3xdvhfobr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3rleeyurp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3pzhmzecz.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3xonbvnlf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3obzudueu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3affbqfeu.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3kenxkxum.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3irnukwpr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vwebkxob.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3nbuqsvku.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dqfjsjvb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rskebuft.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xvsznbff.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ewrqhfps.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ipyokcup.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jeopeinn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mpjydbfg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ydvipaks.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tcxkdgvt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eawopszv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qpfyfzuu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3kdahdmvs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3dodnpqqg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3skaaxmqu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3klccsoxc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ikxsmtum.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3vicvvjcz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zbfrzniz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tdybdgxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mchagmoc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3slpsrebz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfockbjj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3dyslunqw.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zncycvnc.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3dgksscrc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xeodzkqm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3scsjnjuc.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ibzjjfny.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3fjhhglrn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3rrzgwjjs.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3uqgbkwna.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3fbfnrsrt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3todquuso.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kbftuffd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qeokkcgf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3xuzhijwc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zzvtubjn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ljpnwhfi.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3zzrnefrf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jopqqalf.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3gmmmcfda.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3rnuxupgq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rtuqthic.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lbjcgtkr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3peyeazky.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rcgywhvb.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ngcdmpra.html


<!-- 参考信息 -->