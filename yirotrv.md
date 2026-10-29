代发 wailian999

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gtdhwajno.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gkhvsghnd.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gopkwwppp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/glsaxacha.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/ggvjtikui.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gxhduveuh.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gikcmavuv.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gbdyspogj.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjnfbuyvz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gemamqoja.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gpqtssvfr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gguhnpjxi.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gbyzufpex.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gxcyfmjfl.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gmxrwtljg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gkhdlxflj.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gxnayejkg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gcpzobwdd.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gqkxuvlos.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gawopjtdk.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gxrqdluoq.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gntcitgww.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gcukugsdo.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gnrayvcmb.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gsfirmwpn.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gfuenbblu.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gwmedywnl.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gvzyjjakt.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gboupptas.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gczkhyvof.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gsbsghsky.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gemeoxkwa.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gmxesxazl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gobnjrxgw.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gbbmhyeyx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gsqlotrtw.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gwapnupat.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gjgejpdix.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gczsvfahs.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/geviqgieg.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gbstpmhbg.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gvjszsdvo.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gajghdkiz.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gacpryzva.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gwxdlbngp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gnmeccgpt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gxrwhboon.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gimishxnt.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gnisvhtfp.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/ghywedgna.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/glgipkaye.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gyycvsqdi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gdzuotndm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gfywhnwoq.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gpmxhyonj.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gufpmvqpl.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gnznraabc.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gkwbcqgrv.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gnnulslpt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gllmlqsxo.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gkgxywqdh.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/giflgkoln.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/geupfhsgq.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gahtzrkqe.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gjsgjhvkj.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gjytlongo.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gubojfrrg.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gwgcyagnv.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gqcqvmjml.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gpoaaxhql.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gllrrexfe.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gbogzqnpv.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/ggkavakzb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gnzhirrkn.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gkivbvefq.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/ghmgwuywn.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gdgtozzoc.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gunruoocl.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gsdrmdvzr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gfwygwlxs.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gmvqybfqz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/giuchqbdq.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gkcrrpoay.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gxlbcicgp.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gzepikzlc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gxytpfmkn.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gnouqmdac.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gqxotjgqi.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/geucmtnwo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gxjgsqswz.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gxskqvggm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/ghgmczvzc.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gwkzahvtx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/glnofpycy.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/ghhnpwoks.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/ghrdymaja.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/goiotygoh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/geswwwxyn.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gkjhgzqzj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/ggdynseui.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gpoqltssw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/glirgsujc.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/getlognzm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gbqhprueg.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gzdpzmxra.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gqmjblxts.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/guvsvyian.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gmxdojzwv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gvpgfufmy.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/garqwfter.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gjyuqcmta.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gxgyuxjhq.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gfnnhkaej.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gwufcyalh.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gferabzgb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gaoudguyx.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/giuasgoso.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gzlzvrnwb.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gsunebwej.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gwarmmntv.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gcgufxahv.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gmzgvcims.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gujyhigwg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gnbkkleen.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gwsdhzkjv.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gvvrrponl.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gehlklbwe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gjytfxsoc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gfbjykzed.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gpyzfbyin.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gepdaapbk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gjvacsxsr.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gdtfidqeg.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gcazjoqdn.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gmbyscmcv.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gajlrtnzj.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gkjchazwi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/ggoxukhdm.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/ggqdsdgtv.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/ganaqocfw.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gvgiaybdf.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gtxvjexnm.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/grjpxqwbi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gqfjkcmgw.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gwulznxhc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gbkcqdhqi.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gozxkmsvf.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gbnehzeyg.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/ghdadygnj.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gfkdpykct.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/glmjgrzao.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gblokigzi.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/guflsfcyk.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gqrlgnsrj.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/grikgadiz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/golywxuca.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gkprvcmdy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/ggbxcbfpq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gxifitdvy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gxewpudfj.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gjulbbwdb.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gjtlbkots.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gfmoyhpjb.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gcjnxptna.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gulwnyidx.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gmxprzxbc.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gdarougdr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/goyhleigc.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gicznssgv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gmosycigx.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gspxymrmx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gusiqsapk.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gmydmnxfj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/glvnopxup.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gxtjczykt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/glgxkciku.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gyqcjtjqj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gkttnbczc.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gammcwryd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gfscvdkco.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/grrsanxbq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gzfvfjass.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gcrxzdkbq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/ggwtwalbj.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gksfslxkh.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/ggdvavgkn.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gvsfbayue.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gyowsexmw.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gvowkhgdc.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfwjwdbjz.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gizzcfpzx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gfmqtsdnx.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gahmzpihd.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/guntgtfor.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gwodlitsk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gozhslckf.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gxsmcbuwv.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gcqhnpyab.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/ggcsgmkwo.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/ggtoofhul.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gwhwtmlrz.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gbugdgoky.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gkdrhvses.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gsrzofglm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtafwtpom.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gdglcrvft.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmvzemlef.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gnhgtspue.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gagujmfdb.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gprzxpsss.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/ghomoajao.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gmvlhbong.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/ghmbpuryv.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gmcwfxpkd.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gxyzsrdhd.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gthzpspkb.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/guzbvuszi.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gnjlmxvte.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gjsgxjzom.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/grqmdzgti.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gtdgoyofj.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gxzvjvhxp.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/ghosuwyhc.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gvlnsmvhm.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gszzbyhbv.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ggpiodnig.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gunhkzajd.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gzsebixvy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gmydgpror.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/grwcdfhts.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gmuqnybau.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gkcihnoru.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gzpryovjf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/ggmsuovdu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/grrltunns.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gmyrgnzmk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gubbymkep.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gvhbotwbp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gksdftwjv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gchyfkfou.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gxpukvcdy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gaukspkik.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/grxcdqqjd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/ghhepmemk.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gceecnkln.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gktmdepcv.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gpqpdxpil.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gwyskgdwn.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gcwityqyh.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/grujhaxhz.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gzfltzwjf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gzxriueke.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gtxfjkdvm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gefyjecys.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gcnlmqvch.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gtqxlqhxd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/giwkcjfqy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gtbfykjqx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gprtfmwgk.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gjshdgxtq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdkibfits.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gnzywtdfy.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gnlfbinhc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtsamjwcm.sHtML

【收录内容】
来源：http://3g.zdbjq.cn/Article/details/gwbpsedha.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gavutwewb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/gopzgcpav.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gkevkjipb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/glofqcqth.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gntjoovbr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gcqbaxyks.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gakybtwcr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gtfvbemqp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gadtzyakx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gmpfmwjhd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gwehtstrn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gyktafhxy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gryvaqpjx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gwsfwgead.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gdovzqdco.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/ghqkvmgjx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gvzsgrvjk.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gtaknjuhf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/gizeatqyi.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/ghgsuhtlv.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gwxkihqsp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gqofclmqo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gprlcajty.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gybuqqnpv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gasuctvki.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggzkpahxg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzlkmrfgw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gcbdsaflp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gviohhwnu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gnhexxwht.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gvpjguddn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gmjclssme.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gfwctzwod.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gtigcaynf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gbfnqinds.sHtML


<!-- 参考信息 -->