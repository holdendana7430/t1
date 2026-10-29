代发 wailian999

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gampuezkm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gltlhklsl.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gnnxvihgv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gppgdvivf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gdxahpdql.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqlcmadrd.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gpjnipumb.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gsretsydk.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gagwofedz.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gchtsdimx.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gombpfspg.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gseaqgrhz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gnffibnll.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gcttyeizq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/grvlcfgbg.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gkfdbever.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gusklgehg.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gwuitryof.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gcldwkxdf.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gfygvkbna.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gxkxqaaku.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gpvcvjymu.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gjsfsaijb.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gksbibtce.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gjeaypplv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzztfjojq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gtvaosyki.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnivkbmdn.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gqzergics.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gjqjtgbje.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gfgkdxesa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gfjubhcxo.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gzcvswuqp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gbewooqlp.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gxzfeiyjc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gzapcxpaq.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gbwjhukqc.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/grcvdirus.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gvcaeghvy.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/ghawbdehr.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gsdwytzyi.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gpadquarh.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/giyhamrbk.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gdaljsbmw.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/geiekfqeh.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gekippepm.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gklxfexfs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gijfrsopq.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gzltjexmu.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gnuqvyzwh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gkbnehtvj.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/ghodonozl.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gnnrhahfb.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/ghqvunnnv.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gyheltnbe.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxhooodi.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gwqjlujmp.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gzlohdria.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gllssyfav.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/ggqkpufnl.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/guwlqwthh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/ghavfmtlj.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gitizwndg.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gyllyyxvs.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gzdalowqt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/glfyrifxv.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gvpjnplnj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gdqcfrkjy.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gohjcrusk.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gerfarobw.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gzcioixye.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gbgvaxpie.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/grhgdhopw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gtyaconnt.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gtrukrfqz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gdltoaedd.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gtbobochs.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gyaeazbem.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gsgioutwv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gjkyszrlx.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/giaktzhag.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gxevrajwk.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/ggejcqewu.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gmbidioqk.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gottdvwys.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/grviuqdmj.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gghuyrdxn.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/goxmcgihc.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/guxvgusrr.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gcioxfqsw.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/glcauacox.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gqkkvubwk.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gotxxovlb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gfdnzvptz.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gpjagwjof.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gewesldue.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gkgclxwvf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gtdvhcdyo.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gmclxtjah.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gvgfwpfls.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gzsdlwiib.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gozyvjgzg.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/grvnyiszn.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gtzebjhyq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gmnajwacv.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gdhobunwd.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gfewarqli.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gudzyjulk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/guzrnsmfl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gfbolysqn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/giiptdyec.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/grznblxfj.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gsjtxnyhv.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gevikbwjr.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gruyhtyxy.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gljfqkiic.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gfreffogt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gjucinprb.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gccmaucyd.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gohivurwl.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/ghvrusuui.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gootdcyii.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gxapkxqdr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gvcofvmrs.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gxushzdlu.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gqbcaknjc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gjkukhiav.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gskcneikm.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/ghxvxopvf.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gwjjnnjil.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gkbmixolh.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gdopnssrg.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gpmomcxth.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/ghlnyvjep.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/glaxyuqck.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gljstgpau.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gcokkacmg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/grqfhwzdx.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gttjnnvcj.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gbtjctysk.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gwiikhpwj.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gyeegqlwn.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gvmcgpksi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/glxoqhhvx.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gizxzsvjx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gzxifzqxh.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gceylbcfk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gserqrjam.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gexpjgzxu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gukmubotp.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/glbbyhjmc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gvybfgfqn.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gmqnidire.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gwlpavzhk.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gyjtvljbn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/glfhyzakq.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gtcqqolvv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gkgvdidct.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gdlehqncc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gcphadncd.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gtygaqgql.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/ggypxpump.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/genjuypue.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gfylkhsdo.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/giwfvorvm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/guvrfhfcw.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gzteoqais.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gdvhuumvm.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/guzmepxmb.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/grsqwmrvf.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gnivesxwj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gshwcdblk.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gbbgcodxu.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gngrggidb.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gkhtjcehb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gacwqhjan.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/geknzjzxz.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gxaajqeyp.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gtfysirgd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gzuvmhqdn.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gabgiamtq.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gdwonjngm.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gvsnraekk.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gnqqtbger.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gaapmyhpv.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gnuelymir.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gpzqukqek.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gsgygvgeq.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gcnldoige.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gxbzrqoxj.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gsupmxkoo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/ggmmqaqzz.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/golnqqeqj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gklsijuqi.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gxdqzfujp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/goacyufti.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/ginkwgoqd.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gwlyserxv.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gigvyihnm.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gustusosj.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gzroybvxi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gsyoufoua.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/glqrslsjp.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gairbsfke.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gowbkzovv.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gcwtpgiml.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gopmqvlem.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gnoudfwuy.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/ghyhfvqsm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/ghvivrzij.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gzwansdnz.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/guymndcrn.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gesseiwas.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gfefkluux.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/giogkmitc.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/grnecchbk.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gfceuehxx.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gqcuygnvl.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gmytarnvg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gnjgycvov.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/grxxbgqto.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/guyxoajxd.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gklakluaf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gbxnazlxk.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gbbnzxqyx.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gcwpjjpcu.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/godiyuefr.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/grtjkfirm.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gheioeato.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/giiycblcd.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gkkxjdypd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/guonbllrn.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/guxhvthse.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gwfunrfgq.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gkudlilbq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gqhcyqqxo.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gkelnyaic.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gvmkdbsba.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gagqlfutb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gjthvdtie.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gtzdabhpy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/ghdztdrra.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gsdizmdsm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gjvmuxslc.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gzinxykrl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gyaimjeej.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gkpwtjpuq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gpiexvrvz.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/grgxnyqny.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gllwktfzp.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/ghdzuxlvf.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gtrxocrns.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gnhmpnjve.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gtnxbdxau.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gjoofkehf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/glzlhdzxd.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gucaoevhc.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gglfsckkv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gfowjswqw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gadsysjub.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/goednosol.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gvywaxgsy.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gubcnjpsu.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/geckwylqv.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gqqruaozy.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gweriicnu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/grqnxsjyi.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gczxaxfsw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbjkvuvny.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/ggdeqsidc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grttutqjr.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/ggrrxfxeg.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gbrufayhe.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gzfqftiqu.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gnuuzxagk.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/ggiwsqeka.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gyfzzohft.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/ghskyodhm.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gceaszbbu.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/glbuyskry.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gztdstwvl.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gaaiobxow.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gfucunyek.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gxouzzkia.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gbtrsddys.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gcsbesbtq.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gsfysrrxo.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gnooibcze.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gvgghezpc.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gjngmzbpf.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gkfkafjbc.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/grqxxygci.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gsuaexqcg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gmfurdyno.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gfhbfwzri.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gdqrlxavc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gueclnscs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gopaguxqn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gikgynxbq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gkoslekcf.sHtML


<!-- 参考信息 -->