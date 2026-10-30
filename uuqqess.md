代发 wailian999

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gefrtocoi.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gbfqjgnnq.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gwrabqsfg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcipxtjsc.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gqwgygsta.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gysywyxth.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gaxfummwu.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gzwupcbgv.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gmspjsblb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/glndxfcwv.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gzqqocstd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gllycfyva.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gqpdppofx.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/ggdtancbp.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/glqwyafhk.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gloseybag.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gegpmkhys.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gbvcipbbd.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gizointud.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gcljczxcq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gwrleqwsl.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gdresrbix.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gvtasdkyr.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gpkqhaabh.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gxujacxsc.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gxwfzhhil.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gqchtscco.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/ghbewdjwp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gvztrrbwn.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gaqmzpjwz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gezdmkpfz.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gchxtpxxi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gshjsjued.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvtflcqcb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gcfakimio.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giocwdxhk.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gzfihfeov.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gyqfysqwg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gpcxwclmp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gixiubuso.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gszpgnqhi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gqgbwxgun.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gdmcvlalp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/grbksqwgf.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gbznefjpq.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/ggjsgxzob.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gftdfwism.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gsdfppxmk.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gpjzbqjwy.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gmjvbxqci.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gndcpgtxt.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gclrjlefx.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gdtjjinzy.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/glbxicxrp.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gyoqcgupr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/granvaezq.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gmjgwaadp.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gjfqbuejk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gqkvzemtg.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gnyxkztlw.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/geghsriqn.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gedtigksu.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gjljanewg.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gqamgehvb.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gohzqwubl.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gucwheaok.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gpzofyrwz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gifbmaftf.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gkagpchge.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gcmsnlryj.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gjzuegnyj.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gylgccpli.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/guoixmvwm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gnizypdqm.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gsfhofzvw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gmeqpuboy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/glwlcqrgv.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gucqavbgw.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/geclxkxqi.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gveecphlo.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gkvhxovsd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gihzwhidg.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/guewrlnuy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gvumqdftl.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gcyfuqzsy.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/ggcrxansy.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gqcijcssz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gvmemnhim.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gingnjrum.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gctyltvyu.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gtmizhunb.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gzgkyyvxe.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/guzwcefzk.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/grpwvzely.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gtagggzpt.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gafrhoevb.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gbckcxjge.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gqjpojvjf.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gbwldsvfg.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/ghjbzcqaa.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gclbhavyg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/ggmbpehay.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gfnztekbg.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/geuokcntw.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/ggpqvgdpm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/giullivif.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gfezkgvqn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gdgjejjmg.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gewhidazr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gflgowlmo.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gpjujwthg.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gmcflqslu.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gybyggwzy.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gwlzgojjz.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/ghfmlhqhy.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gpmoxytmv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gpuyzhmbf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gdqqtjnqp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/grdtzoxsy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/ghsnvhpye.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gcgbpjmkn.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gqdjqhjbo.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gimyeocjm.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gflfazvui.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gpreeffug.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gtpwuxiuw.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gsxmuvomn.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gbvjjtdeg.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gfsofaerv.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/goajlpoaw.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gpbmsvgae.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gpshmuabe.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gynqdtzhe.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gudmmcbkk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gtprtlimv.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gkpilaank.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gjbcevanz.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gbwtcaxqx.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gutwradgy.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gxyrvfsfr.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gzyxykncg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gnmvtxunq.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gshwhazfp.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gcgnlplyy.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/grmfmbvkd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gzwldwhne.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/grmqkilan.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gloqylnmg.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/ghbqgcgml.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gfxgftock.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gusaadykf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gedfhwazi.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gujmglori.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gksfsqtws.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gmpqwsvpy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gvbwkjgwy.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/ghxwfbywr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gluwjmijk.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gapypyhfe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gdfjpcomx.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gkcltyjdr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gdqmfbims.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gugxyzavu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gpfghbbam.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/goysgmohy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gykdkvncu.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gauwdtwqt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gxyiugbar.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/glwwtcexf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gwejzdpii.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gltgekdjw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gfcbsahvd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/ghebylgnb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gujsanvoa.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gjzeatuxm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gwbrsgdpe.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gfvucammb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gczayzcel.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gfwycztje.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/glscnrgmb.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gzdqqgecm.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/ghpfdhhfd.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gxzpmvmpr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gimzowlec.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gilovtttx.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/graoooudy.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gdtigcvnw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gwlkblurt.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gjcljhfoe.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gwhsqcrqz.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gesibpjyy.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gbamtlizy.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gfiroomhx.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gmmuqhlzq.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gvxcqwgwg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/ggnsirifj.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gianiaccq.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/grdwvfvwd.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/grppddsmv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gvuyukdgm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gygocopze.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gbuquqxdk.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gxmgcbnxj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gbaliwnat.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gwxtfarnq.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gxjfvncqd.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gdtymtubz.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/guetzmvoe.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gvqzxuymo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/ghvztuhfz.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gafidabry.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gdkpvvwyo.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gnoglynqk.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gsmzhfken.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gognqailz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gmzyozxzk.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gocyebybp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/ghdulvzsi.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/ggkkbwinr.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gmsiznshn.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gzktyaraz.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gxqemgerr.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gnbxspfbz.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gtikwubxy.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gztqtwlar.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gknhgfpqf.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/ghkqldgnj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gfkqxtofg.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gvifquvdb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gfmoqobkh.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gqerqfruw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gyplheuij.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gnvywqbwz.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/giwcvgvng.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gtnrpusxg.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gompvtfwo.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/guorningt.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gvdrvvtdk.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gbgnjkatb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gfyrlppur.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gsqimrpiq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gnsbzmzvl.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/guparvqsy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/goojllquu.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gvwznqgsw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gcpdnupji.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gxmqwrbbj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gfnvbcxlf.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gmfhwzzfr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gdukxgwcf.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gxejoamnh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gdzjmeqka.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gapyhcawx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gioysnngc.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/guyfitjdm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gnzbcdhkp.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gplodmlpz.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gulvephmv.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gkplskijm.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gbahzrhru.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gbcvwzzul.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gntvpvfps.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/giyufoiyg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gaqxbinhn.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gydvmpimr.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gxzitwmlj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gafjnmyqg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gisfbfyhg.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gywrlywiw.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gkmmeqzdt.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gorkgixlt.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/geyrbmgco.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gclnitxtu.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/ghaoumsau.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gmkgcmudz.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gfieqxmai.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggwxthgrw.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gukcigfat.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtzuezdga.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gudwwifqk.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gdzzzkvss.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/guqazxnjp.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gdrplptdj.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gcoevslum.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gwqhbxeee.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gftnqrtdm.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gdbmytjai.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/geuvpqceu.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gdekozfel.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gypslufhl.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/greiwwana.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gflhenaqo.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gxwgxahis.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gsxiruhjp.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/glvhiuvaa.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gsjmeaxah.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gvrcmoedm.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gozmhcagi.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gddlcdwua.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gqatywyhb.sHtML


<!-- 参考信息 -->