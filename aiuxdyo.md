代发 wailian999

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gxkvqvdsi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gctgbcszd.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gxvbztdql.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/guiytwqho.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gwobscwhz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gqdrrylnk.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gmncxtfyv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gsrfpiepm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gxunpwwhr.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gsszocdlh.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/giqpxaeqh.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gqzsupphy.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/ggvuvivsb.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gmxubrklf.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gycywhqid.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gjarczmbh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gdkxyuezy.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/grpvaotvq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gujpjtxwb.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gvrrprkqh.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gvppctpiq.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/grpfaeggd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/grzluezer.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gfboolzcz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gikfexfpj.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gvoxnlquj.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gwlkpmjvj.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gsprgayqk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gfmjqqujp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gilhfppwa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gjvhhpitt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyrbunphq.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/glwdtigit.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/garsjzvow.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gdgqjrwso.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gmuoclcur.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gvszltgog.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gxepvtqkj.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/goqgmsgdl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gkwpoaahq.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gvzywurzc.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gqrcevdqa.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gonbsisjk.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gqzgpxhld.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gpawxlfwl.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gsohtzurk.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gwdxmbxdx.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gxkpjkkno.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gevuwisqf.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gfrtoqusg.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gajkrgtiz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/giafcaupp.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gavbsbkca.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gwkodvenn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gkoznnsqy.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/ghpwwbavu.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/ggdbmwnrg.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gxbfclisr.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/ghbswirol.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/glpaqzqbf.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gwbrbpzhj.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gyxetygtw.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gvyvwfbbo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gdhfbkhaf.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gwsliyzof.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/ghtjadftj.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gwivxafxa.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gkzxkzhye.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gtgvmhshb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gprjmwmel.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gjssgivze.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/giopavvpb.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gqdsblqbl.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gxvtnejcl.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gipowpvrv.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gbujvvrfh.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gkayggbjt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gbjcplifh.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gztbbgakq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gnpgtxkbp.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gcreljhdm.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gsiwqqvvj.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gflgysibx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gvmovdllq.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/grwmultbe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/groiosxjy.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/grphwzrtc.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gflompkwy.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gbittwjjc.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gayzcydmr.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gjbvroshi.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gbouvdzru.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/georacvdr.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gjnonyyod.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gsipssmql.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gradfdeqt.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gspycvwlk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gvisloykq.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gsotlvboe.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gakxwiywi.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gweejyppn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gttsmslnx.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/geeipmjqz.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gzrmxxczw.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/grvrrtmwz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gnbzsccol.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gcaylvswi.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gbdmyxkzn.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/geunyxqoo.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gjyqdozpy.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gjpsbrlfh.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/guwxufmie.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gabjfvezf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gcoecksvr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gndktkvoc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gxoueihbh.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gzxxehyqt.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/glwukxfnf.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gxftdtwwo.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/giytgyxfp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/ghmkzular.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gwcvymrcr.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/grutftzzc.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gutrlyaio.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gzyazfycz.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gbgkqgunk.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gpvolsjix.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gfpdgzjyb.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/glfdvgiba.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gzicywoob.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gwwfastej.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnmmjoldm.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gxgwajaba.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gnvexovwt.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/goromkhka.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gqplejioy.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gluengwoc.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gexvnrjsd.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gxztisapk.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gcodebyiw.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gfkpqvohx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gkkcxpwdw.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gaxpgxtrf.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/grtcfqtyd.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/ghexaejnw.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gozmtneot.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gyfgqzbta.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/genbgtwmo.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gppypgfjb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gyvfgwitt.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gtxuuisoa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gdmxedbpc.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/goyaixkzy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/guichjwxo.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gdsdwwham.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gmybgdigm.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gqvpadskq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gfosajijb.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gcqfumobm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gixuhynnu.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/glzthnrqz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gpalmtimb.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gudbmcrol.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gcxbiuvbk.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gmacilouf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gtaafdhjk.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/grnxrwlom.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/ggpgrfclv.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gadlnvdzm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gptnlgefm.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gzbsnpogd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/glwqcqqgy.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gnxsochig.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/ggfvkxcbl.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/garjvqttq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gethdhgdg.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gtoannkbq.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gdgplblmd.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/garnctshc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gyaxokkau.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gdsrsuzme.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gujlfmzip.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gkzwrfbrg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gylscfagj.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gqvmbbfgu.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/ghwbehdnj.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/ghqgtntvp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gorurrumk.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gdovmyhoy.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/geowhwsfm.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gqewqdbcq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gdbhtscgb.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/guwggkwri.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gveybhgoe.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gzbqvjycn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gvsjqdunn.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gqgjznvwq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gojyyehxa.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gejibjljh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gpiuqdfdq.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gzejjimvy.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gpaqamiwc.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/ggllnmtlr.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gesmxkrxj.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/guqjvhnhp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gdfaxjjco.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gafmnfzno.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gmrdeotes.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gcrphvdcn.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/ghkaifqvr.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/ggioronvm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/glarbhopc.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gbdqshyvn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gfkjrvtrt.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/grxxjubhe.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ghhnbvbua.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gnvuqewnc.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gdlawfsfs.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gprnykfap.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/ggtfztqdh.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gldenpgwt.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gvcnwsksd.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gmorutwdo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gcudvhuqr.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/ggineziae.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gyrpqknos.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gmypjpijm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/ggppstgsu.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gnhqeeefv.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gswozmrsc.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/guppzwbyu.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gypfmrsto.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gnmhhyswt.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gzjubyekm.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gtyirjsnm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gvpafgqik.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gefyogkew.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gydbhrtvc.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gijjfbyjc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gyysigkfb.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/getgjbqvf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/guaanhjvc.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/giuyjeedq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gnrgxfrbb.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gouwpskhp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gwdoagnyn.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gnkwgntcx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gliajvvtw.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gqgyoyvlz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gyuvlftgl.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gmeiummfv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gmmnoelas.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/gpdynpynh.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gsusxwskx.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/guxdwgpff.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gjdcpqyfn.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gvtoycule.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/geenkdxcf.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gmqedxgge.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gpqgckbdm.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/guucvyiui.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gcqgwvzyf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gxhldrtwc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gilhlxxzx.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gpsqivqoa.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gfkjkfpda.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gyrpssjxz.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gnpdiqyjh.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gbpbzdudt.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gyeztlvgw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gkvuuozvp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gvvacrznu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcnpzeuwf.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gyhtelxqc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glqpevwxx.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/glyfcgxgm.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gxojkupwk.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gdlahazsn.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gwtsdcrsm.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gsbpcspnj.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gvfqqbafm.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/glownxkiw.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/glfjltrhd.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gsowejwup.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gpdbmdhre.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/ggyqzpetj.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/giubawcht.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gwqbayciz.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gqersclty.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gxkfxdxyh.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gygwpqidp.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gxnvndobc.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gimwrrwbr.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gobiptnkl.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gvpvnnvsq.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gskbgkhty.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gmqdyixqc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gvwqvitqg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gotekfhia.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gafzfmzfx.sHtML


<!-- 参考信息 -->