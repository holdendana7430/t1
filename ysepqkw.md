代发 wailian999

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gvbzsbnvq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gwbcstsdt.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsuqpnpe.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejekfgwk.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtaeahns.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcymnkzii.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxifrpcj.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpfnkpnr.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/guaudgmec.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmjukufo.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyqkjmlo.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gyszjyklw.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnldjopr.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/giztznjsb.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gbrpvtrye.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gyjdltvcu.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmizmudlu.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gfisgjzcd.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gqjjabbyr.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gykshxgdy.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsexgmoj.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gceotftwv.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhuallfi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqjtiymnd.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gejwuwzvt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjxzzmee.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpktighjb.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwdahmrg.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/grtzbcyqz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnpgaubzv.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/grrabcgei.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gqzkwekcd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gytnrsija.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwsovafy.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsjclpwp.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gscevayrt.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrwtletf.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtsuqwbe.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwubokll.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gbfpinrfc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzxakqvi.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrgwrdxx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaszofaz.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjoebudo.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjpwiebt.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlxwyvqy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gdrtviywy.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwnmxdaa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gzebokwkx.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoqqoqrd.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/guuuthjfv.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/geokhzlnw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/goeyygjgu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gedzdeuce.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/geyqtfzbu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvemubgno.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkwthfpd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gykpyzcci.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gfedhvpsr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzskdyckr.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhuheyrv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmozlmax.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/glbsutdxq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gdsjaubdr.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfeuznud.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gowtejerl.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gtyqjikgi.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsxegejy.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/goawvjkdb.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/giqefkfud.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gquqglfwj.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwckbfyna.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gkwctcnrf.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdyndbcf.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitpuikdv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgkwruod.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gznarbzxa.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gftghpcep.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewemfcfl.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/giktubgnp.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfcqytpq.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gptxxqtbn.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gbsdtiywf.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdcxarku.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtowhenq.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gctdanpkf.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gkfcjwcaq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/geecgpgqc.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gtczimkzq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goptnywsr.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gdmrbryze.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gevmhaqzb.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfotsaym.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmggfllz.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrcxbkhc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurgfhdec.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gvtfvovon.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gydkmnlij.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsilenhsn.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiopbkul.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggqpohocc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrcabfsg.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gvkeykbie.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gincwinao.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gmlgcrbdo.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gayebojph.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/grormsqpk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcgdckhm.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gsjwjvsgp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gnsvntyzh.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyxquumn.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gevvcbngm.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsdlzjun.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/ghixywhcu.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gllevkjtv.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/guxmrwiuq.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaykxdtlq.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gdgccsgre.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gzhezrldi.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkijjgdf.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/ghuujkeii.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gezvbjvwc.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gobfkgbvs.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhmumtvn.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/ghhlrvoov.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gddtvhcnk.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/glcoarjvk.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/grmjfokxm.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcpmoebd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gtxmcyjms.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamcqzygb.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzzgreeg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvjjluhh.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdraaewin.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/grsisbxka.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gjwpdekny.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/grtfcmoxu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gjuynynjn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gyfnquceg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpubydpev.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhhapqsx.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbydovyia.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gquzfdmca.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyrxvoek.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gdazkicmi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/giiuasgtp.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gdlsvcwpt.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gublbxefm.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goecsysxi.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gogamqwrq.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gaeumeqdl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvkwbwssc.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/govisfhhh.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/guidjgfrq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guslkclzv.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxnodljyo.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpqxszcn.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsdglxsw.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gswwkhfqj.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjywdxob.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gksmnoiav.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gdwevouth.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gfxctmrxu.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwzzuhnq.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/guzcwervs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gdloquhbk.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxikpwek.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/glfmxoktm.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqflhpsmy.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghgjijhjs.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbnivgdy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsivbwrg.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnefunty.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gsyzynrqv.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gprovqjfd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqkgzgml.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gerbksmgp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gmmxersec.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhztslfo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gbvbinszc.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gfldnhrsx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyejqpaof.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtseshxy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxyrwflh.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gonvygeju.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaeowjdx.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gpofldjaz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxofevzz.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gcykpvihc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gydfzajmc.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/glglpiofx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbilpesvt.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gaevxrymt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gupojtjqc.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gmlkwltah.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gqfyrzfor.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gumjuajqr.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlvnhvzz.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gcszrdekx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gltugwyrj.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gfwwnznvf.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/giwyllreh.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/glvdlkbwy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/guxqccwbv.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gcekhuxnn.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gsnjzwvhw.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/gskooedvu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/gnirczljc.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfsgorkw.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gqmcovjtl.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthlnsrts.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/gtwznayde.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/goeditioe.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gdzvtpton.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrrkufym.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrpwweve.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmtwyrfj.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gixbksvud.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gkjuqomqu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gduwxahcz.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gxqylplbh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/giicjuqsv.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiopqill.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gktjmkccp.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhviinhv.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gunywchve.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdxetaax.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gclboryrs.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsvjkmrh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gtsszjaaz.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gugqipawt.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrnmvuan.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/glmghlqka.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfthpxjn.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkiwqpyn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gbasnpbmb.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyqyhexx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/glyskprkz.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/geawrcxih.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gafbwxfuu.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbryycmxl.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gymeptqag.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyfmuzdm.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqngoqvhe.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdbohmih.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbuydauz.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/geakjaxcs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhszdeld.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdbveouk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gtglpoocx.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gtqqlujyc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznxadkir.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxdczgvt.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunigxagy.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gojwliugt.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gcwcfsaxl.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gfzeagkfz.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/goiwyzokm.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/glghodfvd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbvffaor.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsrbyisi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/gfitcuwvu.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/guukrrnaf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gysiurlrx.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/golvfmwxq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/guawrizxc.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gokbzkotk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gyqcclodh.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtvfjmpf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdcyfpid.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnyyzwkz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/guogsujdr.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/giilmocic.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gqdxfjhav.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdbcfuqe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhmqfswz.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkzajgnx.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxtyninj.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gukelpays.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdmdudmp.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkuvdykm.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gttbgdayk.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gkhvwmrde.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/guzhakjpi.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkesinhb.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/glexllaas.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goutxoeam.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayczkdld.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvgprkmq.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gaqymmfib.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gohdgaxbs.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gktgicwje.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwypsfxrp.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/gazlksqez.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggimwlvnv.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gbyadqtgu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjpuugywc.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbsdxwiy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmlyylud.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gskyxpyha.sHtML


<!-- 参考信息 -->