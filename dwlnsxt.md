代发 wailian999

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmzucdlo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gymfdckfq.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbkxszfwz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/grvcjcxaw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsqeiqxyt.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gnlxtndmc.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gqbrfztmf.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmcrvbld.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefnodyah.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcqiwyrk.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/ggtbxrhfk.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtovshwae.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/grkrcuuse.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyswfwuzc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gqnnxlkap.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gobdnrsep.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gvumiyebc.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gyosuwvtb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gkhsvtvzb.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gjidexfaz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gblxsncmg.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzosoboe.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgwupjcj.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjxidpoe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkefmygzw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzpiygwtp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjoijwow.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxsnligeb.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gykcdzpvf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlqrmxos.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gcpcmdnvr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrsftgji.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdwvrvhw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gkofpdqlz.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gsyrwnpil.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhxwwqqz.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gusxapset.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvchozlbs.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gqlhwjleu.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcnakhbq.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gzxsrfuqr.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gligzqexc.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gjgkbgujn.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gfkusqxhi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzjmskui.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gxekoykte.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gxqbsvjdj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gwldehnob.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gsrkjoxrx.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyguzflcv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavcbvesd.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/giegcxbas.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gslbqkksz.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshjpsuyw.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/grkinfxjw.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoprkpbv.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gzllrwsxs.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqfwsjsu.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gsaaoubib.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gabttbupa.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gclkutiqc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/googppzft.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqsymlil.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gzxevhzgi.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylyaapge.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtifvsdol.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gqzucbxuk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyublkwmx.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdkrntki.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqskfwul.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjylixjv.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbmlkgnd.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzexcjiev.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gzzdvojuj.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzmzmfaf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gerxzvbbn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuxyxlda.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/glbnhszth.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gqkxwruug.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gymcgelnb.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrbuhgtx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gjlzboeje.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdommzdu.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgeyrved.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gywwzewim.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/glynxfwqm.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gxezkdevn.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/ggkzpiudt.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkhmnznv.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzlpamyj.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmuqoaaj.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/grywsmynz.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gkaznpazj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gduzammtg.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gizyauafj.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gwuwamzht.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmepqmckg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdazgqsth.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gwoxaiiqe.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbprpcriw.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpgmcvqo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gebxvlzfl.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgkvwpfs.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/gehsbxqyc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmvupbaw.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/grocindpq.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlhhecjd.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gmzwwjbqy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gpbjqpnqk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwyxrjrg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtyvalum.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/guchgbsrz.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gilmyjgfy.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqngxdmz.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gvqlwrean.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gmtosffzx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmrvxncq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxscpggu.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedkwwevl.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/ghapijjry.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gsptcylcp.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gqihqqmuv.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/goanxhgmv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtlypzbdk.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnjuania.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gzshtyqjl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greurbpkp.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grrvcbtsh.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/guboilxjy.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjcesbmn.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbnuedng.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosvynydr.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/greuplxgi.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gsyqpqepk.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnyqsqbc.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlkasruc.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gizaxihuq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmqrhrwf.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/ghvxiliki.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbekfzakd.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gkmmvhmmo.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/guyewxsbo.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/gcnwghqlo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzcuxwtx.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/goivwkwdb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gwwisuaui.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvculcrwy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhylihas.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gwoodttvp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtknkmakp.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvpbkqbg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhefunox.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbasuayw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gldhzsgpv.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpqyoavf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/guxqpzcgq.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/geemhpcmr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghjyeitnd.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gmmmqyxrh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupntflfv.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbqtvjqt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxvbruqm.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhtbogkc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfgfgbuq.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkoxotdw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gofhrlwbl.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giastlxkt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukwkwlsz.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gojthtqcz.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/grtngegux.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gnypewwko.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/ghxtibamq.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/guekqtgst.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gactulqhy.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gufdjzbvi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatkffkya.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gzjhmiefq.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcpvszgb.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/gykchajcn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/ghqlqijhw.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gdvipzhyl.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwcgxvlv.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfdsvbgv.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxiybrjl.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gegfctujg.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gxlujttzg.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gpochvfku.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gbepawadf.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gtljheync.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gxfbxsohq.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gkudkqttc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/guayqpons.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvzztvxr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gmehzwpcs.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gqpcrlafc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gzyhtbywb.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmxqwfhr.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gljolwiqt.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/glasrtytb.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgvhdmzr.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdjcbeuu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfcsrekx.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gjpkfemcb.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzygralvh.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcdjmsme.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/glvnmyhwx.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyalksoef.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guifozttx.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gdmdnuchq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/grvgduxgx.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gcilkosbg.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/grdyirvpp.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gbmjaxkxn.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gqcklyyax.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcsojuhcs.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaczimzuh.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvxhsoih.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gchxrlugb.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gkqaegdcs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gvyaxggpx.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/glootfser.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/glvqhzwjd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/goatttqqx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gkoozalcp.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwguzqxk.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gxznezlpj.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gbhuiqjuu.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/govbfrpfk.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwoltssy.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gscknsane.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gmutxorbz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gcugeqema.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsbgypfy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/gsigndpvu.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gvooupojo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsbzhopf.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkbzmdhl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/glmfvprnk.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimyexxbl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/grtpodqjj.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gwyoktabk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgtymfro.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gmiophmtm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gcounkqgx.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gdreuocgw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gesepgmzx.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gufcjatbr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/glyqdesik.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gozacajgx.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/guartchtz.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/guivzzszs.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gxcycypjl.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/guubkpvix.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrcjoryd.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdulvzet.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnjttrxs.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaudutet.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhjmitbg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlhsapfl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpbrjuos.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkpofymb.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gffzsdjpi.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbckrciqk.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gcshiqedt.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfykdduz.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjvavloz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gctiggrmm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvusbvie.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfxlzcff.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/geonjgykb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmbczefni.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gdeewkbhg.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gynzxkamn.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gergbdwnd.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbhbwvau.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebhwuswz.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gsbbvixfv.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gszghjbyp.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gtiljgdmz.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gizgjsqku.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gtduesbas.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgiwwads.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gaymrnuro.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givckcrhy.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gbojeqcyy.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/ghejgcanq.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gosumzdjh.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gppsnvtww.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/grccizify.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrdwhasv.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gccrchosq.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/glxegrofj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gasezuqmt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqeggqnu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxswrtos.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghllyoqib.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvowbhdqo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyeumjrh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gknlmfiwh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gysiilmbl.sHtML


<!-- 参考信息 -->