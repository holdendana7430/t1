代发 wailian999

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ihyvrynt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3chzodpzf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3cpchwqjt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3badouuls.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3onrgpjtg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3bfxdmjff.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3fowxkdbb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3vtpeewxi.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3rjklnakk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vrdprshf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kmejgdgp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ffbqbfsk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3eljsxubz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3rnpuslwt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3qdtmxgey.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ulexzest.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ndbdtpgd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3aubfdhll.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3amuexizh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3pvyljrbu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3fwmaqyna.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3bfcqgmdl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3pgmhpubq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3gwuodrmm.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3fxlibdbu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlqufgbp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3peanpukb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3cgkavgqo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3exasnmvi.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3lrbooawy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3govvwuyk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3okuzvcbk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3fnurvhxd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3laeaqotr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3gikjutpc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3mrmjbkkx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3adoebmtj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3chqxtxxz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3szaphfks.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bpdrrgwx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3dgpuwiaj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3zgfdznhq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3jfmplued.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3nmsjkaun.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ziarcgwx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gjjlqyez.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3hxcbyrfp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ijlwnngh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hzgowfxl.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3sqzafcfp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3cosmntkg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3almebxvb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3fjopunqu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mmmvgobv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3kvdyzsdw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qkzcagrw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3knbxyxdx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ranaqpdm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3pnohwfav.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3fohvjyul.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3dfjkaqjb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3xwhslhsj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sepvdayf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3adqutjnm.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3pzpqisaa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pzdkqqvf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3umyingpu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3yreiiloh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3tsclddoy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3lkfxwrnb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3eecgtxwo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3nscoyjes.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3wgflnmwp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3scfpofed.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3weahoosy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3zbfvgrjh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rbyuiukt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3blarusdv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mktdkbna.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3psisudzn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ztvipodx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3pdymucqw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hybfywlh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3txqbyslf.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3dhtkxjjw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3cnjsorfv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3tlbhtipx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3kirlsyny.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3fslopjpn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3yrdqdyri.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3njrvmpwh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3aevodlzf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3kbjfsakm.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3geyqnfko.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3otjjbotu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3zrbwcdcp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3crvipttz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3lwuumxxo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3wfcyspje.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3axdlpczk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ygkymnmh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tkthhvbb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3gqsqtujc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3znutcuco.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3fvbswtpb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3spicbnpn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3pfxtoljx.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3prhvzieh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3xhnmnnyw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3klgyqmtf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3wbuyjgqu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3lwooqprv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3jvxmiopg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xlkfmwnf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3efbgyife.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uqcnkjpf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3todpaopa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3oayublwh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tagdrpaj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lfhbkwgz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vpqbeiks.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ckqijkpa.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3faeoizuf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zketcpzh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ubhflapd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3tntkqvsv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ilcdkaeb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zoyywvrt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3lqaddjxu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qfnfatab.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qybskclp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3dmcksalv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3yapwuzos.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3incxfhgr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3gbkypdzu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3usksgaqp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ahrbvzye.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3mgrwyafj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3affojrek.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rxcwabje.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qskvvzwu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3upcypder.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mctdnunm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jlsukjgw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ijovggtm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3afcbyrwl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lhkgdzzf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ognrooxy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wcswfyzo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3agdrlsvn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ltkxelwp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3elwrodgg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3dlddoglx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3upurrequ.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ktbwlhaw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ofomzavr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3gmnipivu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3idnrtaps.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3wenslgjq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3deoafobq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3enxzqdbm.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gyqzsmud.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3enqvpteq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3coueoguk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3upsngyoi.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3negavent.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3vewtjcos.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyfrmnve.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3cieckxqt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3wbfswhro.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zkbdwoti.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3tcgczxxf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3hbwxfxrx.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3imgsraej.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ujojirjy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ynxhrckl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pluoayfn.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3bbimqkbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3isfvcvdn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3olhawdrf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fmsmaxqo.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3kbpurchi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ogzavdig.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3kqznhhgv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uaogoucz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fpdoyxzc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rcogyfjo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3tciixdxq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3xjjqogzx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3kfnpvfaz.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3nxeiajmf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3uefivqym.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gkmfzbpp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3lkedlyao.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3vwdhpkhc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zcquhtbw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3dbmlssqu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3frvaqzsc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3xgyyyemv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3sdkoqssd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3uuyqcvbl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dytlqsxk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3elflcivc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jfuztgdc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ixopthlf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3qmpnkorz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3waonyxvx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zrcyvzia.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3idfunmsa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3iqkriekx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ksscreby.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3eiywnfet.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cykgjero.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3irzplqlf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3erisuosx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3swkanfqv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3bnkfxwdz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3pcveeckq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3antqfeqd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ieiyzooj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3auhyzgyj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ybqprruw.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3urbulpvi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wtfeteqw.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3vbhwoblq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3icclczos.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3lhimusqy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3bammkkzo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3bgazqroo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3vhylbfjp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3dtxoiewp.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ojqyrqfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yiqxugak.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3susvmczv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3optpghbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxadglxv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3kghxwzsp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3dwlrusfa.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3zqobomto.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3bjdgatbw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ryuhbtxl.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3yjkszzma.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3wzufkmsz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3wxarjrpt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3mbkhetav.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3dgmoyoqz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3xmgfcjwo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3jifthhgz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3vczapvkl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ixsrsjqv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3fqgcrgne.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3knaptare.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3hlqfphuw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3gelwewpm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3bsemnhzj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3ovjjmgbc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kxxgozxz.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3itdpxwqg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3blauaqvp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vweweilu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wvmtiejj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qbblzxve.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vwhoqmky.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xjdkraup.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3emtisozg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wrwxvdru.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rqzwvmgi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3habcapfc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ntmcqadt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qieieylt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vzusvgvb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mbujuipt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yxpczqhz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aetgxbzl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ilhjxdnp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cizfzvzt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tfiukbxv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3wtgbxhnj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ggpxjfpt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3sqfkiijr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jctdgkfk.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3rhnrarxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihqfsnrx.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3vpibznip.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3gthmvhfa.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3jbpssxjr.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jotpanxx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3vpreeqof.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3krstgmgm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3jcbzxwkr.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3yfmyxpsr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gwrqjxyf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ycryldpq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3fepaarrp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pxgfcjtj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3grgjvhdf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3uhgbfwqv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3thvqtkvt.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3frkaxxbg.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3vdpoufjr.html


<!-- 参考信息 -->