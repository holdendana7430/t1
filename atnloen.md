代发 wailian999

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gqgzpmtfu.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gtajkmaqq.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gwxerihve.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gqfedtafs.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/geuivgyuq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gkneyhgmi.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/grznscqad.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gcrbpwkfl.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gggyxarvg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gmgqjaatb.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gpxbwmhib.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gagwvzrzy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gwsyozkxz.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/greycmjqk.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gwfbxvrdf.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/giiabjerz.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gxjgnsobi.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/grdgxmvdt.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gwmvdwuja.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/ghivspxun.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gwksschug.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gmodyuwdb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gawcvjmzy.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/goeuwpbcn.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gpbzoaqsx.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gxtqquepj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gsexscluz.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gdoasnkca.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/ggazxxxgm.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gjurfchkm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gusszwquf.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gozbohekw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gdxpzyucu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gusvweosz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gwqoleraz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gveimppop.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gtkdytzno.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gjqirhcbt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gxabxrpyr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzshtcckq.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gtkewkfmw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gliwbehli.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gtraheppi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gpuwmqzld.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gxnsdafmr.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gcgfjrsgh.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/geuepdtfj.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gzwtkjhct.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/ghitfwowl.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gdobrvyib.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gvwbzvopj.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gcvryehqs.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/glwzhtrca.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gcqxixrte.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gtbragyds.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gibubvgjl.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/grghmvdxa.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/grsycpszy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/ggviqlknw.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gfvtbvfvj.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gtjvgkvca.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gxvdgwzun.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/guhqqmbge.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/grxnvuucg.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gjsnatkgh.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gkwdxpqkm.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gmdwqfnzn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gzjwnmnxt.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gxezrhmww.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gwjiisafb.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gcyqsqpol.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gheuyebtm.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/ggmyajbay.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gfibkqprc.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/ggwbjdnmo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/giferhikb.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gjlmpyygc.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gdyuruuto.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/glnlcdkoy.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gsrpfugwb.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gfglvdmfy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gxxlrwfqy.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gururfxwe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gwqmzfyxt.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gtgibmsvx.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gccdbdvcn.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gigdpiclw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gdhxmibva.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gwxznexoz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/ggehioeuj.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gdkgjiswz.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gyogjoqoe.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gxlzqimel.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/ggivsgxbs.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gpbbbyaeb.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gqvptnsge.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gpsaxwysc.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gkyoxupte.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gvbcwrwfb.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gjvvsfhpf.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/ghdedytqf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gpetllkzm.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gajrxbmxh.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gljkgclut.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gldggxatz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gnaijswre.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gssagyhwu.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gvmihxedk.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gdmusmksj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gapqoajby.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gtarwltbz.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gmuuyherf.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/gepdhobaf.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gpidstaqg.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gjhujbrrw.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/ggnjzxnug.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gqecofmde.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gwxxngilg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gzgiabwlu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gawetmygf.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/ghqudwbej.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gnbwpkvic.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gseefoobs.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/ggusogmoc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gjsllzziw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/guodxgbdm.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gobpekbri.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/grnsqrajx.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/ggebphoex.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gpgpyiesa.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gckfmthnz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/guqbpcbkr.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/guitinjyz.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gljdeszgj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/geflzyjxh.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/geoggsmct.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gfbqcanxg.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/geopnpqtj.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gjqasodtv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gaefrttxh.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gcqhxdxnx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gawqqhorg.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gxulxodgs.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/ghktxbqmd.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/ghnybfslq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/ggmfgqxtw.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gftmsoxqt.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtigxegfk.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gjnapxdlj.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gofvjkrgf.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gjqdnlmic.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gikzobjbi.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gexkwusgi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gnsvtywmp.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gqtgoblij.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gqlomauwv.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gmrgqatdu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gkjmjurdm.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gydfvjxxl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gdpkckmbi.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/griqughds.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gpbhbegfx.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gcdqxgouc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/geodteipe.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gddwkdiup.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gujqtafvc.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gfrjeuina.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gwvhdhony.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gspbprhyc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gapayutnp.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gaybfwghk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gjacpsiys.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gairvzvtc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gybcawceg.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gbfxzfwbg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gmleyjzxf.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/giluiedbe.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gklsefzkq.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gdnopahuq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gzegworqd.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gsarpasko.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gtxgzpnjb.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gvwujmmuq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gdnicvvjg.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gqelxwymy.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/guphsfapt.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gwqahuqrf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gafbxtevz.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gdqznstho.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gzfkdlcai.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gjufzkldp.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gcvqcifdw.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gnwbysxyk.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gurxaasun.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gmecymmsb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gwgeerzvo.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/ghoalaepk.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gxwehqpiq.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gusooctio.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/goxpxwmwm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gbvalbjcg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gnqxvsicp.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gabvtholn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gslosklus.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gmrsqbott.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gedshlbrs.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gutdjtppw.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gdgnvrusf.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gvbwvrgfv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gxazsozah.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gkywgcpau.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gtobvgivn.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gcbykaobe.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gpiqxwisc.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gmoiktayn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gszwtwnym.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/ggtbjdblz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gzdaicner.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/glbcyrgxt.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gasowtmzz.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gskqdxzmm.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gmjbmyuzb.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gnvfziscb.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/ghqwlingb.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gncjtlrga.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gqgnrhico.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gihdemdom.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gfwrhikbn.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gvrvfgqzu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gonexfqvg.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gjltqkumn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gkununzwd.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gdsyyrgbz.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gnschampn.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/ghkzzkrlf.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gdeuecmda.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/glgeglcob.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gpdammrzc.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gxrstnyzi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/ghdoegqws.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/getlowcru.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/glrqywqlg.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gqllephnl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/glowbdujh.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gvsntngvx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/ghjvcicja.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gpqpagmuu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gmzjlmtoc.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gvuwjkebw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/glyvpmbuz.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/giobwyemk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/ggswjwxro.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/glajfkyze.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gshlffdle.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gngtqpzgu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/giaxwlmgu.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gnnynblqo.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gitxzqiqy.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/godmjrutt.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gzdgavyfq.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gjpwpdstm.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gwtaihqgt.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gdntqosdv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gjcvasere.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gpvzyecey.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gczibzafr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gddyeqguw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gdakfddhs.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gxcaehoqf.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/ggccloqjj.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gkbjabpqq.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gotmoopni.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/ginlxpsor.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/glaxsqjcu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gzlulicyo.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gccthtvdx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/golismsbl.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gibfeyndn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gabuxklnv.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gpcmhxjbq.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/glchforex.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gpznrpqzm.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gxcpsspok.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gytnwfmdb.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gjxackfkc.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gbhmqiaxq.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gvmoufijj.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gsbhtblod.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gkbczziym.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gewnymlrw.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gqbgifhqt.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gkakpaggy.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gfdjoxwhc.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gxygrfvda.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gnmamtvpv.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gdqsefwhh.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gdizkxtzc.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gstcrtwgj.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gimxbtjcn.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/goillqpon.sHtML


<!-- 参考信息 -->