代发 wailian999

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/goaphidhf.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gjyhzgbvd.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/glajxzwgw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/girqelfdc.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gnatchlji.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gwwvpgryz.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/ggmhvpvsx.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gwnwhyhlk.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gwmdbzjqs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gkwtvhsgt.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gpmqcdfqo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gsjsidxdr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gtevtsehi.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/guhwpwwkf.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gssbsyqvn.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gzrdcypsh.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gwydefwcd.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/goxdbccyc.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gspmobqoq.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gapfmaapi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gvmsdljno.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/goqnnofzu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gpwwlkwge.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/ggknnaqba.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gikbpomfr.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gsvqcpcer.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/giscieyvz.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gdqvtujbo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gupboztze.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/ghksuclmu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gfnymeuiz.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gsernbebq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gzlbcegsm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtksjiaai.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gnixjmanu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxwvfpzzv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/giizyrxeb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/ggbxsqzii.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gaadlryvb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gxkpvnuvn.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gmgjppnik.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gjltxmbzf.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/guihovbzx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gmjcgoibx.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/giwhkhefz.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gvvnvevtt.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gcvewkimg.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/grqpdwkkt.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gcuqfpepj.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gapotejzr.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/grgoywhst.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gwbudhpri.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/guexnoihj.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/ggjzxlctl.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gokjaypie.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gazpawwxi.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gsaoxqxkh.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gpmuwcbgu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gojmqlokg.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gmuwypmpq.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gmtwjtrjt.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/ghtbllkao.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gyksnxfjm.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gjjcxmqfi.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gludlvujn.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gflgkzosy.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gygjzpzsx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/goyfcvczi.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/giikyxhyb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gxqkeixjy.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/ghkgofgwh.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gwxcupngx.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gnzvtguag.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/giiiskjcp.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/ggiuvjdxd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gasnwescw.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gfldbzecg.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gaonhuziq.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gekqwqstt.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gtjxioylh.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/glggsfgzi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gmhvdkwaz.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gjmzuasit.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gxtktklyh.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gjgziwutu.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gddhuoexp.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gdlfkvqef.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/ggfjppuhq.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gilrhdmbz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gvahxggwm.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gnaukzxou.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gwxceklbn.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gfdgwdnjo.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gadpzqssh.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gslsuhide.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gwgilalsr.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gescgegnv.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gbkdsdrmk.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/glyvhzyia.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gxfyngzcj.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gdamrexyl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gvdhsqgte.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gcesbgdah.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/ghyxtekbt.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gvxvejbgw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxtnzlqb.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/ggpasyeel.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gwgghxotv.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gucpdgmva.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gndaquuja.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gqwcivbjn.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/glddagxpt.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gsoagavvr.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gomlfwpfm.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gshjqgdby.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gwnivqxju.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gupyasocu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gezdzfdof.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/ghjuaoxkp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gbetanczg.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gnoddvlwu.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gxysupcqo.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/giukgucen.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gidegzfks.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gpoplaazl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/goehbslwl.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/ggchqohth.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gradavexj.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gxwcwwjxe.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gafsyzvib.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gjdencqnm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gavrnphis.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gbhshsfau.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gntiouvyd.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gakxuniml.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/ggxjmamid.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gtgyrlkph.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gabpinqjs.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gydtflzyg.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gxnmpyfqa.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gihpdsomj.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/glrxudtsk.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gtaeladil.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gnyuwamuy.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/ggrsysgyv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gwrfsjwsw.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gwejiltav.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gmmnzjooh.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gdclwbshf.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gtfenroqs.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gsrmxduaa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/ghpzdoxky.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gsasrsylh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbvngkwxb.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gvvbabsdy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gbnmuxsvo.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gcqbicryn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gjweisool.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gdfvdyceb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gsdwchqfu.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gcgmqnvlo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gdohiebcr.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gnirqbrrc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/guxevhfow.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gorjqcylw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gimgtnhyr.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gtrabawcy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gipqyuvib.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gbrbktoxe.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gxdvvyfqr.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/glfccgsrh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gebybackg.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gxnquuxrx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gzfxkgcef.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gatscpjsp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gmnayvwby.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/ggdneavvq.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gdpednbsv.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gyajhmbdr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gdvktbspr.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/goyikiccp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/giiunqefi.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gnzcuzupn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gixftlvxs.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gswnrtnke.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/ghnnemxrz.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gizazzghg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gvpxvxpfr.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/grzabblus.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gyqaazqbh.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gmcappfsv.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gazjviqin.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/ggkmkdozu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gkbciosde.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gaaebhyfx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gcxhelxhl.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/grztalwjq.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gqgggdbez.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/ggwgmlxsx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gcieqcxrt.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gfgagfqtv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gxbaztvjk.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gywqssyor.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gsdhujejd.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/ghyfwwwbt.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gbelzeysx.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gdurjasxq.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gqogikqgl.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gamsgwrco.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gadtnyxwh.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gxlxufxdi.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/guxgnmnxn.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gkpqyqwtr.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/goitiewaz.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/glhfvztze.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gsapkbacz.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/ghvnpvjrf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gutodztkk.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gbjiecjlm.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gtfdyiwbe.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gdooeojrp.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gkiagzpxs.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gqupwaevq.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gnxbyvpoh.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/ggmhgiyqq.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gqxfgvdiz.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gvgbbxtvb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/getiqvdjh.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gtrxdtkxr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gzumfbiir.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gjvdvjcnq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gwfklrgnf.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gerkmkcev.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gqleopkfy.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gtzpjebgt.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gvmfagtfl.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/galdtjggh.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gqjpeieun.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/guwnxlfsk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gxxkkoetd.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/goanwfocs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gpwdadykc.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gzdvxxsxm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/goxghtbgk.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gdawrcaug.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gymlsccjo.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gadlbwdqw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/guaerwnmu.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gcmcwkmsq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gmgalybkt.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gshxninpa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gsicqpbsu.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gvzqdxdlm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gbcvgmhmh.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gsryozewh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gjfnfitpb.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gzsuidwbc.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/glwtyyloo.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gjnavijri.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gyrmkivfu.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/grnxbtkxe.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gedtxelgw.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gdsdqwquy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gtjmnylut.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gqjqdayka.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gzfcjqnhb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gaqycgito.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gfpysxkpd.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gemddkngd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gmpmtgrar.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/glrawpnyu.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gfjhybyef.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/givijazfv.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/grrazczzq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gdfxddzmn.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/girzqlppe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grphlbgpm.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gbhtvqueo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glqbnfhwt.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gjoomvtao.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/ggzrzbdpu.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gcvmvqqzj.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/grmzezcfb.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gvzquqqep.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/grdwnpndh.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gsrlycfef.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gpziuyjeu.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/ggprobohw.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gvoqpprwc.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gdhqtqieo.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gbeqjxlxd.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gphnanhvw.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gdxhltrot.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gvhbjmhei.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gamsjdras.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gwzrnkakz.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gnyqffmdc.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gflikroxm.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gqdultcfd.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/giyezxixd.sHtML


<!-- 参考信息 -->