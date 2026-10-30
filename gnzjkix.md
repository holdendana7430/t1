代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gqinobflp.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gxlwsjmej.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/glummvtmk.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gbtyrigzy.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmcvxmgx.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gpahqmrdm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqnxavaw.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gzhdlbkxc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gpoumnxwd.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdhjboln.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoxdjqju.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/ggspvwqih.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsspnmbnp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkbhpcevg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzjmjkgy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykwfnmuf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbjgirrq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvbmaqie.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/guftbbomp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfqwjvofe.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/girywfast.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwtmhqan.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gumglhbcr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gzosegggs.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyftmion.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkvtkzqd.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/grpomgznv.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gezopyhmy.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gxikqhmok.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/guwfpptsm.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gxmiqbdbc.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjbdxvzf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmqygoyd.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/ggrcgohqo.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnouretj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/grbedvina.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvewxpjl.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbfcsigd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/ghnftwkff.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gppokbnon.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmbdgfpw.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gedxctrye.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubbmqcwm.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyzxnxaj.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gsmqjhsoc.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gedgvmkgc.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwpqaxcb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnchxbxis.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoogdvyd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglgsgxtt.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gyloixagf.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gywdjozka.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhdtizwu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gyxrxppou.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gprxoemdv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gktfxdrtr.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gvddlurue.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsxxwocz.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlvsteyf.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gxgneelyk.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfnjzolq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqotuyphm.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gitssfizs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzowetotw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscxronke.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gdrhstqzo.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gnumsvdwp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyivpzcpd.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gqroxszij.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gomnhdqdm.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwvfxbkj.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gmtkauuhh.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzuzuuuh.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyazruvlp.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkcymbzn.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbievsqhu.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gdbchossq.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/genyglkzv.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbkbyvdo.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaybfuhb.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gcyhqpxsu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gnsbackah.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gyskmlvqi.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxysfyhc.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwndxpugm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoqiaowy.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/ggnbetvco.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gvgtoshax.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhudhzuq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfifqpffv.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gzfbsrzas.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiuvjdhl.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvtleayz.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/ggtfxsoaj.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoqqnecs.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gjyjzgpif.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gsizegcjd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/guosljqgl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjbtoxma.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/gjwzbhczd.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gsoytbnob.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblyswbki.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gwtzjgjhd.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gmobhqsxj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnxfswpr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghupcuspa.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/guyihjiof.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwcfoqab.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gtwdkbjga.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqkmgoha.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/glwutoyio.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhwfpibd.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqbrlrtv.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/galrybikp.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnosbviyg.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrptxwzh.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvmebmsp.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnqlnhxn.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gticfyous.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/glvoqjwiy.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gzqxmjynr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaohuhzi.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grciqtyxm.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqxmttgr.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujwnlzvo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gloebtngy.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcztiaznt.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiabhuia.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnsmomqe.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmstfcunm.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/ghmqlhxhy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gnndjfnwc.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbozoenp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gwbtytkbo.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/glhrlrgsn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gmsgcujqy.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gaccfzxfa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyksixslw.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/godjhdpxm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvejniitk.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gksrkcvuq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdnhzjuo.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/geeibdzfu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkqxouty.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gxviepynu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnltpabic.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gcojrxebj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/glkrfwibu.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxvmitrw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gmynbzfgd.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gevcfeikw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/ganioprsp.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gqcsrsfbx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gpvekzmwf.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/grqmkbwyl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gghkfcwaw.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsrhixlx.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrbrnwru.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gdmliofei.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/gjmwfacdd.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gikugpunh.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gyhsevluw.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/glspdlaqh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gaqqgkgoe.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzjzasyp.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/glmilvxoa.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaajuaup.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/glhpsxwiv.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gnfchxoft.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqtkllnz.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwzojbev.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/gmqpsfmoo.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxjnqgjo.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmuxmitl.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqdwrynl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/giaedikii.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuhtzonw.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gkorwoihq.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhnfonzm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllpmlkts.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gxqpprxla.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnoulhez.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/grkoidgjw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gcfebubzs.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gctgxbaev.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbluxasy.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gywdwyqbi.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuzypvgb.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gzvfcvtdc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gjuxvytvm.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gucztciks.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpnaqzdy.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuhfnyfu.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gknqsqrno.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/grbwbcucz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gitaidgpk.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gwldqdrcs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gsobydeox.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gcnzdpczm.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjywejnu.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gimhqmyol.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gasdvnnbu.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gezzgxpbo.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnjhhnhj.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gxytdiapg.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gdqhybfuu.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnoktboh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiwvarko.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gugasjomd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gootdxsbg.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/goivcprpg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gypuqqxqu.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gtqdxvbpg.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gwrlpzuyl.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gdspuwvkp.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwmjpxtk.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsxfwagj.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gfkgptdvv.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gavxfjxgw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gqwlyzwii.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gqoeqshmn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcjimwoo.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gkftherue.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtpvsado.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gcumeoaea.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeqtwnpf.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gmtiipazf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaqdewez.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gmspjfkxq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gxkcngyex.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvhinric.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkpzkpmg.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglfjafjw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicglnybv.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaczdtyv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzouwqaya.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gbecakjgz.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/ghgzbcelp.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggupscgnz.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaucjkam.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gvfjkpsoi.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gecyuaqmp.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupvrtsxb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmktlcac.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gfptqball.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gywkhilfn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/geomewthn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gisiaksbr.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gyvdjpbtp.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gzjtkcduv.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqgtgxxg.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/guvtpsyqu.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopwyeiva.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjblpfjz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gitbwatsk.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gprgxcynu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecfificl.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusgklrmz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghqjihch.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/ghmcifmys.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/glblaminq.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gwlnbuqzj.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gipzuxozj.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gvlprazle.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpcctzmk.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoezzsau.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/ghgadpkvl.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvzklqul.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gfzsczvup.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkmqxify.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzndncqfx.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/ganblqavy.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvxpqncn.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/grzorgzlu.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdxbiqkt.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzapoqtwi.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdqkjbjb.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmiczgcr.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gdgwlcodj.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzammpmns.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gominapfh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gjrticbdd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/grbdptwww.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gvtjfgllm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gimfvwmcl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziflpmxf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gsenzrhwf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gocwhxqjg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwrszhhb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoqheijr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfjzspbd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrlgqfzj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gmfpckgnz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gipuuhmtf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcksfpym.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbdvjmge.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwgiyvlm.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdspoqwo.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gfnytpxfs.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gtdwtdwcg.sHtML


<!-- 参考信息 -->