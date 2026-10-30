代发 wailian999

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzivwryx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwshyuvwb.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gcsdzjxzi.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlkcwplu.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqrakihc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzzqojqrp.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guiidrkbi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsemlllti.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkojhflgt.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqfewqugn.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmqdnvof.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfqveuqi.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gunfekdgm.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gekuinqig.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gfbnmamod.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxcohuha.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/giedhyxie.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/ggccqplky.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtjkoudh.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgviifqt.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngvxgbzx.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbfxwexq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdssqrpt.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqlpybxa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gyhuvqwrj.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsizrvusp.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gkcolfqhb.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/ggpanoqzn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gswdlfmnf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghekxntss.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsqhghqo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqxvdrrnz.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbjgyyog.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gtldohnzr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gztavisex.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsboahrgh.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gwodnptgs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gphyvtwsq.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/giygexwsa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gzwbfwkew.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzzhbxci.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkinppohn.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzcxirqe.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/givrjiogj.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gihvflurj.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpxutwdv.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gjanuouji.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gjajhwnnz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqvctkbm.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmmxkvfh.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gfazqaugp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gwwpcthef.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/giqbotsfu.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/ghzcrrxyo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjykeufnc.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gjhacyjvo.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrcqtweh.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/ghuulzaku.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gpnohpbld.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gymmbjlkw.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gtjjdhunx.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gtgqfjsrz.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gheraxemv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/ggqhhcowh.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxvdafmm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjftvnti.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvutdieh.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/glhoztded.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gqyzwewef.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuomiord.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gvevvqkzl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfoaawtm.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gshomervt.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/ghojabgmt.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/ggmaeilli.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gqnzuzprk.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giurdyfqw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/glgexwjks.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gxogddpje.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/guncgttuy.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gnpnsizng.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrfllghr.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbqluslc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gddgoxoro.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gvsdsarut.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gjmuendgh.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gazmqvahj.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gswvceibh.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhkgobkn.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/ghryddplz.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpffbcrg.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gifiphxna.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gkuwmidig.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvmbygno.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheyuygsq.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gxtvwbjmp.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaoyoeiw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gyjqfdazx.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gpysgtwas.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/ghjkymiih.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gjrkcqpmc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gpvstflme.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdiifuju.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gunuamqyj.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcuercgt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/grijrdksz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrzqxznb.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/guabtrbgb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuxmbfgm.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gmgtdwfbm.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdgxtido.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gdimkzerz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyyxpoqj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgoeiybm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvkttjke.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/grudsttev.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gqhtmmoio.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gfsdjtuul.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvrshycb.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhnxliun.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/grgxzkzjd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnfxlfuem.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gjjlesdfo.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/giskmegjy.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gnakepkfm.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gtalgdvcu.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gsnzwwcld.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gihfkjonk.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzmtqjka.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gxlksnggh.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gyzsjrihm.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdegckrk.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gacfkpsiv.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjejkeiop.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gctvagmue.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gvzexzwha.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhnejytr.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gupkkldqn.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqgtlenr.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/grdrdqbca.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gczhoyhdi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/glrwjapip.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gywtekbkk.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvdvavym.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gyskzqfeq.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvsbycyu.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmfntrja.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gxosfhkzl.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/giydhegzf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/giysaycdz.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfpnuvfp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gjjwoovml.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/glearadtl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/grlglnezp.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gechkuatf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gicbgcblo.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghukjusnu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/ggrlbswry.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gbftzwdbg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/grsgxifvr.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gbjwrfoaw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gykutlhwk.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gsmszzrpo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggreqqrfb.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkytnblm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbqbbhba.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gpclszmfn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gshiifvxd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gxemrekbh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjclmkpnj.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhkomaxb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/giifqvvqj.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gdenosqyi.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsslzseum.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyomndgn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gugagrrmn.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/goovcdfht.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnnpcbxp.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gurceypmm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjhmfnzr.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkojjdzz.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/grayotqrv.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmqlbaqi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjzqtmlp.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gopmqdxal.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/gxxcfmvfm.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/glcmvgews.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gioaugfmm.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gscbycdpc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbvkpkge.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gugwxxzmy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/guiuzrgmi.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/ggdvlyydl.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gxqvzolec.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcwstlqe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gztrypmmn.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtirvvsu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gjnkooyfy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgbhcrbb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gddqbnxfh.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/gfwulcokc.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gxfvflhtx.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnawjwlzj.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gucnasupu.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gybkwzqpw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwfctpkt.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhwzmrxb.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxrkqivx.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfbofgid.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtkwclxr.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuvdzzrz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/glesvuavn.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gokcdhqxn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gkmbhjqfp.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfzvswzo.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvvcndxm.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwuydyzp.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/gipmbnbty.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqknypjbc.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gwdbhbckh.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmrggdsq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxaufneq.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/guvtvnkzm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckajodfw.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gcazfuafn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwltwfdg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckskbsxq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpehlimi.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/grkdaliop.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbkztflx.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/glevvvfju.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdceqwbwy.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gehdikqyk.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/glzgamskp.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndbkgdqb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/grvaquhfw.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqmuljeh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaockrzrf.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcgcsfnk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/ghyjgbiin.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaebpwvd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhxyboob.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnaznvfc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmskdahl.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gqyuvejbg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gnnzaovde.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gavarvbbm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjygomgl.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkqikbjz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gccldjdit.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwedzlfg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyhvjivm.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpglzhwi.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gnnvwwuju.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwahhblc.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grewfvzvx.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/grkgpyhku.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gxjxyushh.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfvdyqdp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gwhejebzz.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gafjiaunq.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gzfnlbbjw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gqyzyeswf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaffkpgu.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjsqfgdg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiuwgaok.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gsylinvwl.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gznjkzjid.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gzafufkaz.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklyjtyur.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gyrmwbowv.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gpldojwuf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssdtffxb.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbalfrfar.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxrsuccaj.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gtlwmbrti.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbiuhgkn.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gtkwqvpul.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqftzsqn.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gluvlruqy.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/girbfsetb.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupqxadaa.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxemrjfza.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gwnnxcmop.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gjapbhgbi.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/goyknntvp.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gjjhfubwd.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeihilju.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqjfqszf.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gqyswpigh.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gkfazbsmg.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbxqsngy.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gtormlvrz.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwypdnfs.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqomkcjoh.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gofiypkfu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjsfxzpq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gntciftiy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/goysdkzsh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gcdtrozdq.sHtML


<!-- 参考信息 -->