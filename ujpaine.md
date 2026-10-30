代发 wailian999

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gtelmgdpn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gevqgqjeu.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgjnodnd.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgiglcdc.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnajcrisn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gngcsymqf.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsjgbydz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkzvihqh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgywhpvw.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ghhgwhitb.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grridyjcs.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gobkfdlxm.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gcodnrqpp.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gepsfyhlt.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gavvpygbo.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefuczqwp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/grfzxjybm.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvgvxupa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gookemklm.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gystthocx.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbngaroez.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gbffzdcgj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmefmoquo.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzdyzbzk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzvgufvn.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gvarziicf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftibxnml.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzearlyby.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gmfizdwnh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grfyjuhmi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gwhgmilcr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuvjtsjb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjkloord.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzuhhwcu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/ghlipcmqb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqazhsbr.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gzifqekrg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gccfshxkn.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gtuqyadzr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gefnsoadd.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gochsedcc.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthesynaf.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/geejqwmzp.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacspxtof.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggojedppu.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/grfcvygxo.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gcxvkixsa.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrlcmzds.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/ghgdngwnc.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyztdogd.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjfuovnm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gzrfbwwgz.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gevezyyms.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaecoclfw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gialesaan.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/glvnsjvie.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gindffblm.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuphjsic.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gyywpnlnp.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/glsbjgszl.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/guuzwyyer.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzxksvge.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gftwtfijo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuodzdhf.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohuvvspe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejdenaaw.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gengqoqry.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywtfobch.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gvqcapbmg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gwasuehwh.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/geuxzamwg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gbvtdkgkf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmlcldqu.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gffccyjow.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkopeuoi.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gfdyeleld.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbdwonnas.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/goruwnrdp.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gdxejcsai.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gnnidgano.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjthyvjhv.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggajvhpwt.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gzualjddv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxnfllwm.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gbudclhhz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gxekbegks.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gmbhokmso.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwcodglh.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gihihecmd.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpiwnbbj.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/ggcrajyhk.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gljrrkomw.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gbgooyqwm.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfdrjixv.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/giamoxcdi.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoiajkip.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gdhlmljvl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/giyhhuzrb.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbbbneep.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gevmzrmpu.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzupzknd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/golssrcer.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/glrmxorij.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gbogvtfxa.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjbfsbmy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxosnzsp.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gmqnbpatq.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giegojiel.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoathuhd.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstxtpxpc.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guasjqusy.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gzrimxnkk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gnirunlow.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonsydhxv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gvmimlasq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gmbayftan.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjizhjwuo.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gjqjforun.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guievyjfb.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/giohnmsih.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gjtongueu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtpjunho.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gpdryldaw.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gcbbndpxk.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsxfvdpb.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjzsurpo.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqntznjnt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gealcxvbl.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gorcaxxbp.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypxhzlwj.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gqjeyghse.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifdurobb.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvygqwpy.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giymiusuc.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpndjexu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghykuudgj.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/giheqwyvu.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gpemdwnau.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gslkzctnb.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/glgfmxeps.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzqsyikr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/guhwftdgv.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gutcoyqnf.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gbhdwlhld.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcklhzmk.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdabxlwom.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gyqgpxbhq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsebkkus.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/guxtgvugk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnnepgxm.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gvhzqpbza.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gkgbuppem.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/goqrjuwgb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gslziuoeb.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gfhhajlwf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gvvduzaum.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gegxatuee.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbabzxvkp.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaanpxsgk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxkjickl.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwpqyzmj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtutpzvfg.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpztbpfnt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkxuoapu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gtditcgpv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/grrwalkoc.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gowdeotux.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwezxhxhv.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfaqjqpe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqmanvry.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gmqpfchbr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgtnlanz.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/guvealyoi.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayzwwxwg.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gzsaooavf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfpbowon.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubtiufuy.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/glmxltdrx.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmstltiq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gbayaqpyv.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/giyzdgzev.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gevecpyda.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcarryxu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gqdcvpajg.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gqwbljtqs.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvpzjksy.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/goxlxamsd.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/glypviosz.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwdetztf.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gknvygdpa.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gccnbaftn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxvszbca.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gxspiqihh.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gjvznmzdn.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gvytmmjbx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysywhtwh.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gbxtxerya.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjuwfngg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmacocrvw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxtoobfl.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gzdzkqbyw.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujkqrtkf.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/goujrazvk.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkstuivr.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gvwqvfprq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjxwaept.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzvpayej.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdejwyhk.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gskhyfkko.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzedymkc.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gaxgilpxo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gvzyxlflh.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaeelqbr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gksjiyilf.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gomatqtco.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gfpwkvfgd.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/giucltykg.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/grqsodfen.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmnmijivq.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gtpxlfdjc.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gusziftwg.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfiohzmm.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gidromtgr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdtusjjrb.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqdglmcy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgwxpaax.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gxygxhstp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gborflmmj.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrmduiqp.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gngloroog.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/grjajdten.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gbcaxiwda.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/ghqqjrkif.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfawsnzm.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhektlht.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnleyyzu.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwjvhhyc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdncuthhu.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpailytz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwuypdqp.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gfefgikgm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gprtytbkc.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswfdvmas.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gfapczhsv.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gftotdwzn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gegfcfrvy.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmbanbbe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvjfnfbj.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiecggec.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaxmroih.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxirzriio.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gzfqqqeig.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnzqegus.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegbrqetv.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/guzvijknb.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrznutuu.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gckyjxjfj.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gderirzus.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gorlkkpdj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gofcdknav.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/glhccbloo.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gibsuemsj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gcfcdipwp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzuabdjb.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/goynaimyd.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gvznemklj.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/giwtruzeg.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gfhlaequm.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/ghpneugxq.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gdowwsptl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gddphvoxj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdbyxqmr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gktnnllpm.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaivwvlm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gukkajdcy.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gulqdmhvo.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gcmrrtyks.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqbanpcp.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnbvyccw.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpdtercb.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gmordlnvx.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gphgoibap.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbnxrnmp.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgicdpbt.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gaxmpjvxk.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupuixfuv.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gvbpvuogx.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gjxbqbnwp.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/guevovwii.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/guoiapseu.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjxnyutb.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbubsulzk.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqoptqfl.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/grqsrkpkj.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/guypctzuy.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gpgjduoyy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gptmqzcle.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gtheipavi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpfozxfc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpfjtqwl.sHtML


<!-- 参考信息 -->