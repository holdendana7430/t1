代发 wailian999

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gelbqjngd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gudrzmpgd.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gismqwadc.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gyjszrwnx.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gzagrxmls.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gtbjjxpyz.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/ggjlycjtp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gatjaeuck.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/grrtuemcx.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gylkedfrv.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gbvtfrshq.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gvzodurxp.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/ggebatpbv.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gcsqanwav.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gbyrcllal.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gtcohcqlv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gsspkmytl.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/grsujyjet.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gobwnqgny.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/ggxlppzwv.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/goakfuvrd.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gxozrmtbq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gurznmnph.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gxgeyzvzw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gehuefpjj.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/ggcoospte.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/glojlfxsq.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gnhhvacqu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gkhrrhxhd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzbzjruja.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/goyxvanrm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggpoxtfih.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gstjkeuoj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gmwnpviqr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/grgsaufrm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gyhcectay.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gcyizqdmf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gilefrdcl.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gudsepkgz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gobkqdcor.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gcuyqdktu.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gdlkgsuxw.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gknigwhgk.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gdpknkise.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gsrtcimkd.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/glfosvtxc.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/glplevzdb.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gcizlkgyp.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gyphhzkbx.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gsdhkzosf.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gozayzxug.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/ghqfullfu.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gqrlmcnwm.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gvranstha.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gksdntxum.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gsvichqqv.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gwdruueek.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gbtisjnmu.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gydcblddu.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/goypvhdda.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gbauucddl.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gdrovlicb.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gfesnxbua.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gyryupuun.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gnvyysgka.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/grhfqliub.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gazpusafw.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gyrrldzax.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gselbxpja.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gckawpzjs.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gsiijpxyy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gupgwcfer.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/ggiuciixo.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gesuvsktk.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gdxjxiomk.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gzbvqrgex.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gjgfkhfcg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gcqymobdl.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gefcbflaa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/giceffpqm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gqqttzjwt.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gkzhojsrh.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gmvzseucm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/giosbwnje.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/grdluugux.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gyeaacttz.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gximkqene.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gekeargvx.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gglmhydmm.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gyvikvrbk.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gafcdjvit.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gaxmbndkr.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gqtlvvzvt.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gykqhipgl.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gqftqbuym.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gdmhotqme.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gbbwbnvqw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gboryqhkz.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gcdkxcfua.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gyztrccue.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gggakhgoz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gjwwtohum.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gqqbxpbgl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/glaewcmxz.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/geetcxwdd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gdcqwnlry.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/grfltzjzc.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gxqphoxiq.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gscesrvjl.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gvmbnqjpq.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gukisukhd.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gfkeyobfy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/ghzgrqcuy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/ghkqnonuz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gvhphhhxc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/grmaisqll.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gvcizocre.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gfdvzfitx.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/ggnrkqjmd.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjwqytyzy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gssbvtcgz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/grkoinrdr.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gfbmrxhhy.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/ghwaxaxkm.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gdxgpvycm.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gjncszbrv.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gpbqtsapp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gsoxkaxtk.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gtkovrspa.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/ghbkxrubu.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gokiyfeqc.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gvdrvpuxo.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gwxprahcj.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gwsosykbx.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gvniwdwpp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/ggfpdqgty.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gxbgkrsie.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/glomgsngp.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gervjtqlf.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gwkjknvmz.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gofjqjent.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gfyiysefq.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gceucprot.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gnsjfldzg.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gdbxaujnw.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/guyomkaxn.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gkopfujzq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ghuxyrhot.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gvczxtfle.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gocedakhu.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gdpbopazc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gpkgkolbk.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gluoqfcgb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gkiggnbjl.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gncxspont.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/ghxymttsk.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gogxnygkk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/grgogwgmr.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gaxrnepik.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/glmpzhvmi.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gwqpdifpq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gzonejgnp.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/glzivwmqf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gvwkbbieu.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/grwpwsxgm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gstgnqhyn.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gddlwvotq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gvbthhqio.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/ghwoqgkji.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gysfxsbnd.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/groyodros.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gsyqvjvnx.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gcxgwpfdg.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gtuyjzqoo.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gkovalqsp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gheuahhgn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gcwycsogq.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/godjuylts.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gjrhkbxzk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gohusudzx.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gxvmalqrx.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gbzcdxged.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gmownsegf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gowdbdtjp.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gbisbcsbo.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gztipgvmo.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gokedmspq.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gwewpbtrl.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gtruuugwh.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gcrowutnv.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gthxyawbi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gdyhyhunp.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gbyhepfgd.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gewwctwtg.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/ggfnirazy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/galdoqyww.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/ghkhjjctv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gunyowodg.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gpcizozdn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gsycvuifj.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gqgtsxfmu.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gbkeabwmg.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gzontdikw.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gsjlwrore.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gcsdrxqic.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gshpdgbpy.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gfgaxpvxj.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gagoclric.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gzyfioahn.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gbcnrjkmy.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gzeokgahv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gwpyesgjn.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gzgtjjoqn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gsccpauop.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gtjdaqjwq.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gsoakszor.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gjitxsfxv.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gfvvvlezr.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gacjtabjj.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gljyjjkec.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gvejskhzx.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gyrjwjgvz.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gcprzmhin.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gyiilpugj.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gjsodpceq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/golccafvl.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gkknzigrr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/ggutclfbd.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gzdjxaxzq.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gbryfoscl.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gemybbgrd.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/ghbnkzweb.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/grklfiemz.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gjsdzlnjq.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gyraqjpel.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gccfbadwv.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gmlkgqwkq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gzikzfwqw.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gnpmilcjb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gmyrharwl.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gnpecrief.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/giizmejnq.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/grsnakabk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/goenalula.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gwjvehbfn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gmsfkfbuw.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/ggpfkuhba.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gdvmmldmy.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gmrnxvtpt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/ghgwzqebh.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/giitboflf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/goxmxpvjd.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gfbkmcroq.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gjesqdgqy.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gcealzelq.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/guufhlcjp.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gidmpdfaw.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/guypopyzx.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gjqbmqzrw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gyzwwfhkg.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gtjoqdvfj.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/giihquisy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gzgmngmhe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gsypakcwo.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/ggfnbdnfj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gzlblgjst.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gbibhpaqr.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gpjlkyjjy.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gmbqvmxgy.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gumxovdbc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/glkcttvav.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gcdvjmctu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glpjdjeph.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/goaqwfkjx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcxbfsxhm.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/guihtcotc.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/givyfmvlw.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gemwsxied.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gqvwetrnt.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/ghwtmyetr.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/grertgtlk.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gwlnvejba.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gmwbavjwg.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gacakeupo.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gutrqjtss.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gclblcdau.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gjulnkayu.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gxcqpwdzp.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gcjtcebiw.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gkwsrxbpc.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/glpzihzoq.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/grgmvsfnr.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gabradorz.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gnhytwcrv.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gcklxbpel.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/glhrikneb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gwucpyurr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gdfyhunbv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gtftpsvre.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gtugwxpri.sHtML


<!-- 参考信息 -->