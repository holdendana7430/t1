代发 wailian999

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2uhtogqxi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2essavurv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2sxtvqtll.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wlajoeid.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2sydocagn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2tshymyas.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2osgueisx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ngcltfqi.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2uudrlvoi.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ivgrwxzf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ugwyhcvg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2avoqgclu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ipangvjh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2invpaiwv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2hzrnonoq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2uafmsyis.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2avfimmrb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2bkwfqods.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2jbltfkks.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2laslgjjl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2unldyrdv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2lqfhxpjt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2vdskivys.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qhpqidiv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ppglxtej.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqnbghel.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2acjthdpr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lvlfngio.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2iupyxsqs.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2bltxdkvz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2zrgaklnz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2pkxoyjle.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2gfxwbqgp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2dtiitdin.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2fdnxtidx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ewegwask.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2twwfnzpl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2nhmhmwrk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ytzhdbnm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ywcjxgmf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xiewohaw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2zwfnpwlz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2zujxzeuq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2nwvxzmlk.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mdybmcxp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2kdxppuwf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2sglszrzb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2nkvvplkh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2xjgfvnpz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2lsreuedd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qbbucyti.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2wsimbkme.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2kktfabda.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2peynfilh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ihlweayf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2axudqbfa.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ubfelmso.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2qwatpnoz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dmlhtwqa.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xlurzhtd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2wgkjhasu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mobburog.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2lichavce.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2lrtfucfb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2grgewngl.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2npqggktu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tuwfoegn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bhokfurw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2xkozflps.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2nokzhkxp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2lopuwmlq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2sinyxcee.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xsswjfpc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2tipkqnfp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2zdelvgsp.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2tukpldth.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gfabjoqx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2psvnqlyj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2lmkaakab.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2dwqzqiyo.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2hnferfpy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2yogtlsih.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jkqvbqke.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2apgwkvau.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ijvtzwpc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2hvoeazlo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2lvqnfbzt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubcgyzye.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2yifocokx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2dcarhyvn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2obxegkno.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mpxyvnnm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2missfkan.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2nilwoxti.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2fktrbixt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2zascfxpi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2twcrsttw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wxkojwba.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ztxxaqjr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ezmcfzun.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zfurlzbw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2nzzuncve.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2qpcplxlt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2vvjpflis.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2brrudmew.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xgllsycf.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2qsbjpuql.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bjeogtic.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2nagwyjzs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cdddqbol.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2rajegunc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2egkmxcfn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2pghnblfn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2gugcuabu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2zzdeploj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2zfkxiqyj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2khezvrzu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fszaqzyo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2epmdkaaj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xeuidlll.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2obpcoqfa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2aiopqlev.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2lplebwrn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2dhfmdqcs.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2lunskqxx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2bbuvdawj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2qtjhiqrf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2pmfqfdwj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2yqsgotos.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xodcgnot.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2cfzxknar.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2jznmaahi.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kcdljlqf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2coubfbxc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vihqfhiq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2efptymdp.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2igylpaut.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2pmdvbney.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2pckmbphf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2hrtblnpp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2iswpnlkc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2dcvsvqje.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wdpigzkd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2dhqykrik.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2imbxurle.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2zrothxve.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2uqqmdpnd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2wufeeamv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ggfdlkeh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2nncaawto.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2tyztaeon.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ctjbbegy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2yydaodku.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pkrwitqk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2hvgsllne.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2lhxwicgo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2hrfqmgvw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2lvbbsstq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2hvueoryv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zhsgrvog.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vejcalil.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2kkowcsmi.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2yqneddac.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ysjxinql.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2wtlrgeap.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cqggqhqt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wudwhklf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mqwfgrha.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xxkpfgmc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ukcfbzwo.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hsiytbum.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qqesrfmm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ymfaozxr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2uezzaecf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pvmkauzw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hwloqgof.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jmifgnza.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2qtsbgfni.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2vwqywbkn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wmzewgaj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2dtmlxprn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pzghxokj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qwfxptua.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2yzzzhlba.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2rqzyslei.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2zsljanug.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2bbumqdvm.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2uwumshwp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2thhxoksw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2pfquggmd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2kaovuzsb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2fderqyog.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2gdvbfbrs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2sqllzzyz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jijekehy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kimyjzpe.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2wviydajx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tlsplxie.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rromxoeo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xdbffjcq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2irzgvdgw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2slvwmiyu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2hppyhvbv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2auvbxycn.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2grvzivhg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wjcwqrnn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2jbsdxiwl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qyhlqlxm.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2tvreeduk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2pzrqpxzc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2rnlaluri.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jyskayrl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2uznkgqqx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qstqdahx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2afkhucok.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lidhtuzh.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ksozjxas.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2azugzinp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2dlyfguzt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2drpbcjgq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fcxonbbp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2tnxgrafn.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2fkdvobav.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2itxtmfhc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2zyjectar.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2okhxlchy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2dizkqtsz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2memotbgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkffavpf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2trjykemm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzrjqamc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2qdzmfznb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2byfgxyjw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ilegamqy.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2gwgyjsmn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2syvxhrhp.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vkguyawu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jktpilyg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sqegpolj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mmavylih.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2yqmpynqz.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2clwcqjqk.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2mshzbvts.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mymqcanw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2nchrlubs.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yqrrowap.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2mavbfibn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2beofnyjo.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cnmgpwna.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2azhslzvz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2papdfroi.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2aetacsbf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2cyfboqwf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qwkephxr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2weqljztm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ivhkkflc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2qhqzpzmi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zijwarsy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mxqynmou.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2tbsyvvtr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uuczbekj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wxnxxlzf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2faobjpby.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2okvqjhqt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2idbqbuap.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hpqhvbqt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2avxocwja.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qeukhkrb.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2dfoovrwb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2sjpqwydf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2geyiplhh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wktbsiqf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2unxlhzaq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tmwwqxkz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2sgvjuhgx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2inqyaryx.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2szordelf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vzlwuiqn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2qjimtunw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2qsbbzdzt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2swdsispn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2cglwwywn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2fmrtnvwf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2fvzjuujz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmrcsyun.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2hqvxkrkq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2vjvevqnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzmbdjft.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2olkhlcze.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2cjgzvvap.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2utudrmfn.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2gfbwxxaj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2zktqwjvy.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2aenqghci.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2rlprnkzz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2entdvcqr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2pahboguj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2fgkqqopu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2xigpevpc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2khxshyno.html


<!-- 参考信息 -->