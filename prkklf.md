代发 wailian999

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2qznadvvj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2myaeczxu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ewfezbko.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wdcudqsu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ayotfitc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2sywrmvfz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2exgpcucw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2spavrfgr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gmzlimtr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hfugioyn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2furejucy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2rfwnuqat.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ptrinnzc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tsinpmqc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ebndozjv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2vdnvadgl.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jmvglkfz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2kyfgpqzu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2izuvyosn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ohsnowge.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2uphisflf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vrckmprn.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2zjapppph.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yzoftnfd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2yrezbunf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2iswpnqna.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zqqgeaha.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2frskgqwk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2kykexpzf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qznsdkmx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2xdxonqvj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2zsypgwft.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lhjjxyya.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rpzgmqam.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2rlqnivkq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kueoegyu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2yuscczjx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ymtptgpf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ntvqsnaz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2hojnvlhm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2qyujmqhy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2lxpdhric.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2pszebktn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2clcafmfw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2dueywcpf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2rxpmvyuf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gfpmlnyx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dvuyvfmw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2cyjsawpt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rnkyadwu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vkfdzdbc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2wjtqkkwc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2comekagv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2sehdibff.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2jvgizuot.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2aijgrupx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2smvnvbql.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2pyvpfhqm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2nbdxakxt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2xomapymy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2zeyxcgvd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2lflyihlj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2tzlgscat.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2glyysair.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2uuonaura.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2jcybqldm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ufkvqdgv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dzoorttz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2jszunsee.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2idhdylkn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2sszftfal.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ndlxecjl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2shkosbzw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2tgclmsil.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2kqhmphtb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2fmmcihah.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2itfspszz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sufufpkx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2uralrtne.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vojqzejs.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2koxbmkez.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2hzuxphdo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xqucpyof.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2whedncbz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xdysojoh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2vfxdwwgp.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2niruknma.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zruzbeib.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2awynchou.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2zkwplipj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2djrunubr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rhyeyart.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ipowiofq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2kstcgefg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2yhiiakff.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2amxftfsc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2cqijfyhq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mgbtcgsr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2wmyvdipn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2woeeemaq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fgcvzace.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2bplhjthl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2udmpjfeg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nqaieusn.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2csklgzuf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xvfejoas.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2wozhatyv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2unsngfuu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2breyvlxa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ljujihri.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2czzuzrmm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2sttmzjdr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2wmzibgeb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2xraqglte.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ivrscoyv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2dginxtjm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2knqyqjid.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zxuywgox.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ritqcrkt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2chvgnyvd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2guwgqmrg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2vorlflzy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vrpcxqdv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2qazfhvhg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2lepivsmc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ojabrezy.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2xaardcpq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2stfqzvge.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2goaiiihf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gagjosho.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ygowwkno.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wfnoodol.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2dpbrsobu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2galnyyhd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mxxyanam.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2qbxfakqc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2hsmgwdyh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2htfeknzd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2xvfjtzzn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2jmumhagl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2dqysnzyk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2jotlixvl.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ojkcgjui.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qeoaddfz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2grqltwrt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2djjvpxxr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2txspuxrn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2lunwfkwb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2voetblln.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2mnxnsuzj.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2rvazhooo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2nljqonhc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2iuiyyhnv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jdtzlzaw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2cpcxkdyx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2iifiirou.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2bhprwbyh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2esylcrwb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ccalbnxq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2xoqtjsvp.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2uxulnhtj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2viqiurhz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2nigladby.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2vspcfztk.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2qvhkgfdi.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hzqvdomy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2benmists.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xrtpwsub.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2sbramxft.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2mqccntqi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ukcsiukj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dcfogemy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2qqaqldxh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2nntknejy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qsdsqxvb.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dxisrofg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2xpntdqoh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2aysjzprr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2brckqjnb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xwadqrvm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2jbbieyvq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kgcrpfuv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qqcckqoc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2dsxxlrbf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2sudcfuln.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vuzywrls.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ikeccnfk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2mbmsvkwh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2urrvgaqq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2gynogmnr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2iboqtxki.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2bjcmqvhz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2rknrdifw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gwufpoad.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2wileatmw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gknyvxor.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2dndyohgs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vhsrqukg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eoyufxgs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2objvckmw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uxzbcgbn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rinyhtua.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2lbtjyvwj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2cozhcvxj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2bfmyyqmf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qujvwxfd.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qgwobuyl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2knxzunmg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zvjbbxzn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ewwvqtja.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2xnwepusz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xbjuwmft.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2uowjjadg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fqgmqgah.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2toiticuw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2aonbsnyu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rbxayttr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2epsxynrq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2oydyesgl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2zjyonsib.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kgcivvzr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2xafzbzgc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2tvxmdevg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2jxavavpn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vtdcdcpi.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2cgtvajit.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2rgjnckjg.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xmoxvldo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixxcxjrq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2lvonaxtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avqebhuh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2wxepnyag.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2yrzrkxtb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2vczkcxcc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2iloxngbd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yprdkqoh.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lahfcuae.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cfeynqhm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bvumzckd.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2emqxiwdy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2hdzgywwh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2hvrmmpgd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2hdvapeuv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2jabvzowg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2vcieesdc.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pqarvkxe.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2gfzkhxbj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2oomtoiqd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wxclmudp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jcvjijij.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cwcwnfiq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2giefkkax.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tmsyrjgz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bdjpymhz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2cqoienda.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2eubaxops.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2oqsikxxj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2orscyici.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2azzlhwoh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2iidxjqnk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qywhtvgn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dzwzzvgk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rmgpeixv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kdnrriyc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zexpslnz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jcvomqcz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2rcyivlij.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zkxgadft.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2wnshcmfz.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xdhwkwuh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wfkabdic.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2lnkmouat.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2vmjcfpzk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zkjbbxyv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xbufszda.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jguwuvub.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ehdrrgoc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vjmwlvra.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2zrvtvxng.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2bcbuamuv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2opflwoiy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2iztiupye.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2vrwvwxvb.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2kpavxfgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2inqiqkaz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2lbrwfpdz.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2zwhraziq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awxcopnf.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2mvfyjrxv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2wfgvuyvd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2mhyevxor.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2jqhbpogw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2efsdszpm.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2icftgghb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2glcebmqa.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2lwxwrudr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2nsqqknmk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2cwkqhqyz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2hiihtcwo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2eemmjrmy.html


<!-- 参考信息 -->