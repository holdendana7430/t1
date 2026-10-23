代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gegoeduh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3qhshodil.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xfpdzemz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ygkappsg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3nhxtaing.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ksoyqizu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3milxgcun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocylhluj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ouoocsfo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3mpukaheh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ptswseqp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iagemeqa.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3cdigwyiq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3tfzrwyly.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3azoshlzs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3uqkeqrrz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3sgmyuivz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xtbiefkw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3iergvyem.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3vhfkbrlk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3uhtltxdb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hdpicegp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ozaykrfb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3uguckyil.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ecmvltfu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3lynvkgrv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3khiceavv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3igekrxlt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3debgjxpd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wkyarqud.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3goctbsdz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3vafxbmie.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3vfejwyvx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3yhibrcpv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3wertrjpu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3labfafnc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3rkkuxwjt.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3tclhigcz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3mbquniaj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3iwufjnsd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3xlogjleo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3oiillocb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3hpdwtsym.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3odyhpzyn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ioniujfk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pugvrucf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3vtzlqyot.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3nmyzhekm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hvuinfsb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3muydftvk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hngrdihi.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3cpyptgqq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3nfhcrkoy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3tqlnyrtm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3bzzsvlox.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3stuxpjht.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3mzjwsgzc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3txdpecwu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xunhyyoe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bqvkoeii.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qguwprgq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3zdzzkfhr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3kkucflpl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3dqkjfung.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3pbqhuyog.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3xmbvkosq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3whhgbayr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xgmnespq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3prjbwhei.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kkvnotuo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3czeebzgn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3bejzvlut.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3rmzfdyqj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3pawhhymv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3mlprktgj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3lnsgapyk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3kfagpcqj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wdnmjxkn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xlvrxcni.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ghseegoa.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ywimssui.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3fzujevne.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3svkwagzi.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3bcjadeli.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3kuecfliz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3wpgvqbrp.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xncunsog.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3cmffheni.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3gtrkgdpe.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3qcxclkpr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3dbcwurde.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3tuobxbbe.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3anflxswp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ovttlcuo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3lubsvvrg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3uaxpmrlh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3gtvfxawc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ztchupgf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wrhohrcx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3muabkczd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3muhtlbtn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3wbbzgpbd.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hxgvdmth.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eszillag.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ezvjvefp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3eoqjmndw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3eajbtfbi.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3soofjpau.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ltpqzgep.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3edfjrdlj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3opptwlkh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vpabiutt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qpsgtwus.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3jgowblck.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3vlavanri.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xgyqalyd.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xlrufnpn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3waglfesi.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3xfibzjvt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bpwofcjb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fckktsmt.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3jcnbuupe.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kgpyiuxt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3abmxoiaa.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3qdygxomx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sumjgpph.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3xwqrmmxg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3uauqwepl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3hjsjufdj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3glnerztz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3qrrqltuu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3vmbcoihn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ldkkjhbq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3eycymflq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3tzzroytp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3shzlnwim.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3iadxkqsa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3awdjdwid.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3gctrtckw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jpgymndl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ifxsmovt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3vhdkzzmf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3moylgnva.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3eogjywsy.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3kgpkbnpt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3zoxzozye.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3eqrjdxnq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3cvmxjivz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3kinepygq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3qnfjjnho.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3tlwezyel.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3wkrnhswz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3kmfiwkfe.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3yaekuumi.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ycgoggtg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3uiwloheu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3yjfotwgk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3qonuadvr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3joevrtwz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3krpnqzqr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3easjmmke.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3skyfeiko.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jgskfdhr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3nieecygm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ihchhxej.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3nsqasjks.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3mekoyvkm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3rlnazmxt.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3uculrtqg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3vukxslrq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3twoscmud.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3jqgcildz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3gmuceuqo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bnqbyrsz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3utavznpg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3zbdxajiw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3agvsddch.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zdlomksu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3cvlxabho.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3mlbdwjjv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3idxpjtwe.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3mvmsgrli.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3fjmqpwnz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ijfjadin.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3jnibcttb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3btgfpmym.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3tndsqxdh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3konvwgpq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3rjldikng.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3hqddhkdm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nsnsiqey.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ebiwgoca.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ekgfzhfa.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3mbqvbqtd.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3agiwomqy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yzudhbby.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3vnksmuxl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3osqobkgm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3oeemdmbo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rladvcgn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3bkimadkq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uuxiuylr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3uzintxaa.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3bbghefcz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3dyyjshxo.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3lnkbhkte.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3vkgukoac.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ztoryufe.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3cjcsbwws.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xwmpyafz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ikllvurk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3radpqlfo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3eferkiqc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wtoiuinf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3xygpioul.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ubvfwgbt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3posgqvga.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iccskzyj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nnixudxb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3btvsfagy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xzhonmyh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3chswkucg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3bvjpdyoy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ryhiyyfh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xqcqxzrm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cwleeyaz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3dvxcylqp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ndvalnnj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3yjtyhtrv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3dassznqt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3crwmmbme.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jtediltn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mmgrmgjo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uavqepnt.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ifmcuxal.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3yrfxyeqc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ervcfvah.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dlpgvwvf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3wlvjboiq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3aqfvhfmw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ajjadlrk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3lhffjzyd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3qrsynuyp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3vawjwnjl.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3gtqtlapz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3dugceoan.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3aubjtvzf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ejcfgqvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mluoadbs.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ouscfoql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnwymdxw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3wxinlvkz.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3hdsnlxfq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3odatobrv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3uhkenyge.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3gpupcebl.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3prgksprz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zyetnhxd.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3inobifux.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3twooefqp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3decviwjd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3wmhlrlbv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3oailthjf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3unjlcbhr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3wljddhua.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fqwwmcem.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3swdagmfb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ifrdqqxg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3nvjwpgis.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ogobuwfh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3arayzhvs.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3owfmaqwj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3yiilxnsi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pjnhgsgg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3drsvefoc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qnpezuni.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3jmeemipd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xcdpcaqd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gfmnwqgd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3brkwnbpm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nerkktfx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xjozyoqj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vulrhdlo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bnouwhyl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aumtjpmu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3zygyayoc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3rnchwopr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3henjopci.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3mrqgdusw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3hxfwhxhs.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3bejbteve.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ktgznzyp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3xlqryvbg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bgogvzmc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3soliaico.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dgwoxjll.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3jocoxwqk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kbjmdwiq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3yqbnnxsu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3xtorrtaf.html


<!-- 参考信息 -->