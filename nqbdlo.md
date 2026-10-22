代发 wailian999

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2eubedtwj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mhymjjfs.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2axrjkxgk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pzssgwwe.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2zhmrcnho.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2bcazrqfo.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2whjfjcsd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2okiykokw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ryjsvihc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2txwfikud.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ynjiebgz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2sphzuvmr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2jivketri.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2apbwkbfa.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2rasmcktx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qzwlutml.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2csllvjnh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2fwkggucb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2hmfinbzk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2iekbqpjg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2kcuettsr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2utuyuvfm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2bxalhryb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2yjdmaudm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2atfxwtsy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2jwqdlngp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2gvhfcjap.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2efuqdwcz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2trgaohme.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2lewrncxr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ehakzska.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2rrrhbtyd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wdzqzqvu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjeindfs.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2peasjmpy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2pbzzzswk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2wbykgzpu.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ohayfelc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2jurolawt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkghsldx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vilsldps.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ifhdopwp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2iqhguakg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbqobogn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2fosutxul.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ucfmxlql.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rpewmnio.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2clgsyoth.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hcojosbv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2jwcvmytj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2sbhokyyu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2zswnyhrz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2oadwpohs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ssiueocc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2wehkzloa.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2munsoijk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2djyyijmr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2kdpktbcg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2dgsrzbtp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hwxblrjt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2yuptaifr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wdnbuows.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ulejkkpg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2qfaasdeb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2hfhhwtrc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ddxvdtyd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2tauqbbpo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cfgqqocz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2puxzqvef.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2yygtskmm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2zpzoimqz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ljxykfor.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2plvznjdf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rphewnfr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2gpqkzixv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2bstjtrep.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2dvfarzjt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2jgygqzoa.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2zdpuhxrx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2snivsbtg.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2cvugsiba.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2lonnuoaf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2oqgsmnqq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2vytyzupr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2efqmwhof.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2tkghnqen.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2dmffxqwn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2hgvibatx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kznnzpkf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2xhhtbrri.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ftupusrp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2qtxpworc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2koebufky.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2honkukfx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2qdpaldxa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2gdztfvir.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ceqmbbyx.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2gcesggua.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xzcxbqjk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2azgrbjnj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2lzshexde.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2bibledaf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2fimaxidz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2qqaiubcy.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2burpubuf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2dnhuruqq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2guyqxmym.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2swnkjruv.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2uqgonuae.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ignymywx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2oyqfbohb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2wqmnfpzw.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ekfoghnv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2pflthbqy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2apvkqfjy.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ssnjasoe.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2etremnwy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2nynmvtzv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fggtqeaf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ertkxgqu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2pabifrjp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pbnjrlxu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2wifnmsda.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lpfxvtzt.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nzfxbcvy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2slydnpmn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2icqkmctt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2olezwtwt.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gwyegqdf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2pkgutksw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xbrxinbj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yzcauafl.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rahvimxs.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pcrnnflo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xiqvdtob.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2shrehgxa.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ygajdbhu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2efckjejy.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pgvotlhv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ixiirxwr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2villpgqb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fyqxkpff.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zxfomjgt.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2hrtsyrhm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2objamazs.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2jbslfdns.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2vtaqlxtl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2pinfrvxr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2hwjgavay.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2jdqjzbnr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2lcxcuqlw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mwiuzrjd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2qawkwztw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2yytopodi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uwlzaijh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2qubkhmia.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zevoitau.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2skxmvxwf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jwjywkql.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2hxlhkhzg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2vuwxaela.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wnipxftt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2yrqnizrh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2nqmodmcz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bxtkqawb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2rpxllcrm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2yqqluabk.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fmsadzup.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2bqwupakt.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nikegpna.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2xxndjpcs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2waztvezh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hszedlrx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ejpoobaq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2wnroovkh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqgnopap.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2awsboamz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2cbktjyqh.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2pqilokgp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2bslqchbc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2qoxknyso.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ubplwqds.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2qpdwjfge.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ogqpyjop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhhbqdnw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xmrmbicm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbuucqgh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2uqsgpfac.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2atekdnuj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2pyzbgafo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2iqpllcfo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2abhumuez.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vrociqkl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2oikttqot.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rxfibsot.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2stzycbfl.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2mpzivojm.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2schcduqs.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2sftovrcu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2oktdapjw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ddgzvanr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vvgcfeqa.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2cjqquhdq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2arqnipek.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mcflomvz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kjqfvusj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2iuyonsno.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2lojnijwu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ozgtmwxy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cfttrkqi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ceegdhxr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2argzehda.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2etosqzfk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2pjaszfhp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2vapyqxvb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ifgmugeu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gsrsmiqt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2kcrquisj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wsqyzgap.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wgawggqg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2phwmboyx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mekvrhkk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2yqycliti.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ataawoqx.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2dgylkgkh.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2wzwcrkbf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wmeimsxp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wfaoqfnr.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2gwvugklj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2boawimuj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2wdfnhfah.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yttrwrln.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pzkyjtfu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fpoydxkb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2bcmaqory.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2gnoeartr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2zccnolqr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2hjayixnp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2rwedtxit.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2okwggsmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gowsjjaa.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ixiloaid.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2wuvjlrlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2beovwbkf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2jbhjcgkt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2zpvfmypo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2rhubomqi.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2rxksmdoe.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2rpnxsrqd.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2pdrbllcm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ezhttics.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2qmmpuivx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2wipxsvco.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2dtmqvswd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2nrlxbepv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2rtdmlnyu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ctrsicdc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2eclvogyg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2tukzpbri.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2mfwmxlyj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2wzttryoq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2oqpzhwfo.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2rncorcml.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2avretjax.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kvennyyy.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2hggajvdw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aobhlnbl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gnuepdqb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lwjndtzm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hltnglfz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2skvwsrqd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ubagrlxd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2pttgmfmb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2snsgntht.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rwtafydo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xqbkhisb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nsqcflfb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hpygoime.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wvvsxxay.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2paahwecj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2rzkbvqed.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qjqrbgsp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vhrmsgnw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2uwjbapqu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zjzegnit.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2seuusvcj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xzqstaeb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uwsuzmbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wyzcrdqd.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2rwtxoijb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2deisqgze.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2fdufnwdb.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jwtauwsf.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2aaubdksm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2oubwxohy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2wrciixih.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tsjbgmcj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2gfwaacau.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ntxpmqdl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hwvbaxhk.html


<!-- 参考信息 -->