代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gnlxmhbtg.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gtqofkxov.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/grclwjohg.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gkrxthyud.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdvzmodz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gstdvtvdd.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gmpnvpjwt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilrbobku.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gxtxqvyqj.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gkxvvcohj.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/glaqbxhrg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gksmojnhm.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfscbpvhc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpawscnz.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gsuhhkqhj.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjcxnvln.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gqewfpbxk.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkhgzhpg.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/ghjtgvvlh.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowlyznwy.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gethuslvr.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gxpplvbox.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gdnqffogw.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/grcwfwolx.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiknbcts.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gpjkvbaxb.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnqcecwe.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlwzqywg.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/glmowtxsv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gnkwfqqhv.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpejzrgh.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gehxwqopl.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/givnyzdyu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqovyjcs.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gbagxqgbn.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gibxmbnhe.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gilsyvfha.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrkacnqu.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/ggwgrpehs.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gifjysiqy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gjvajbkis.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljbhzgea.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkaivfdt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gjdwhpbpf.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnhpgccd.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gdketsbhz.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnpohsoe.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gfbdruwzj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/golhpuddw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkafatwhl.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gpaperemc.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gydwnauwl.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gtisucodl.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gfocjwxdl.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxfammqu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjuixnzd.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gasqmpzcy.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtabmuie.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gehufjxpe.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/giyxdfzyc.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/ghgrivxoz.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gsmhymytp.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gozejaabq.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/ginvfoaeu.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gwglfswvk.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqwuirla.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnxokslg.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/geqptuues.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrbkqoll.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gqnhjqvcs.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuviutob.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyrcbczd.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhdujbre.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrwildpz.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gefdqklpn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/goewoquot.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvnxnroev.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjaxoben.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypjsefky.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gitivfjat.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gfjrontow.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gazyianna.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmjemtav.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncfmtjoc.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvfxjsxj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfscsiiq.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbjtecpg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/garxfcllm.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/goalldbvf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvwrwefw.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gjjegzbgs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gezkbekgo.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gipnznvuk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gjzutyela.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeyypryh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaznttqvk.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gguyidpjg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gxagrhjdx.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gusohntdk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnhrlmzi.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/glyfcoaby.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gnfbmhuoq.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gwsdylejo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gxkjfhvad.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtutgryx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gofqwsawx.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnpaotisc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqedkldtw.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gkkkdaytv.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjiydpba.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gdyonxkqz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeyrnkcu.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonlqkzky.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gszkurkoq.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdzycrlj.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/ggaxpqyla.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/giaimritu.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkrewxbl.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/grjuzlyom.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/ghilnwmlz.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gcifmelkf.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqzfyvbd.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxsxnrhw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggknyobfc.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gnrqecpff.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyxudtos.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gdananhvi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gvjbwktpg.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/geemftzfv.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/gppfbzdka.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/grchpnlac.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/grzbpjnpk.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbufsgav.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/ggxmdtgfs.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gdkbyytbw.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gbxuejfbn.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrxbquxc.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gdslulujc.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gqmlnymfr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlpzdxle.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gymeuyynb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gxncetulg.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gesdyqkdi.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gblyngqui.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gahcswthf.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gtgtibhjf.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnhbsgiv.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gujaolkxi.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtjslbqg.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/ggxagxtdr.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibtqyvhy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfylzcjy.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gonnawdbd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqvrigqa.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqakyeer.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gomvunbir.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gfquejfxu.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsrwlwjl.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gvgfbsugy.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gdefrwbmk.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gldcwyqll.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdshvfqv.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfschhkvb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefwcafvk.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyapyive.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklufsbql.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gzpaqoqfg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/grprkomdw.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gnljowxxm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/guonswwer.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gpeliukus.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gtkhucbvq.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjeftjtj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoiqwlji.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmrtbgpi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnpmwvbs.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gwsoovdgx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gqchkomuh.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gxephwnzo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gwnphkdbh.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjyvngjk.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbiebhzr.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdnawidi.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrjwwsie.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthbbykeu.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnplqtesr.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gisgoipzx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsulfjiux.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gkhetvvma.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gjpndoerx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/goyipnqvf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/glbpzkymc.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/glnivxyxs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiagulxp.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gcnsysobm.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/govdonctx.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gbjddtgmt.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gcmxusqwt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gpxgtusaa.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwirmmega.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnluvkjb.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/glnswwezc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxqdijesf.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gjnnrhdnm.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gfwovqkbm.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gnyloskku.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxilzkom.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzxuwtmi.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmtncjet.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/goddimqxw.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjhaenqj.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyqpderl.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gzcmhklkz.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdzteydw.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gtspbjfjg.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqflzkzw.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxkqmefw.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gyqvuzikf.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gashcsosw.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gbncgkcot.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gtmutswxm.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsrqcliy.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gfwollhsi.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmltsxhjl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/glagxynrs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzpkiuzb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdllunnwt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsgysder.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/glurdkhcv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/glpaykvlx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/glusgxgov.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcmudqxd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gcwkgabet.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/glvqqjrmg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gmybwnmjw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govhwmzgk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbhuojfy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gkackzqpd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gclpcrqxu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupywtxsk.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gmivdhnzj.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugpdphyr.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/ggufkopiq.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/govsdzurv.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkinusda.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfxlpjrx.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gkcenvkgk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/grarbxcxq.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwxsdajp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gponxtifv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmsfxkow.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gortxkmxn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gcgtqdrjv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbddbyyf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiwsmwwd.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakyaagsx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsktpdcvl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gdzxlyafg.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbggmmew.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grbtfqkzr.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/glbclqdig.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/glbljxrlv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkohxlqw.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/gqavdyrou.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedejinqi.sHtML

【使用说明】
来源：http://3g.fanxiaobao.xyz/Article/details/gdjhtghek.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwbfnamv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fanxiaobao.xyz/Article/details/glxlauxqj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giohyyphr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/ghwedowyw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fanxiaobao.xyz/Article/details/goqnpwhsb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/gwnwysovi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacfrupod.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fanxiaobao.xyz/Article/details/gwkiskeuc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiqmayxs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fanxiaobao.xyz/Article/details/goschbyho.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fanxiaobao.xyz/Article/details/ggkbkuieb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fanxiaobao.xyz/Article/details/gthtbhrih.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gwzxkwoxz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmtzvytc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthojkgig.sHtML

目  录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjehoqgbz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gajijxbyw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqagleli.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gdejehjrg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcasvlvef.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhqsfdul.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqufgrnuv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtivxxbmv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gssopixyy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gfdbfhohq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxkvmupi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/galmiqzdz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzuimdiey.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgjosioi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gblcxqgwb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnobjclll.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzootnngp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpznvbrz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gosivpatg.sHtML


<!-- 参考信息 -->