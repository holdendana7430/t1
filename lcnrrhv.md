代发 wailian999

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwnqfnqi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwtovohgj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctzmvpxe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gwffklgfd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpwxvqidy.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gztbmsidi.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gedimodej.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gahtycdrr.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gqpimxcee.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwscfluuz.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkhtgwxo.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrqslqjh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gaszfyjkf.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gbxwoltjz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfpkqopt.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwuymvjw.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhmkgvzx.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gmvdbnhns.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gezslqguo.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmftfspx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gsrwhmzfc.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gmcdhrmbh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzmmfxzn.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gowysolpu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcyneaet.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdoqaltx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhctbfff.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnfpjaidx.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gzuyewigl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gsckbxqhv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuhvlfbn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdbycywe.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/ghueectsw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqnqogvd.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gxinbblrx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gpbllmhab.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtmjwgwk.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gcivsikty.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/genwdvyyj.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsuszvza.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbadihuf.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gszoumbmx.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gjzhusvbl.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gcfbtfdts.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/geibxcypc.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaztvwnh.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpleyfnt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/ghmrnhton.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtcmrbwc.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpjnqpuo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gvnhcsewu.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gfwmkells.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gllnekaql.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrpufxpp.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/glzzfqgwg.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gryhdskpx.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzjxhnhi.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoeyjnwq.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/guphqqfqp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gludirbjo.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnpqicvg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbcpdewp.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gdrshtwir.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gidhogcvh.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlcgghke.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjirjmau.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/ghhkuyckw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoewrxfn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmakppeng.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfnfxypj.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwopyisx.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrljmicx.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmzkmwnua.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gofcyhxex.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoptlhtu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/glzbczdhr.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gbeleqncv.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gclnnfrdt.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gaosfngqz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrgcbigd.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrpcbocm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvbzqicc.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/ggwgdfmub.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gqonpsssg.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/glwpjnlpp.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/ghfxcsflj.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gqffvyrnc.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqoggkcc.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gceglvbhe.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiqtfuqd.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ggycexunu.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtqiosky.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gjfbvrwxq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gslznynpm.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbvlujum.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gluhvbzrh.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhfalwmo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkujhveao.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhwovauq.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/grvbholcc.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwvyyazd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlbjsgxp.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gdhldhtsg.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/grirlxxrq.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/ghfrktpdc.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkavhbwa.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwydnjlir.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvzmevop.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/geiafattv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjnbqrmy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gpqfrruns.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggymrcrze.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbpdzwkq.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/ggwtjfica.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gwahalmpq.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpduwezn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gsbggurqj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glistifto.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gazlzgoin.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpycdwoz.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyrekftd.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gzqpanjrw.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gvqriecax.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvpnfilli.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gxbxumjtq.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gmgcwrvjl.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gedwkvzyv.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfhirzlw.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthlpsndi.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godnjzosa.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwriradfj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbislirwf.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshobwdju.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gexnuywqg.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjjdtdrr.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gvznrrrzc.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gofdcwqlc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/grkjizbty.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gjvqvnrab.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzovwhfx.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzxjucnm.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwbzqvwrp.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/gxxdngjwz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gensanueu.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfaxvvfdr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/grpsevzqb.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gynnlvpwx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/glcnsrzme.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gggaxapml.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gdpozdyrz.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/golnoiohh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gsfnnckho.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjixqwjy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gckkmlmfv.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gshienzln.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gmggxvulz.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gtpeeuodc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkortveyw.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiihylok.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwftmkcit.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxdrwqip.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfxqnkde.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gtpwekpzh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/geredycsv.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmxznnmp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqszjrqo.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gxrebtcrb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwfolhxt.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfafxhfe.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gkaxehlsr.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gtupuggvb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelowcust.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gxoelgpmg.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gvxebefzn.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvttjmec.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gfpxfftiy.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/glctmbugq.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gtewmiwdr.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gkvlmunet.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/grqqhiwdv.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gfxinnnpo.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gexcmyblh.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/girzfudin.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gofxotmjz.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlqqmmfv.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gxiachrhv.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsedrtlb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhqubueu.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gvkwbhhvg.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclwjvhdi.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/glfrctphs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gsmcftzqg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslqzmavz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gqblpbycy.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gscsqpfyh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzibthdf.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gqwqqyeit.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gszpvtwyi.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcvawmzj.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjncpwbn.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gixjmlkvx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbhfrjqd.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/glinlmmfa.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gynsospir.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/grsvduqqm.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gzteifgjx.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmtafjck.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/glqohijtk.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelxkstll.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gshiqjmyv.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gacwyrgwi.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyhxqgst.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gngcerjya.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtyrdkiq.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkcjwfvf.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpajtzzw.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gauoqpxdp.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbazwtqpm.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gqqheisrf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gratbsceu.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gmywaixsm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gazpzfpip.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gqsohgwnd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gddgyxadu.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/giptxhehy.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gsmqlwhgn.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/glqdkghlh.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnekmojz.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcbvcwcm.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvozyrjvd.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gjwzxantg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gqbpkripy.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcwcopgc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/goxromwdt.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/grkkkkaak.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/glqjpratn.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzpyluxo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gbxsgjzxj.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwwwqovg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gpejzabtg.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gncgufaux.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqthywig.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gtfoacjbk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gdkacdgzn.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gugvzhizl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gdvvzgamg.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gdcuoliqh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcigptia.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznayvcxw.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gvslkmgbl.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gulkqsnte.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhcvpsww.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/guiayrkdf.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmlutvpe.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gamkjpktx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/glixyouvb.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gcnsolnqq.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gunjvheom.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gonqvtkah.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/guiqvlkok.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmjyvohx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsllnsqe.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbwhwflk.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gewvgmuch.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gbugkqtqq.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gytzlzqjn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gonxgoomr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeyefhvg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glpzilvll.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gcereyngo.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpjnpvoe.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/grrzzuflt.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsksjjbd.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gspuzdwne.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gxvhaxowd.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwyuglig.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gakvxcles.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gzbyjgxcb.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gebnbcbmc.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gwagtlpaa.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlexxgwg.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfrkrfzm.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoeuadgw.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gfnvqrlbz.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiyqjpsy.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxlsjczz.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gytswnnly.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gzctcfhzk.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/glubqpnad.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gtxvrjhiw.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfchujyiq.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxymujml.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbtgxpfm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gyaizimwy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsiprvng.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhqvhqul.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvljhrnl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gywymifvv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gzctwliec.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gsfdbfodd.sHtML


<!-- 参考信息 -->