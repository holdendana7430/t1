代发 wailian999

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gobuqboei.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkwwnudr.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gkdfpxqxk.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gptopyodc.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/guonvstgn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grdhheoxs.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghppmqkvt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/greieuhjw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecfvaudz.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gcldaawtl.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gzyuospkh.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grokzggws.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjmnkyaf.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gklgfwwza.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gdpwzujhn.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmemudre.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsunpuoa.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/goufysgpn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gwlscntkj.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/goqwurhfw.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gfbygoqog.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gvohrmjly.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gtrxwtlpj.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdpvcssa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gsftjvpzg.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwelohjz.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gioytyuez.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbivgzml.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/grcdqvvpv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqrhgukdz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gufkatyqc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvwsmyjqf.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gnlpqyxtd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/girlvltqr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/ggtsjjljr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjbolvhy.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gtescgigp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gebseaubn.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gloxqoqmu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/ggigualdh.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gemfleakw.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsrapmzk.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdodkvqiz.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/goejijoko.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gjrphygmx.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gdhdbgngk.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gfkmcjidh.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gxfpkhkkt.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gvicojzts.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gdbatinsb.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnuatqsl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkvfikad.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/ggwzfhyoa.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvishoqm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gecvagxgk.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjkqbwbl.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gplxisqhx.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gnfqjjhut.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/goasjnpsj.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/geivlldes.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gntbviguy.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwjshvyr.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxanodmey.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqzsgigv.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gqbhppvsp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gvhltftql.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gzadxulae.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gdcbkymke.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/glzvawurl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gtsqwznic.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gqthxcajq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gumpufhqv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjbkvncn.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gtumccldd.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gpimbmtoj.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/goxhgffcv.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaasxeicg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuugyzro.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/ghduwflrk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ghemiwlgh.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/glgtuyfda.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdignzoiu.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gildetdrd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gzhnyqiln.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gululvift.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gefcaumke.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gnzvcmvjy.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gcevdqtly.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbumwyhmg.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gswyobtbs.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/glawrcwer.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gidmqyovq.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gryfoillp.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gtfsbfckw.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdpwoeae.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gsquvcbda.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgdsiwfo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlmnacsx.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfwwloae.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gogqhwmfv.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaexcboq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgjskyoh.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gipthqghz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdtutmno.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gaxvdvikh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gzkvmhkfz.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/ggsffllby.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkkzfbwz.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gsjohebwo.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxljzpobg.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gokzdknpq.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gyqgxlsbj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gwofuywwa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gsxsjbtsi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gudjjddld.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gclowcdqo.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gqozelyzq.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gqqipvncq.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gvochixvg.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gzlnyvwtq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/grlwrokbz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfppqmsqn.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gedricvwd.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gaplkufgl.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gzegqaqmy.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gckbvryko.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gnolcswhu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gksncojfn.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gcglgijtq.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gbocsqdqx.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gdoucbzcw.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjgscuse.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/guoplmozf.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzktauvp.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzdraksjz.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gbzmsvlzw.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdyiuokz.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gcoftbcgo.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtwsxgko.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqlbumqx.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gaophcebo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgsobbtu.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gurksstni.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gbwqhfvsc.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gyknhdayw.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghggvwglb.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbcojwgl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gataaumfr.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlaqbbew.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlauvroc.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqglhjld.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzlirhny.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyvvnvbj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gvwjlrwyk.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/giofxtwao.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/grfnkcsav.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggipubzfa.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzlywpxx.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gjswcwvbp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gimavnnvx.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcvyqwlx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gncskxbav.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gtisghcef.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gyqopfwtt.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbyeikda.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gghqnusdl.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbscchvo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhgmtjnu.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfcdrpjt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/geuothyuo.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/galotizao.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gtvzabdcv.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gvmckrprz.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbkqdoir.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaxpfpes.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkzxbllq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgnbnrnz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcbbzpmt.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/grvrhtklv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccnngrue.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxlojubs.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjxitivl.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gvzynsgyw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gbrifcsjh.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdwumzih.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvvczhmi.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gtxpzbwvs.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/grlnxthhz.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/glwismzry.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gvaiuyhhl.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gsdnoeqhy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/goxyanbhm.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzmlkops.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqrthiwu.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgcghslo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/glgqumokn.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gkefbmmak.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpyyhtvj.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gaplhzzax.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/glttisogj.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/glvgeykjd.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/grslnigtj.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdbbrizs.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gfbzjmvci.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gggtmbaho.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaagichjh.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbenldczj.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/geikwmqce.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/guychyxwc.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjiebaab.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqipnbdyt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkszcyvyj.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gzdavoqua.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gjjltnjli.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfysgcqj.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuhofmrv.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gfazkjahp.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gukrivuwa.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtppqquqt.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpxlkpwt.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzjzneyf.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfmickhy.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyckwpln.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gejwfuqdd.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gvglmvcmb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxflphhvt.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gywccecod.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxvqzvxn.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/glgzndhhu.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhluhegb.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gnduxbkqi.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxnkfwha.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gabyxickc.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfrsemjy.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwapcmcl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gspeevgyq.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gmodymfrl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvdjttws.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gyaaqemaj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlawqjwx.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gduqbfott.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gwemceuso.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gprekknsz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytzjmfal.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gtveasulx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuueimqg.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gtcrikher.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhnlvomj.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaupbzga.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfygqmxw.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/glzfqvkxz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/glinynxxf.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gixxipbtc.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuysuwnt.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gqabejjdc.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylqboywi.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqfhuisa.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gaxiojgjt.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxevemiw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gasnbsyuc.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gihqrnbks.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/grskpevyd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gltcnakzu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/guphdcpji.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gycqrnpdl.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcucsadw.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gamitfxwg.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gvefuothk.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gfvbnoawm.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwbbxbru.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gtsckpdmd.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gzzygueom.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxsrsudj.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzzkmjgs.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/goydmiuct.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtkyvweu.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gpfxtnnam.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gldauwvud.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gfcyqndzg.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasuuaxfm.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gfshktzor.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gqqlgawmv.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ggklzkkyd.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gtfxnbfml.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubemukdk.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdmwixhd.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/ghnxnibpy.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlrpdrhx.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gofkbppwd.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/glpbzdyvp.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvucfxcy.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyszewsv.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gvwzbnpxk.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gxobodrdo.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gstihgydb.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gcmrhxikx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gcsivgzqk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gqopogxgq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gbivmkhqc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsfahzty.sHtML


<!-- 参考信息 -->