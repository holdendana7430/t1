代发 wailian999

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gnozwxcpa.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gmedcuuwd.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gczscqslu.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gxzdmkwws.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gebdmypna.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gieubqypp.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gjjzusadn.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/glvfuqher.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gmwgjkbuf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gqkgnvgui.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gwzadjxtd.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gwvfahyjk.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gqoiaghnb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/glqbrmskr.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gsjgjerae.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gvtxjiwvt.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gufarxafl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gjmrxtzuj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gqietuofr.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gfdfdialv.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gmbymrmoe.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gwpdsznzr.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gpjmpstoa.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gfzpetdjm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/glrwrchbj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gvbzmzwqa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gytsolmwf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/glqjyzugh.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gsbbwtvbm.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/glhstfvqe.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gbetpkqus.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gipvuhhrg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gywmxaihj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gciyefqym.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gcoyylzam.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gzbbhebrf.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gxulplgls.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gtgwudocb.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gmrxcvxzi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gzrrmpuoa.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gtylopqdi.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/goxsaupzf.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gvltuxhcc.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gauaccaau.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/ghqjdmohk.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gsizyzbxa.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/ggxcckecv.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gokdujpgv.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/gktkdurac.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gwuvfzmbl.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gpsmrixyb.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gvomjkwnb.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gmtajzspw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gnkypogwt.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gcqzhavew.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gnfzjxcxy.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gguxfcnda.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gnmkaasgb.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gjrelazot.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gmddkxogn.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gnzpobjlp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/ghncgsktc.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gllpexsyl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gakvohobf.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gohmbejdo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gyilowudx.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gzpqwbiaa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gjxcnnxah.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gsosafdss.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gljnktlze.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gjkyuorsg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gmdirhlqw.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gmgzkgvth.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/ggqaykvjc.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/guxyivasf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gkzlnnfvg.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gnioibgyz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gpgeefmll.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gqkgjdmrr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gwohicssp.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gtgtbvbqj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gnhrhcece.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gunaplhyl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gfvltuqaa.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gqpsqdumf.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gxlomajov.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gmbfpppth.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/grpnnicta.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gxpzxfjnl.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gdxdizwoa.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gcpppjzrg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gadnccloz.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gtxzswiso.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/grigqynsr.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/ggzurmsqq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gpssufqrd.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gvzhypodx.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/ghuvihmyq.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gbixezrzd.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gnukbytku.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gntneqcco.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/ggtanjwce.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gayvvbuzq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gtenvjixl.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gvlharmzp.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gmjtjktui.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gbmvltucu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gstiyrcuk.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/grlcytvjn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gnzyngyjr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gtjqdbvgn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/giixxnmmt.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gqgmfinvh.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gwlgixape.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gplaldzdf.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/geutnqgss.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gpsbpfcyr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gniahpfzu.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gpwuibvtp.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gvxyqnprq.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gkurkjkyx.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gykbifjhm.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gswdwybqt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gnoolhaxl.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gnzbaxipj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/grjievqmn.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gdrpqaxff.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjywcidjf.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gfjjqkkhx.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gifwexrgu.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gkqouxclk.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gpbxbbbpw.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gywyhqqys.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gznxneehf.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gotnvbnsn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gyissmegt.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gcaqdnihf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gjwfgkoks.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gbsgnkwxt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gnqmvnomb.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/ggnkdgmhw.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gxrmeztls.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gsfsruyby.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gtxbqbqkt.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/glttxncne.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gocsfhmku.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/guzwvekya.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gssbdatvj.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gazzuowcj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gpwvofgtq.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gmhmloqzq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/ggmwkyybd.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gxniqcnkd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/ggmlgcieb.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gknsqhepg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/ghdyqvhhd.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gqyticaff.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gpnvtnbkm.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gowmhcgmh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gtnufyhgt.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gdvhbvpug.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gykzbmfid.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gguehtmgz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gfwlndmdk.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gxbymogiv.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gzuvpqktm.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gogfgqjkt.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gvrwwnezm.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gqlchuzth.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gtqjkblwn.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gldqcmhtv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/ghgerdlep.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gstymlrtl.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gohfixepy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gvgtsuzqr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtjyvanyj.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gbsljjijk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/grsjiikxj.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/ggnmjbzuo.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gshnsdhdp.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gviwgyknz.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gaefnxhiu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/ghtnozzyv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gzwkvsapr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtawdctiu.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gjfabxcvw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyazroivf.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gawmwnabn.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gzlxzbyjx.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/ggwjhjvme.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gmboofdxh.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gurbnviex.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/ghdbkotsn.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gzimfkcri.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gritwvypd.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gbyfmlyks.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gbssjykar.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/grycdzhtz.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gxsuurxna.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gbmhopsvu.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/genionmbs.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gsoywvpel.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gnvgmaxzl.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/grdasnqcf.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gisnrkrcc.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gzizykrwe.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/ggefjkwvc.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gdqbmcchk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gcxrlykzx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gxehgpwar.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gsbxyfxen.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gznmosmne.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gdedqdvnv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/ggfyvrmgc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gbddybyud.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gmoiwdpev.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gyncnsrxh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gmwoxzoji.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gborajotd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gjnyuzrhw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gkrcutfgh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gkacfyrac.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/gpknzjbpl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gzzkraipc.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gnkvqjtbq.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gfaeebvyx.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/glvxbvjqz.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/grxbvtxqi.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gkkjqjxcb.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gxsexkuyk.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gaapetdme.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gzaqybtee.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gboecyjek.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gfdybrfjk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gvwhwetds.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/ggoicifvc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gezohlsfm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/godyrolyq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/goxeniwcb.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gfpkyaxeo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghgjmpepe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/ggzhlpdkx.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/ghjnhipek.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gllfwxemk.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gadaxrwvf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gqherrito.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gaerzylrd.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gruaiokus.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gytxorull.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gzlcebfhq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gbxcrzsfp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/gsygfmspn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gnbnouljf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gyrhgnlmp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gpqfsqnjg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gttldqrvc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gsmahkcog.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gcriylaca.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gzzxvzhef.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gccjlvpsc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gkhieglug.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gplbimdvm.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gtzgwdtde.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/ggdibtfhz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/ggyiberar.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gfctisrol.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/glvzmbddi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/ghvccfory.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gtfzahvfv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gigwtqpki.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gmwypfjum.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gairkvgvm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/ghtgjwuzc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggfswkhnj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdmuvjlqf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gvifxpqqk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnrgbnfxm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gejmgetcm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/ghulenuzc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gnfqnyrzb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gsczbkswr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gefjzdbze.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gpziuxims.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gqgxfvtps.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gchycokqk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/geklqubrf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gcuzsygxn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gotjbegae.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glfdsqszu.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gejgfdslg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giwfzfwsw.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcnxlyliy.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gbjafzlkw.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gfhqepift.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/geqssaecd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/goczwobif.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gvhtpxcir.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/ghgpkelkv.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gqdypkqgx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gzgdarlqy.sHtML


<!-- 参考信息 -->