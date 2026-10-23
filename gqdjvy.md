代发 wailian999

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3jpdyjdfi.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3betderla.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3dgzhstuw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3zphajohq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3zecuehgi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3autdodrz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wuyczlxx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3chbynoku.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3wqxonclr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3owoykuzo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3xulaxnsx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3sxmyjxkd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3xpgmxsip.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3umftopwy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3sorelswe.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qakfxxwu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3afivhamr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3xzqvjjxb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3awwkqmlt.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3zmbyfobu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3dclzdwqp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3jqhuxula.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3qvutcpob.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ifguwlru.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3viuvmoku.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3jkylaugs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rdhvghjo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3kgitpqgt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ccifvryc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3tpkpfzfr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3drqxhbhk.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3hihehrdz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3tzsmxsxr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwjrlczb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3anqybllj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3clbytyrn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3kcnqpzpp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cyjiuezq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gifrlgia.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zntmbmum.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3iixexyvh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3yyqtlloc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3xvcrjdkz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upmiavac.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3vqhkacsc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3dxyrcjlt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3aovhstcl.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3oyosllny.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3zlyzjhhf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3xawqxasu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jbzdkhzr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3llnpktfr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3nrwfojlz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qnbkwraa.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3bdwepsse.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cxppfwcq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iecngosd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3fkfmvlia.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3lbiytshf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ymdqkvjf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3qvcgpzmo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sptvjqlw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3dlehzkjb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rqilgnia.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3anamcsio.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3levuxfsd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3mtyzxgrx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3knwhgymy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3euezotze.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3twiyyady.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tzjdoltl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3zrebsozp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3iaifprwp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oqvsrwkk.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3wetqlcbw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aboqwnca.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3rzvabext.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kwdfvrej.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qgiffhhy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3gawitrge.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3yxblxyzs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3tjttxumv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3vconifiz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3gbonuqbp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3iaonaefq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hbugaoyr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3loxpznrd.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ilwenpau.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rgdeytuw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3oicaoctg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3egvrqgko.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3emzpmxjv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ksyjdpev.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hwvyaqrj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3tdzojqch.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3fpdoxbjq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3znqdkngb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vrtylmqx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bclxnpuq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3isektueb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3aamunzbp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3vsvovuns.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3hmllyohi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3zgvhqctq.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3kznbsitv.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3lrvdfdyp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3brbqwiin.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3gcpnwiul.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3mmsgopku.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bjzaqemt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rnuhvdyi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3gmzekyjs.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3kbhtkghg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xswilcgz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3gcstxilx.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3nuoqlggy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3mhljiqed.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3zskgmmre.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3dosztvrk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3xfjtrqxz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3osguduww.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ujedtrpb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3xmxougxo.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mucptdsf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cuagcwqu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3iirvorvj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3rduawago.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ekrkzzzx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3zpkkrykt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ybkwsaro.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3thurdsrt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rioymmnr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ukzssnsy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3eyoozrvq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3oubhgzco.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ptdwesoe.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3zkxfutes.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kpcdkcjo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3jysgswkc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ofoeejcr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3kbagyjku.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3jksawzts.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3bkkphoup.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3syuzsbwm.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ldxpmjme.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3necfrukg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3stjtswwx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3cvcpthfk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3eozrdqmt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3uzbfmtse.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3qhngmzdh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qkgizvgj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3zvrfkaai.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3peyemjmq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hkuecnhi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3pfqoengg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cdcsrlbi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bdllsder.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3izlerhic.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3pawmfwjo.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3zihyxmei.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ezyruiuv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ibcaaqzn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3zspghdue.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ujdabuvc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3dacmfdvg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3vekzrxdi.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rcfpxzhm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3pywlfntd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lazzbhjg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3brxlbdad.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hqtgafhy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lmwdopkf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ohaeyrzd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ugyzsbbp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilimdjge.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mhtwhtcw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3jzkjxvzf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3pbtulwmo.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3pvozefpf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ofcbruny.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3pxhublwe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ukpfndye.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3flexnttf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swsmdpth.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3unvzvyuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhvozhnh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3bkoxodpf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3etnzghyp.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3keyrkkmd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3zzgzqamm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wwmndmxx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3afratywe.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ekogdnue.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ybekmvbj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3facouzts.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3hlaxriiu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hngarank.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3desrouwf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3gdkypwsx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3obtlqxzs.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3liyberzh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3sawnodnf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3iuzergaf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hrdtiiwc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3runozvyd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3nsuhgjnw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3kmuzrycw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3sthlnmsg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dtlljrzy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3umyhoppw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jttcyjxi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3pfsqfutz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hsnqknnr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dbvvlyve.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zwkcdjep.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3deciwmxh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3kuncevkg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yscgfqum.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hjncuhvk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vzqbcxaj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3giazmrjy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3odfvsrvy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ktxtfsgv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3oqtxxege.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ljbrrzyy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3xrhxbkpw.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3czqshwhr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3xgemhorp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sjhcehgc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3wenroxwt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kzbacwtr.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3avjtayle.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jlnnvsrw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3mnpesphc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3lbwakyxk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3iftniiyq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3sdjrtpqi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3nhcizgtq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3nitxusjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfkrhbyn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3nyimjtzj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3nnkkhzgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enxmocrf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3gipgubpb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ppqkygan.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3audbzrvy.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3wrguvggv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3geeobbkp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3jwztupvo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ogwjrhla.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3vxwwnuki.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3lczbtpcd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3otygothh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3szuzsjio.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3lqpjssks.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ajbwobsi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3fefbgfqn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wxmvmnyu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3lqnlqjdi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3qhmfjqup.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3cuyyocdm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3hoyzcgqi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3ybrkfucr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bvthnhjj.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3zdlpuyav.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cwmnjdcg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qhiaiojs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3aipqabbn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dforifoc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3urckvymq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xedtdptu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dgjmdzpv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fbtefwje.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qooajasx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gujczviy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lhtvgvlq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gwtxxxsy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kfraemuu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hgighvzz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bpjmwgmq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lkvrskhc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pikfhnve.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3elhxwrcw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zhqdptex.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3mcarsvsc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ofrimxjh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vwkmhrkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsxzizaw.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3fwtybswc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwuqovqe.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3bnfkluki.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3fpfclooj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3rgtcrcph.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ijnzgtrl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ktlisokd.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bhrhpbzc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3agmhvwaq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3wserqlba.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xtspcihr.html


<!-- 参考信息 -->