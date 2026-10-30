代发 wailian999

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gmjluerdp.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbljtlgcy.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqztmcgps.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfozitkx.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glygzduzv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gytvohwsk.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gcqiwhvco.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gosdndqlk.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldmqgbgq.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyioonxu.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwauujai.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/geizyzmjh.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gxpyhzurf.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gqzljqwyh.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gulbiayao.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gifmkqgge.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgqsbxyo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gcunryvxn.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjebfobkv.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpftpcwsv.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gbwlgjgwq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gkavqvwmo.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gsscghvzj.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnehlwid.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhnqiwgd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdrjqeoe.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhomcwoi.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gwmkxqhue.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspudjjhs.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gjarohxtr.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/grdjcytrl.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgfglqsc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpawpuenv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gdtgeglmg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfrlamzk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gpdcivtoz.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gelwsqsns.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrpypptv.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/grupqturw.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzvniatm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/glutgwior.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgjogqht.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdnemdwb.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/griqnqifb.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiighebw.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gakwyxpgu.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/ghfapaxii.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnlpkkkhi.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gcmtzhvhq.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gtkxnezps.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/gxilaexkp.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvarkmzfm.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrkrrcsu.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwtrkftl.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpigjfxro.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiwiagfd.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gjervtjaw.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gczrtjdev.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gejuzrowc.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gybtupqcg.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gqxyngbig.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gobdzxnts.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gxehjqcaz.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gipvhfpyy.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gmgtpvahx.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbwizfvy.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/gbrgmosfa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajmjmlhj.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdxjpskl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzlpysve.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gztuhiuil.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geguffaxs.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gswsjfrtx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gavdknknw.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhcnmbzl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtjyvnjb.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegwcpoyr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttxlljcy.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gtehjfawx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjceaniw.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gbuwamjlv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gatcoeagn.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gaapxslnw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhvhsrai.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/ggvgekjmk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/guhojifrx.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gdweqadfe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gduplpdrw.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gvrkdcglg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/giacxknog.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gayenrrag.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gspgzzuqc.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/geyrwvezh.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/goqnfjbvj.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbgpgnyr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakjifnrf.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gfbrgdiuy.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/glsrmopij.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzxdlqlo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyfawkgn.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmnrvrrj.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gphndjndg.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqyswtvo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwldmpss.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgphqbwx.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/girgfaipa.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gipkicdlc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghecxxprg.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gynwvczdo.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gscsqfatb.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkubudvdr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gdzzjchbj.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoatghwi.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gdixfccky.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpmtpyih.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gxfmnyurx.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gwzidwkwy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkmzbeyq.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gtdwnrlsj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtxjjtzj.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhhhgxio.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfymnzef.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gtdhpztjy.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgerlglu.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdmtfegc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/goqmiwcoy.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwmmunvf.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gllkqrvga.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gdnutinmm.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkmfjypo.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gdqxgxwzn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzprcmcuw.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gauuzokwz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/glucgiqmg.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqglcijzz.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbexgrvmj.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnmarxzn.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/glnhxjarm.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gasbzcybh.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gumfwbgye.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/glzowajsf.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gmebwefms.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gxjqgfcih.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvkqcubx.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gzfximxvc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gcalhnbuy.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/giyedaqwy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gltkgtlwr.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gimjpbtxx.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/goeokuzjg.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbroiopz.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gqkucjmhf.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/glxhznfla.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzhmmjfi.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gqstzjpdq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gigwchbdf.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gskfeiodb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqwhgxvz.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gsmffhssz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhfneyjx.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/grwggoypp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gzxvcqsiz.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gplbnkwbp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gmvqxrbnb.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gbpqomxqn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gucixlpad.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggihwzwqe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/guwpesjlm.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsquswjh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdguskwh.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoyrfswg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gookosrzd.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gnimzziqp.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmoaidtx.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gouiywrmu.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gecorxpfj.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gekbsvugh.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/grcgxitos.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfviqdgn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gsbzuiuco.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gwibldtsn.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gglsvyrzs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjflnqtfk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gaixnizai.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gxuhxqnuf.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/ggplbhmzm.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godeohebp.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gmdsrnpwz.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gdqeptvct.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/grslbvyjw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjcyxqqn.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gudqxntry.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklhtxqvh.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gzagvagfw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grnbuwile.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gnplzczpu.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhqadhbu.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdosqwlp.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gmehcrycp.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsseznof.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/ggwxcugit.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/giqiewjsy.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwoderoh.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiscxkns.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gplhajznp.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmqtaubv.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gahfomfxx.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/giphfolsn.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gtvfrevpk.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gujynkfzp.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnivkuxv.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/galyyboxw.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxtgjzql.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdbdlhhh.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzvyyujd.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsljtgha.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gtkozfjos.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdqvycro.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbuakuyd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgzmyadh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/glhgvdsxt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmvaypqh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqmqgtuw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwgbhfng.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpgndkes.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gxmfgtzls.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/glbggtlhy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gapofpxoe.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gruqpwpeo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/grxygcgwo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gsekvjfqi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gahpbuobd.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gcbpgzlbm.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/ginvzixmp.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gfnrzogwe.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/grmjrdggp.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/guqmdelei.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gphwgapce.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gruarhuar.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gkftxurti.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/giubjmvoc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/glxacxqxs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fanxiaobao.xyz/Article/details/guignszsi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fanxiaobao.xyz/Article/details/gsxhxivlu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjcotvjw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyhvguic.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggctaxver.sHtML

—— 文件结束 ——
来源：http://baike.fanxiaobao.xyz/Article/details/gfnxzkrpn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmvwcvov.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflvikbhb.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsqbiypj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/giwzjimtn.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/ghadkrjoj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqbarbwa.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/getyplide.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbgymqtf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gprzugbeg.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/gngothnbp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fanxiaobao.xyz/Article/details/gebsyjzxb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/gmwkwcoxa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/gpmmmwvnl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/gxnhyesjq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/gppvojriv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhktlrck.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fanxiaobao.xyz/Article/details/ghxcwsqcc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrhdxytw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fanxiaobao.xyz/Article/details/gurxuijzd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkkuutqy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fanxiaobao.xyz/Article/details/guijoorre.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fanxiaobao.xyz/Article/details/gfutuguuk.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gibiodyyn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/grzuksxoc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobilnzkf.sHtML

目  录
来源：http://blog.fanxiaobao.xyz/Article/details/giwkcsvsy.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoztisor.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gevqezhei.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyolfbgxx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gjckqsxrx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gdlomxraz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ggmoeonwh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmfclrwf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gnqucebuq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gblobuelr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/giptazsoa.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/grffqljfb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gokjozrxw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzjwbtwe.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyywygyln.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gijomespb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxovcjrsy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlszjhvy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gcxmompnb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkpobunnv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gvpmhjwvk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhddgbec.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqoznxrz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goruanjua.sHtML

A. 基础语法与类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcedyapi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsockmmc.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/guwehcchi.sHtML


<!-- 参考信息 -->