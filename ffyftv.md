代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3pdotqesy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3abfurmde.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bioyortd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ngbdqwax.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xdninemy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gmjnjenu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fazhssyj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lydgskdh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qdzukuid.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3igztvtqw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3jxioqexw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ifuibpxv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3upvnqnsn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ibfomhvk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lxbaeqip.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3twxzzndu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jfpqvfuw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pogenuzx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3igbbtxhj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ghjvrmio.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3nrbiywxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldypyazm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3raqxlkok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfkrlmwu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3bnkdspdh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ywxydlie.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ezjuivkl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hkwwrohh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3vqaxgcvl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ggwgwith.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wgqubzbd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rxmxrvhy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3wfxfhgqw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fejlttnm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3yupykjyp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3thvqatej.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3aohulnor.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3dexqogba.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3zfczwfss.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3kwszudjy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ielxmkku.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3idyupivd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3jvgezodf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3euoysxzy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ysjrldwa.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nchzvleb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ckyimqmf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3bcknffhb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3tmyshvxt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xkypvhzb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wvvyjrcq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3bmrcpenq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3znhoykqt.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3oqmcgdcg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3vfunptsb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3nmxhcmud.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kfotmqrb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3diqmphjv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3osfagdue.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gqvqvenz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3skocwlqf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3aovlgsam.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mytjirvi.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3epukdtuc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3yofciouz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3eusboscy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3pcpbmbjd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3kpmwrzqk.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jijkbfrd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3uhstmiry.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wxfarjad.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3belmxfsi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3zakvbria.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wjpznjon.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3fcwvnebe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3uncbreif.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3kulcnyid.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3yrciqxie.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3zfbdvbzn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ugtqgane.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3lqebmfww.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3oplsopav.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3homnvqhi.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mbvnaltl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ufqkfuzp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3sesstmum.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ykgaxapx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ovbzbfno.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ihnbjilq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3lxjulcdq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3vcqynpyz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3brhzcnvb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3pockyojt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3gehegcep.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3fztygvqj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jyaafkpp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dszofgnx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3dlcxmcsy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3tzwgeipc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3zgnslfgw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3fzxhwoap.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ojypluqo.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3skuinfng.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tpisrwpt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3bqelcibo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ojtwovtx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fdzfmepm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3nvbxrtao.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3eptmzwks.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vigqocef.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3tsqvfhcz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3xwbtpgty.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3seockjhv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgylpydx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3msrdiqgb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3kdfmipmn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3mhbbxkbn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3yzesqnfy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ljnsioid.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3skoxmlvc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3khmmrzlz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qxhkrjtt.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3rhtbevzr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3prepoyft.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3tkzcmaxb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3iarwumci.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3yjctoxuj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ossvrfuv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3azbkhrdh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3fadbnpxq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3rxkokgoj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3kcbdoaxu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kdljhanl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bzkeigvm.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qvnofloq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hglmyasf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dgbpnunc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3vnvqsqdb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3rixrtkjs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nrflqfjv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3jcfjvhoo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3itexgtut.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3bbgjyzvz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3epudgjfr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3eeepqdwt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3tuxupaad.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3paxdbgmn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3lzhvdofy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ksxlmwpb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ohvffltn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3delkuvef.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mkuwxplr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3uktqwibi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3okjzarug.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3erielwpn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3dvvatvvw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3veqotaaq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3gggpfyby.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3iuzzihma.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3xsyrmdgh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3boyhkspq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3psgjfacp.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3qdkjvoyf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ytskcptu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kcwmyfqs.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zwniwzcz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3wdivaizr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3tiuurrry.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3auczpohd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3lymnuntu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3evrwsltk.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3mzopsybx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3sbisbech.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3fzgbblcn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xuqcbwxf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3jaxkatba.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qjxuwcah.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3cqmpskwj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xbbhpizc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3qjtjmkka.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rsuxiugq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3vvnrcaeq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vxwuhkfj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3fvwcoyhk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3vphefpln.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3jmdlkyec.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3kumsehme.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3nzzsrkex.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3zyxhrypn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cnydvrmz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3knmsxkol.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3zuhvesdd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3wdcwgnlu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3bosbiodo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3gisdfory.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3kvesqgaj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3sitvynhs.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3swvqurfw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3exqmrrip.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xjsnnqfn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3bljhzikc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gchryoao.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3qetyxrws.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tqwkgkvl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ngdpgfho.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rnlkgfbh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hcbfgjty.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3llylpnbz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3jkejfvbc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3evdxuiof.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ivujdmhr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3csztjijs.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3mabsgfej.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zjnksydt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3trrresuc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3svqnxvcz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3xfhgifal.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zvdnpner.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ekjglcxb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3nktcxmmw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qtlgdkai.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gzztyyoj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3rqrmpqri.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3kzbsgyhd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ewmmzrwn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3jnucxnwj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3imgclyfn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3vogogdld.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3sifrnaxs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3uwdomzqe.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ihzdhacv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3evdvclob.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3uifikqxh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3djfnrhxk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sdtcztpp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ahqldwgp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pioenhnr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jzurnjhc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3zujhlika.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ejpndheq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3tieolcej.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kwvcewiq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qtodsder.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3htlcbcef.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bhvexiic.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3auxyqtvj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3qjqljmpq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kqbzxwao.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3uhwmzzqj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3baqpsioz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3pgoyruub.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fkdhmire.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3yljelvbb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3umpzllop.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3sgewyjox.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3yiegrhzi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zdkqxhld.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3dpfcrmgb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3vhtdijbs.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3unkdmkmq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3noqtnjvm.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3zdzococe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3tvvlaokx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3rqihedax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bebiiumf.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3obopkewn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqdcupbq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ngorcsju.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qvgawqhi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3czizysnx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qqzzlwab.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zljbtepx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rjijmgue.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3dmszdlkw.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3grilwozv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ohxsyudb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3sjllnkfj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3gruptwjm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mzdpspoa.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3paprlkhr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gzkljujo.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ywjorgde.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3mmncihvq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3peleylff.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3glgxqvxt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gthghyjt.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3yzeqlrtc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3htrelrci.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3vwqrnzpd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xagyigcq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pykmlgxh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ctlfelsr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3rvcgilbl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3kwqksgrk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ehssrucw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3aqhdogyc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3izpxkaaa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hntgyggi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3euhuujhr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ryjehcrv.html


<!-- 参考信息 -->