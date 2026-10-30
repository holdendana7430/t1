代发 wailian999

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gknbgubrb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlduwtwi.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwfzlzwz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ginwrxauf.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gqbpvrysr.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gxossofsv.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/glhqeecwx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gohboqvbc.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gvgojvpok.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuwerxdp.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gwvwfozgb.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gpwraplwm.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopcpmhas.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmakbyqqr.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnagvthj.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxxtxhqr.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbjbkwwi.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnkgelxj.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gmjkfxrwp.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotvgmtnx.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkmkitwr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gejtrokov.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsguajwax.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gtoorakja.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmxchxfm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gungjdirj.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gtbefzpdy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldzxyctv.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/guwpabgrf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmccvtwx.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/grmuphyrv.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gbnfiaaep.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gjxafmyqu.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncreuino.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gmnjnglea.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gbpbihwrd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gouldbsrl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwonvhih.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gyiwapxws.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gysmkpucd.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/grovtermi.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gjgqdtdiv.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gcocccmbe.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmepnvanr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/goyxcmcab.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqqnsuzhl.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavyvoems.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gcxyohlcm.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gxnvubpem.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gysluowly.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gbzrqxalg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqljlmwa.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gldfqkojq.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/gspozoqcn.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjjqrdkc.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gdmdizocg.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvwpwqxt.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisfiqxwn.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblkdotfs.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnjbyhds.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gzinmpiyx.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/geszvbyfn.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gswwxpzxq.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gmnfdoiog.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgpotgpz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/guwdfyifz.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/glulkqysh.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeyfvmah.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/ggofpfcbd.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtwqjcou.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/goijkbwcd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gyhpzctsy.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gweztmbfb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbymphzb.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gywmvbeco.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gqcdakvfi.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/goxusyyrn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gkqvxgttf.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/ghauxbrmr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gcoespexi.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwnythar.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwnyakpz.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/ggmtajukk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuvepaem.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gslbghebv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/guewdvoei.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gumrayrnr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjixvbhws.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcihryll.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyydbyzj.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gwxbvrmlp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gedbuqcwi.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gawcygmbo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gkdbypkco.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gainbvucy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtosxbcik.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gxpjujkgx.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjrkreom.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryreqggs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmryktmr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyoiavyo.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gtkibvdef.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gojlgpgad.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gnktzmqja.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseywmvyo.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gaggyxpps.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gvmekppdf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmrkycic.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbhgoomc.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbpqzqzn.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwsjblho.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/geyebvzyf.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genuwwukq.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoeutwvg.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gnuusmssy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gvppahfdg.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/goixurqma.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqjwyzob.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdiooecd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gxblmssgf.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoogxcin.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gmntznaqo.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/ggkescjdb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gurethqmz.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsetpixz.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqdraslh.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gqictrrlq.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gcaerwyyf.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gekdnfiae.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxvmfoyr.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlgflpxm.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gavxjpcfj.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gjlmcnhtz.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/grxrbsnba.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbctqpsfp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gousphpgp.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/guacjnvcy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gbhcsuyac.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/giekmbjvb.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gvparkpmr.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gekambbfl.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlyzwqml.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gthshgxjp.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwoowdjk.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxsmhrmm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/giehljmvs.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gxyktqpjw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gqtryippi.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/grbloticd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtwhaeuh.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gktwuagdx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gopqknlon.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gybfefnoy.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqndulox.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gdsjcctff.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gtpqpirkl.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gsxcoxrsi.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/grpnndmwh.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gxknrwrhg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gsdgeunzk.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/ggiiylvqt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfkcjqwv.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlhlxpyf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gtshosfet.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqvrzilt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gpsilapko.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gnibwauld.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmwqteic.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gayzaecyu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfavcsrma.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gxvqnpnas.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtrqlcyf.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gyntxqxvh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvuvacxi.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/goyiljubc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwxqzjrn.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxjykmmm.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqkikjub.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghshqwnhr.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxywzstl.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gvtopgmem.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlcdgezy.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghppcczec.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gnflgkllg.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfziffvd.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gzemsbyyo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/grbsitrzs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gakioidaw.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/grwkqyaww.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gomqonerg.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/germxejfq.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfkwetfp.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsptbajz.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gycfqsuos.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljambxcv.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gmvqfglmm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfmnkbagb.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuyotbjk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyrukshh.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gjoozkvjs.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdndvpdz.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkmwpvqw.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gipdnlwyg.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/glwayyrfe.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnakiunmx.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxxvubjm.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/guxmsqtab.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexydbweb.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgrtndrp.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkbnhdpt.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/glnvoetiw.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gremwacvg.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswjbkxyd.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqfyqosi.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gswevhqkj.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/guhlmqids.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gzdxrifzx.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gynbbdnco.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gxqzypfqw.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gjizbouxt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gqosypvkk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdmhamlm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpfgtuds.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/ghinwspzn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/ghdptzydv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gonvffmmy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gofqbsive.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmulkmup.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gdnqrpkup.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/ggizsctol.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvotgqhb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gadfllmzy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gyjwjpzal.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gafhsjulf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbvkudna.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnujqnxmz.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gjtpolkte.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjqaodhy.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/ggforftcc.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gcrqhavaq.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuadksds.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gwozysgyc.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwrbnldj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gttdwlfhu.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhwqsotr.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gxbiiqgbe.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyntwoiv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/giqegdqhk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gxkspdsku.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfekzahj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gqaovzgke.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/ggosnojtp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvlthzzl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnbpauyl.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/geejwayos.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvvlatnk.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbenxrbkn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnccckwg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gdujaxaqf.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknfppsqv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fanxiaobao.xyz/Article/details/gvealerps.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gypbzxdon.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/geyihoxll.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/gvpukehyb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fanxiaobao.xyz/Article/details/gzpwayemx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fanxiaobao.xyz/Article/details/ggejrdjkd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fanxiaobao.xyz/Article/details/ghmwgxcpg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/gohkpnwpy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fanxiaobao.xyz/Article/details/ghjtzfagu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuhvkqed.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fanxiaobao.xyz/Article/details/gkglmuojk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gzfwwphbu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxruhodb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fanxiaobao.xyz/Article/details/gffcdnumc.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwncdirde.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/goanuaubl.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gotucsaqg.sHtML

目  录
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpvggyfo.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/geinpmrvk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggllkibni.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujgwcqry.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkbvfloq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gokrrqvsu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gctkzjvsl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gvccyhaby.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gracjefbu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gkswfowyx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gcxyeiczw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpzxnawp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gpidrnsls.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkcplincg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoisvbhd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/guevbbity.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gousdjdhh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/grfgzvulv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvvgueak.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gcazrgqrr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqazefjt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvsxykxf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcpcrkna.sHtML


<!-- 参考信息 -->