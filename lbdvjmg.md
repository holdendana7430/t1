代发 wailian999

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gbsmxonqq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gsvemynqq.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gjhcqdfwr.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gwldfcpcc.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gnojhvvct.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gelmtmwdn.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gjqobwzbo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/guyqcuorp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gchvybfrk.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gzgdscrit.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/ggpdooxfe.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/glpqvekcn.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gwrcvipvd.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/guvkwifpg.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gzeoujoxn.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gjutjuxzf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/grdppnyga.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gnyapnsyx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gweabiuwv.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gbwjrsgwu.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gyznxnozj.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gbezxhdgn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gituoqwzs.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gkfwvickp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gvotwbayo.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/ggszjpwco.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gatdkajlk.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gieidemtt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gabsgpjze.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvfbouymt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gtblapecu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gazzkfabt.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gkzrosmlw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gmziqlrij.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gotckyynw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gshdlgfyg.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gzacjdres.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/grnhxljpi.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gvbubpgvu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gxnyxydoo.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gpeydicoc.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/ggdbrdjbt.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gavlpnobn.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gquigtske.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gperwrksu.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gbbninyiv.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gxciwwgun.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gffjpqhql.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gbnfsagfs.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gbwahkhfn.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gvmjoswnr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gonskknup.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gvilvmhdt.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gxoldccvy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gcvzghsmp.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gpmqtckdu.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gvvuhyvmu.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gkhinerad.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gpyphcymt.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gycnmtpul.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gumqvvlyh.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gtsovodlo.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gbzfgygvv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gmkzgmbqm.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gilntuhhp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gvnvsdxje.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/ghgahriji.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gsrhtesee.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/ggsbopgvv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gueuaptxw.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gxytflozp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gtnigkriy.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gvjxgwilc.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/geluvgvaq.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gagkqlobh.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/geeuekjzy.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gqsfrzhsj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gkhojqbbi.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gaozpcetb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gbkufnlpy.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gsmvboygw.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gtsupoyjn.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gjhjqxkpb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gszqzuabw.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gvjmskcnp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gzghliycp.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/ghnxlgaue.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gerugybfn.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gvmoiqfnt.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gptwhfpie.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/ghqltuerx.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gfiwjmtgv.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/geygrnnsa.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/geyrzchjz.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gjycdgmid.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gugaanxau.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gpahoqxgh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gkhwaulpk.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gajnoiumg.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gyyprfxbj.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/ghchzdlpl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gqfvsdwro.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/grmhqfddz.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gbduycdht.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gjnogyxcr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gctdnfcnu.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gtcpnsrgc.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gzpcpltav.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gwblbxrwv.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/ganwypfnx.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gkthmuxdq.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/grnejpbcj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gghqhnpgo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gjtypqxpe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gwwbprjle.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gkkajprus.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gufsjlgax.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/ggqoweuuc.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gkyclxhxt.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gsiyxqbte.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gsdbtnsmw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gdzthansk.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/genrcamam.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gzibaqayl.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gnkjrgpml.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/ggogqhyur.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gfynfnrtg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gqptrwgjs.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gtgdsgcrg.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gkfzpadlj.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/geawbforu.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gbaprbkve.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gehnfooeg.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/grimvxvaq.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gymasuvre.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gltqhrtgn.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gprsepibp.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gcmqpqvpr.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gtfmxesiw.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gmuqtfxla.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/grzmfumnl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gzopfynlt.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/guiplvrbb.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gktmoupjx.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/guodudcnd.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/guusebwwy.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gxkrbjcdi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gkatmqoqy.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/ghvpnniac.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gnaanlaii.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/goguervou.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gouyfchzm.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gwfzlhshh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gzpjzydxj.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gqldevgxg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gdmybscvn.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gbqxhhvpp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gdgoqvrvm.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gdkubzdcw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gdalrmdgf.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gncmrdtps.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmhebwgxm.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gxmmpxrjn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gxabhcltb.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gjademoxn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gnoaqnlxm.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gyccoyvkq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gznvtzcoy.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gyyekqvxb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gucihgyfw.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/glgdtewpc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/glgiifjip.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gpvsttlwt.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gjmcfppjx.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gyawzbzqv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/goqhgnlbi.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gkebufcsa.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gyyarevgy.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/grxoqxmyy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gmtwmhhee.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gpsdpszot.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gquojjymq.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gkpkibavz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gyxicnluj.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gsuhyqwdd.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/goeraozhx.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gesorpacp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gjitufkrl.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gwltidhvn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gismfpnsk.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gugzfsokp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gewwtnbvk.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gsuowgskz.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gckiesldr.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gvujueslp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/ghawjwayy.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/goctfrwmd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gmqkyktsd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gvmcagmrm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gqmeiedmk.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gvesbezeo.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gglrwdlev.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gsbgcbkki.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/ghhcigelu.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/glvrdbyxo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gqxcldqek.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gdanlmrnu.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/ggdptxmzp.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/ghchvtvtr.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gfzhsutcg.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gumwrguez.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gngwlwrxm.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/givaxqlid.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gurazmlae.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/geieutiwm.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gulldptou.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gtlvznbjs.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gfuvzrnfq.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gwdsqruzo.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gnjwirujn.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gbtxwoily.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gmssaxdol.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gdiuhoblg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gspgkqova.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gwpkjsbvt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gdiymbcxa.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/ghaqjmkgd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gleetqszk.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gupooynol.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gimaqugzj.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gsxcglvdg.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gtnducbtv.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gijsmefyo.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gzjrslnvz.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gfdqwdrdo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gtuonqmko.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gbhtqpmor.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gtsibbsmn.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gevefyabj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gnqvqkpkd.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/ggnbvuoht.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/gfypsxrgm.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/geqdisczi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gtpnuzmra.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gizgjmmoc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gufspztke.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gagzcupwd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gtngptbfw.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gppbufxcy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gpgobcjvd.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gkwvxotmr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gfrkjncfc.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gnkodtlhp.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/godwfdcvk.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/ggnecudep.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ggblmrrxy.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gdutfptwn.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gevcjohmz.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gtcadtdzj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gomqvwlvc.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gbplzdgph.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/ggnftwtxm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gwnxzdysq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gmhjpgmbh.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gbgvqivug.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gvkcfzrzp.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gvjduoivb.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gyvbphmfu.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gjlbnwvjr.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gaqojwbzf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/grxpcliqd.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/grbysxgyf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpxsszxsf.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/grzodzyjo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkqmyjpdr.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/glxinspta.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gaadoxjxg.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gbxflnznw.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gxfjbyenp.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gvijaqapo.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gmncfzjqs.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/giissnmmw.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/ggpgxcvhe.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gsppqrknl.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gemtogqtg.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gtwxgpnnd.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gsfsvaevc.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gbpdjuitt.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gogknoucz.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gngjetaxp.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/grilhykos.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/garxpmpdl.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/girvsyfmd.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/ghhvvtkkh.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gvpikfvyl.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/ghwvbrvom.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gentherjw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gslfxmvgn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gfqhccdfm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/glgibgnkb.sHtML


<!-- 参考信息 -->