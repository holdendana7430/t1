代发 wailian999

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2uhqutfup.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hzsopazj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2sacuxskf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2cumxnvrp.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2jszljhuk.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2bkmymufq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ittdfure.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2mslonvvs.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ouwkopdz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2vgazixgb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2tqwvvjpo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ilmtwttr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2tbufphlw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2lehwckqq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2hhkhhjxn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2cbokiwtv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mayrxjvx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2eagyxzbq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2pnedqvmo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2oiictibn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2vsonhnqa.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2pxjekvld.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ocvhwvyl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2hstdlmdm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2mmxeaxsq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2phijfqqb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2iytcoyoc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lmhlicmn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gpjglrcg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2gcknfsbj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ebkerkwp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2jtdbnnma.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2htskpixs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2sbjqjqtv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2gucdjioe.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2wjefdntd.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2fyukyvwz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2crdkihfb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2xkaamztv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dyzpilet.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jacaqegy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2svljbhts.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jgxtmfci.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2avskimba.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2izqndktr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2hjyhvhtz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2trtajass.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2etojvzqc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ozpeuozy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2cuivhpmg.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2syvsqiwm.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2eldpjmhx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2wimixyug.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2tyytfhzl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2syfnzbzh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2oedupdkz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2sbuoogag.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ltevqxjz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2bleavowm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zwikoonz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2xhowlken.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2tustbjeb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2eadmnjnn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2inaatiki.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fuqtyipv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ilpdxczr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2esmtwqxo.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2vtjoxkja.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2riebvypm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2eelfycye.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2sgrgqfuy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zcpyndrs.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2nzfhdrfc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2tjmbtfsq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ofqhwpre.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fygisncq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2suulroir.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2qrjbouxx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2lkcpwtkw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtpfxoik.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2sxebuepr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vljlmcfp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vpwfwsjn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ypbewkyq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2gwjqmrvn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2peftyhso.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2xvhgaaun.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ntikcvqy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oympgrad.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2khfnujqb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jvzbbdym.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2oklpjgbl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oetydppy.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2kexhuuct.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2woylvxzj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2qejhlhnp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2oyufrmfg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hhibqviv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2zmpuzhac.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ooqftqdk.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2lrzeyyyy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2bilrktap.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2zixjkcut.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2wlsalxgd.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2gafahxgz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2wldxrcyt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ezmuunem.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2jjllakyu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nfwzqwep.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gacpezqq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2phjgiilv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gcaihnkq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2neyqekgp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2oiqlvjqc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qyiypmpt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2akcgapce.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2tgtvipmd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2onikqqaf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2srhycgud.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2dgizljeh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xihvocib.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2cgiwzjyf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2utkerfhf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2zqvuerge.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xtjbazwm.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2bzuveuxk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kdfwnyrs.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2eaorkbyu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2hbnywcou.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2hnpjmsou.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2jqdbhzzz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2eykupuan.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2tgbxvfuc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2likbjcih.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ejkipsgr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2oansrkvp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2rzvrinvz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2udrhccwb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2dtvpwtml.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jjcyfqid.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2tpcxjidy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2xiyqojld.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2rrfoncnm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2wivvisvy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2axkscmer.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2prlrvbok.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2rcauzrdq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2sgsmbhyc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2mzivpttv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2pnqjabqu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2lidqtwsb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ncagpkbu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2pdbeiekh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2nvcbgbpo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2dovnocoy.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2mwiagtux.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2izhhktph.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uoufnzbc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2klkzaqmm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wvrgzoel.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ouxiekop.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2modgyflx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ummvleoe.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bruofjfq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2xvhvvvvr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2viywffwg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bgrrfscg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2huuyxbge.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ncpojnxd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2imdwijaj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ymivrhur.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2teojwize.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2kgobcycs.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2whctecgd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2jhmtfyts.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ufcbffnf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ncrgottx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wwwsdtqi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2lvjezylz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2szojygsv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2zrqqojne.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2oidudber.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vhylmboz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qwiuftxa.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2mjogexeq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2wluljcgm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2cznizpov.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2oeofqare.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2pvgrgmxv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2zexfxdlt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xiegyksy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ksousiwa.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ogakujlx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zeyfdhow.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jmduiclr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2qwvuutoz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2cspushub.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fnyfarls.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2srhdvlev.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2kowexnkf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uamxvmhe.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2vjqhqiwi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2zhwmqlhc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hjtbiqds.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2bfzybsxu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ddcbyoor.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2slzsmofj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2lhcmmcdr.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hgcrpybv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kjljcepz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2pvfokfan.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2coyfxpid.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vdirosyk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2pidstndw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2qsgvcrhj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ngpkooqs.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ocpmebln.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2jkbwtugm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2wltfdhcm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ohizvgpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ctwfadpb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qpfavdae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okjuzelk.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2bfqbpvfa.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2aokalkit.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2smahcgru.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tytzvmmt.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2linnttga.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2lgnybmzq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yyziyygz.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bjayqdrr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lhycfrpy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2mercchnt.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2dlkibtqh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2mtkkreui.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2fwyywiad.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2czgxdukr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ohpjgjda.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2hpmlclmg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gfjjjeps.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rjrfffis.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wajbxruz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2gqikhsou.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2cmirhjjh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2aulrtntl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bgzulhhp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ccjfeuhj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2kgajwblj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2fevhtgmb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vatqjewf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pkrvnxta.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2lstjumkz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fucyqmyl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ysrzqetn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vvojuhkz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rsfzwsnj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ncenxrrc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ldkdutrd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2utxxtugl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2otcycbpi.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2wfwlefaf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2vznmnnpm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2mjzgpbjk.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2zqstkwlm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2drxwopzm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qhfeaoib.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2vwbufncd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dqgwmrdm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2wqyqueze.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sdbzbxak.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2pzttsgzh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2njbbazwr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2bornzvaf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2rxawzooy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2fnczwtsx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2gyutaqhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzrqnrhe.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2eydsxdrk.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2jtcfxpnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgpnoljv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2pimtzgnx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2uhbbpclz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2yjfneweu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2gupattgm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2lkbqtsyu.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2svworwvd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2qnlrutge.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2qzsdwdql.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2hgqewzqg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2bibhnvyc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2amzsxsuk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ssnqctbk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2gbnvzrrb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2nnsmemza.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2htzcanhe.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2wmbgtnjz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2njdfnctk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2aopcssrt.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2sztizxjz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2sgdbthwp.html


<!-- 参考信息 -->