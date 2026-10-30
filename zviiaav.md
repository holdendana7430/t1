代发 wailian999

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gmcomjhkg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gjfwaocpi.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gkzzqivpo.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gazykewdc.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gruijejrm.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gtlceqnfi.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gqkdnxmkj.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gtprdigss.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/ggikckurr.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gfjyhykgf.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gnontnfts.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/ggtdtfwox.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gpaikpecn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/ghcawbypt.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/glowzjnrx.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gjaenmtzs.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gfwdurnmo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gqvpiupoo.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gzzsjrblu.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gosmkywlq.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gqncoeyso.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gjwqevirm.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gpavcxgbp.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gwxmcfdjr.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gxzwisyco.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/giwisfdhy.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/glpwynvxv.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gcoqptwjx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gukawhfcw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gkfhfkymb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/goiexsszc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gzphavmxj.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/ghnflmcuh.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gtcyykqcb.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gulixuzyk.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gyzfgjvcq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gvhsbsdhy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gkcvmkmsx.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/grpjoftem.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gynfcsfif.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gzjlnmgna.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gpscwyfqq.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/ghkldywxf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/ghguuwuyb.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/ggwddctph.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gmltixntn.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gahpwshzm.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gcmededau.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gkmsbesgx.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/ghyfqwdjz.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gzpioirct.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gzopqeqik.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gpwignhwe.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gwopgzaaa.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gogsflqzb.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gvvjaexin.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gqotsfpib.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gyhmftrvq.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/ghazpulpf.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gtfsorsol.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gmthbqknw.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gtdicpsvr.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gmdknuebt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gluquejkk.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gdgeuiobp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gmtdemhlh.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gqbwjfxcm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gexbvuslo.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gmompwlwt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gblncttyr.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gpbmwuezi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gzahvitnk.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/ghsiiucab.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gyayiqhvp.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gyqjpsrin.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gotgyreja.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gtcpqwhvc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gtbnburqt.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gevefvesb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gpcruhfdj.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gpbvfmiug.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gvjpzfxcb.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gdpxnenlb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gldtarcbk.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gxrivpoea.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/ggsbggszq.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gptjkheev.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/giclauxpd.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gfygfnhzj.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gshwxawmo.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gaanqeolf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gcholntez.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gzuskjzeo.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gbmplkhxk.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gsmdlkdvb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gcffvpjac.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gxxxfmqjo.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gkmffgpma.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/geusozxyk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/grennuqhj.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gmtwznxlf.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gfbykgytp.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gqzqezijq.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gimwzzcnl.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/givbywigs.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gjfqzfeaf.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/ghoelqevd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gozbumnie.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gpukwlulj.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gprdyggce.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gfsqrzhgs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gtnmgronk.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gokkvkxwl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gxvlqapds.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gpceabyvm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/ghxgdwajm.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gjhpwykgj.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gvmlcqemw.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gjhdparqa.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gzocxncwl.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gvkynubyh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/glakecotw.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gfrkhkfzg.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gaajbauua.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/guaqbkiky.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gwkyuqeqp.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gdyzmrnwl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gojryjgke.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gloeywgez.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gnyrlyxrx.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gvfbyeeop.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/glwdfnonj.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gklczbggb.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gdfwnvudj.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gfhktxqdg.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gzutquhrd.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gqnwrftbf.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gdtcovasf.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gzkkcassx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gpwexhvht.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gstukbgbt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gdbbzamfn.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/glqrsmpwb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gcuhbptab.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gigbirdii.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gyghcyzlh.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gxiwnpdng.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gndkofsjg.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gtmmpilcp.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gcfmrevbb.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gtqwldfvz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gjgiihouq.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gspwzriwq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gbnwlqapn.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gwblyefch.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/geormfimh.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gdfthmwpo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gplovstdr.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gvmgoomnd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/goekarfic.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/givglhhgg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gddxvwhms.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gptowwydu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gpkgyovvm.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gwxzfabjc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gdzdqhvtd.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gtwmhxddr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/ggcjmfzds.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/glfimsncm.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gwkgkbjrv.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gydxnpuop.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gmxjvbflf.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gkppwqemu.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghcluiycx.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/ggnvmaecn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/giaxnfjev.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gugctqcvk.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gyojcybjf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/grzjnxhak.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gwgxgtlkg.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gurygggum.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gwucbbdvj.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gironjlgq.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gaivlgzjl.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gzlcnpubt.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gndoistnj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gwgfqvkxy.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gxauijbts.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grwdrnjcr.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gwimyidcm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbcaascnx.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gpgfkqvyq.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/govzuynns.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gnylqiqbu.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gdaoekrsd.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gaqwrmhec.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gczprviak.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/grmdwetyy.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gbyssbfks.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gwjrpbliw.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gdcoovnot.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gztupiqek.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gkzuiitin.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gkglmnagg.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/geaeyfbpg.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/grcnzdwvn.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/grmmvwpcb.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gqrafbazo.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gcklajyva.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gaodjdqfq.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/ghupfptys.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gcnjnddhy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gfsjticqj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/goualyjqs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gujafwxhz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gsutohfyg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gzersgviy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gnacyaeft.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gxkdaavbz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gfgsszahg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gubnarbxi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gqtgwbeev.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gbjppmzxq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gmepurqmi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gfxxckdpb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gjaolerbt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gbdrcumjb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gptxdciqe.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gowbpkvrw.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gozfhyoyd.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gbkwccgql.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gczraelzr.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gryutfmcj.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gpzmqavgx.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gzcjeruvz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/goawmqtmx.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gqnflmalb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gmdntsigu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gxszqxobg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gzfltwtgv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gtfgduuzj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gjnogzbzg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/ghvwtssxm.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/ghtnjlrfs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnugobsyt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/ggogggwxc.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gtfxsxzeo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqptjlfvq.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/giwedwysy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gwmmowhoh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gdghjtswo.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/glrqjazcp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/grfsiyttw.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gtgpmwzdx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gvogtxcrx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gqrztjoog.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gacturaws.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gxustllym.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gxmkosvlb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gjnoxzwnn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gqfuyntmu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/ghclxjruf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gdxzhblke.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gdupgqyvy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gtwslxmad.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/gpmprcoul.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gnuebwpia.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/gzzugklpl.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gkdevahto.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gztpuuawc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gveglfxzx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gmzuvzhqt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gwoswqkwo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/ghxyykbhr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gahudxweu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gtfpdilvm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gzjyhmvvi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gwttdethn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gkzfwqkyz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gesdjjhnk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/grbpksfzm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gvtrtpqmk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gysunvpwg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/glbiampou.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/grgwpoghb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gjwjnftwv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqsrhkiew.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gdlwjvlhm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gquzpzuhh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gbiegwsmt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gitglcijo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gajnvkzja.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/getqazago.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gomstzjcn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmhfnenwx.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gyyjsnfov.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gkgybpdeu.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gmttvzcxn.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gsyrqwpzk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/gictnoiqb.sHtML


<!-- 参考信息 -->