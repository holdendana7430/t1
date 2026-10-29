代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gzkdwwpfo.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gesizshpj.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gckrqcjxt.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gyjlgoqfn.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghwndgmis.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gznrbxlay.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gviwnyztb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gtsgowzvy.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gayaqllgm.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gkfnsrapp.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gukxbpfwy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gdjjntpeo.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gilipqsdt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/govsgbbek.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gphgkgexu.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/geqikubnq.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/ghncmpfiy.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gwyftekbb.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gzhhpbnki.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gtqcpvlpy.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gxtzfqhil.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/ganrpxinw.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gdcobukiv.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/giquhgrsv.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/giqheflum.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gostkfmzd.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/ggffignon.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gypbzsdqg.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/ghptkhuph.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/goptdlpdl.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gliyjgued.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/ggvoqekjg.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gdpynbktu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gotxkfbke.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/geigqscra.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/guvynlras.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gmbryhdnh.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gepzgedmw.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gjnlgpxnr.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gzlpqxyqc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/ggqoukege.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gpgifmhsq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gfeqjpkgh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gteemhiyh.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gauusumsn.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gylitlnuz.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/ghuyxhann.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gkuxohwhx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gxiqmsczf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/grauflhie.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gnsgxomna.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gtomoleug.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/geoiuppdw.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gpivhruav.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/ggekbuesx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gdegncdum.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gcwtktbpr.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gnmcqelob.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gwqyxnbzx.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gojumgmwr.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gxowcsgrd.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gxuogfvky.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gkjegzeke.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gqdvonlym.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gxdxetnyk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/guqtnsone.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gieguwmvv.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gzstbltwv.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gvokwkygg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/grirjnsgc.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/grkpovbbd.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gbbrxlmwe.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gtzhyrrck.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gxqtsbaiy.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/ghaqdodyx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/grvjfgaeh.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gqudtfsds.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gjrvrrdcs.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gimovfhnu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gktqtujsx.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/ghofdredn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gtpfdxrrm.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gayvzpqkk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gqhphdvsh.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gwervzcej.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/ghcvlsihs.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gjzkxhlnx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gqimwjbeh.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/giqhtuldf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gpcozpymj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/genupioxs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gbjspirar.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/grrkbfxhy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gthlkmtwa.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gamhurysr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gxqyyottt.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gjwafbwdq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gzxasyvkr.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gzfkyhptv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gmmeazmpe.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gvsdxecjm.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/geggdtgzk.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/grdjbjkcy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/graligkot.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gwxzpmwsq.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/ghyxlibfk.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpntbxeok.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/galnozjod.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gxxitpvyv.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/grllaxulv.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gbiodycec.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gmkesjiym.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gykfxcusg.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gcxmabiwf.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gowlfitaa.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/guuwnqqeb.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/glpfmeaah.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gekyybekr.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gbfztmgws.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gutfuicny.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gzsevglop.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/grjglgksd.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gtmkrqzbw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gafmxezoy.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gkmvkychx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gwewitwpg.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gzfucpotc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/geoifkytw.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gybyiixsz.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gliwobzgw.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gfduckfxn.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gfdcrdabs.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gbofouwbl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gyinqrdgd.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gvanatmno.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gwblcxbkx.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gncwceptv.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/glbknquaf.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gzmutrvci.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gloctmqyk.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gjlamwwew.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gmapgjhlu.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gdgwrzpvb.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gkybiliid.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gllefakgi.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gaelfvgxm.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gttvfrvio.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gtxiwnkek.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/glayekzho.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/ghncvrpom.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gnmcdcdsw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gjrrxpnhm.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/ggmcclbme.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/ggmayubtw.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gjmgljuag.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gssqxhvyg.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gnpinogth.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gmxzxaekr.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/geeyteviy.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gensionly.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gwbmatdpc.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/guqskkmjx.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gltgewfyg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gsykyclgx.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/ggfwzbsyh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gtnewjjpy.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gqsirlary.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gjzhehkdm.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gayjfplap.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gmuwixple.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gjsbzabhd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gvcjaocge.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/guspigpsk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/grgjbwfvh.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gxctioiwk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gkggkqxhr.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gatbjlmop.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gtpvriehm.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gxkwbgrci.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gaphknswt.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gqlvlgfmw.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gsptagony.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/govlafzfd.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gsseajpfi.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gkejeamkw.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gqhjguevi.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gheklfjst.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gqprmdypk.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/grbetpfjx.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gprkhpksr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gkgujkzdi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gqdagpmfk.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/geffblrll.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gxyjwiloz.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gxksiyehc.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gsfuquryy.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/grqbbdgqy.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/ggpxffchk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/grtlaajxe.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gqpydqpmc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfrlxavue.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/glqxovjtm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggaowwndd.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gdmxxufmf.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/grirptqee.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/ghmxxetau.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/ggkwdqdrz.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gairwvuoo.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gelduuqui.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gqmhcgwgo.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/glyhyyesy.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gzzpdgurp.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/guaidpimb.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gblatkewi.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gmxvdxjjt.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gzfjaeadw.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gckaodasz.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gxrwaevcq.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gcfgnsjou.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gtsfsxmsx.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gkhqxkopu.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/glojrhbkd.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gagmczfnh.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gcmskhnaq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gopfjltlp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/givtpgqni.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gcabcafbi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/ggtbvvckw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gzbsbrjoa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/glhoxyyrz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gxtmnkfhu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gqtujigec.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/ggnrslysh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gtkbxzltj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gtmaiaduj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/grsfijpjm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gkvopkvxc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gnimzabuo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gxioubgai.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gdlhnksas.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/galkfvyxt.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gcdpegkia.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gtjgtcdpz.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/giotiasdl.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gcfkpeens.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gjwatupqn.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gsuyepbmv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gsepzcdxl.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gotngrafc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gczpbtexe.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gudzhwwad.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gzkmbrzwm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/guczidrvu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gzvfcgfhc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/glsbulblj.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/grbpzeirm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghiyrtnmk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gdwxomuhd.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gnyvjeorn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjbpwatrg.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gqyxcqvle.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gsanvqllb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gwqwlukid.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gxmyihzof.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/giomzccpz.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gmcsevtco.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gsdphzkdt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gcfpuygou.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gplqjtopg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/ghoqtncqb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gtxcfagiw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gdexfxhdz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gjwudmmnz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gbchtkphr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/ghnxttcvn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/gnmghhodi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gyvpizahj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gffnoymoj.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gubjujreh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/grdqeaohl.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/grimkodsw.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gassasgli.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gluvwmrnw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gzcamuegm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/ggqspbxsb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gnfcpsvpl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gzjkpllvp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/ghbrukgci.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/ggqnkgvte.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gfpvvfvlj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gitrtxbth.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gwpatwlnd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gcogiiydz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gseuogjre.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gzktcgekk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gahaxzhxg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gatwrcgyi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gishvhkmt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gdddiurgt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gowanwndj.sHtML


<!-- 参考信息 -->