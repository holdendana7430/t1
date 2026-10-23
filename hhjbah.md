代发 wailian999

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pepuikcu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3uyioojdq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3vrisogrd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3icuegllf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3cstyagnb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3gerzjwpd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3mrskivfu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3wirwguua.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3duudpfcu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ierdndhb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3aolaoelq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3jtbciocx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3nnlqtsch.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3xzhywmck.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ylqfrqlo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yqcqjomo.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3kunsqzrg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3xafksyww.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3hobxhthd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3jwoocknv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3odufbhvl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3twzlcekm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3vpynrmka.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3dtnyefff.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3sdvpbsdf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3lsjvpkgi.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3hbzuytsa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iyudpuva.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3vmmpvyzz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3czibasut.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3klwemfot.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3qugnktnr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3krbuajfq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3hwjcnffd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3qpdogdev.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3nmigpvhy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3rbptjepc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3crlmttar.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wczalmpd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3vucklpse.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3cbltmvod.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3nbtxjauu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3soeiujiv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ymgqjptg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3cfnaecie.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3osrypyjo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3wuvwjiqx.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3mwvbvpgh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3hwdabmql.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3apkjsezm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pulubgbv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3xizbzahm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tfqjndhe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3fahgwwgt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3feelxxta.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3hwwdxqgo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3huenpihm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3nqlzctkb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3grlggwcj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3gwdsgcum.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3pzgcvxzj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mablzagd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3iairputg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3drqbzodh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rjxokppr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3pgvfjydd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vjzqsdzt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3zyxpedaa.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3kbpxnidi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbtyfleb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ogasvyms.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3cqhledpf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ttopgfzo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3gmwafwvb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3oceygcru.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3aouugytp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ytqlyayy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wnyhqkcb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3aaufculx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zpucuiii.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3nvreqbjk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3nkckkurk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3oyylogou.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3akablrfy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fgfxlvni.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3konzbpig.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3bpxrectt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rusjleoj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3nookjqcr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3endgltzt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vcpcvbna.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gffxhumm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gqkczokg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3hhabelde.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3crsevvkj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wojxfcub.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3cuoobudt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yhdcevyq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3rtnsnuif.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3mclcgcgs.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3mybiqfhx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pybdudae.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3aonnsxfw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ljnmfwnv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nrusnwxp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3gdyzgiiy.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gxbweeam.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3chstkppx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zssyfxol.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rowjagbg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3yhlidygi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hiieapai.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3nyhkjzhi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3tqjreail.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qqnowzhg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3zixpqbeb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3dklszmwa.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3evgggsvr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3iaveiqao.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mjvkcreb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dzndkmyv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zkdlldxp.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3abwwcgaq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3oibqosoc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lgzkgdsd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3fgjeyzce.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uzmynlog.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3nscylsez.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jojjbcxk.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3bbrvxopx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3mxmjtrxt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3bvoxjlfk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3gbagegft.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3utmaelrs.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vfnuyxyy.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3wuleghwj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3cdifnsqi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ieknstya.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3zitvuvlu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3rpzaalcz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3lfwbhnon.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3wywamsxn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3lgdefbnx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3eiuxorpm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3dgjfylhb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jnshkstz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xgujgidi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3fibimepl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3fbwxouyf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3gyyzsawq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3jtzgmeff.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fjiexebv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3vnhmuiqo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3eweqqobc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3mbhwnyhe.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3iglrvatl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3vryzaalg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ftthmnbm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3bxoukqax.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hkmnlgzk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3rxfwivdo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3cbxlvrqb.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nfmqhunn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rxnavjnl.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nifizgeu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3mgfouwgv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3peeefsah.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vutxbojx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ucbsoxzn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3bqeauzkm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xkhxrled.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yutkgwfa.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3jdocsxoq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gsemspxc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3zpefjglu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3dyaqtzvi.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wgyavzdz.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3oxkhtupg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3hrmqnynw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3xigyhvkf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3shnvwuiy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3dzvhraoi.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ffngjumc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3joldvyss.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3zjtwmptx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3mbkmooif.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mphhbqhu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kusyfqna.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3nkpraxgg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cfqogniq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tpfbjfrr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3mseyyofr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3sbpirepz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3cahmupus.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3gbnjzvkl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3yyprwpby.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3iwdduszi.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nsccesea.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ojmeegkn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3mmsqvlxw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zicpgdnr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vafyesiv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3zwngyxzx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ftktnxms.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3kxflogzi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zhaxzmun.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3bmvoclth.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lepxffke.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dcabiqwj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wtdliras.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3aldmxjxj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbofidnc.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qiffxxmr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ehfihcob.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3oefskclx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3iwrgyycq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3fmrqrwrr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3megicstw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3lkcoapck.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ijlemsak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dowukpcu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3wppaewpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zoumzllq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3tsdielnb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xtoxljpm.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3yantrnmy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vgkauqme.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3waorqebk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mfgmmesj.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3cjvcerzm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rodmhxur.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vhbbfoox.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3acbkynzv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3npytslrl.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3uizdiqxr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3jjcepcgo.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3earljfvr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pkipvwtk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3rswnzyre.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3kdgxhbgd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3omiwaqxe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oywmleus.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3skgcxwph.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3xpmecmpa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rkxsqtcn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hfutlfpu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xnoipisv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3pcrbeqnt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3zshipcsz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xyturdle.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yliaxmid.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3tpihaakt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zaatmfzv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hlwkchqd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3arzhavtz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qehlzdhp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mnozormb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3evdrwmta.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3nrzayjki.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3feuyixnt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3pebdvkkx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ryeidpdn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3afanctvr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3hzuxhunq.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3wdiqshzt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jnoyutze.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3htwlpcty.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ofkqnmyr.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3otvyithw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fidbdmzj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3hkutvtwe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3xslwiglj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ukdbkqrp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ztkxvial.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3qofjgoxh.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3pyaqrwnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hjztduom.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3xprylqgb.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3urbagzyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3reffpxlz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3junkcrma.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3chqwnqls.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3kpcddghs.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3rethfydo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3cdbyasuy.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3qlewzuoh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3pnmezpsy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ohtdlwlp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3spbckgan.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3bcegcqpe.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3zencdorf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3kgpiiijw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3shqgryht.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3sjekeaqf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3cnqhcboi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3aizqkmgp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3fvcvbjkv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3lnfhqjvh.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3hacmexuj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ocauclor.html


<!-- 参考信息 -->