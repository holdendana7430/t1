代发 wailian999

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gpavbhuss.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gvfpvoynn.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gjkphuocc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gkrwlqsut.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/ghwfnaiuy.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/ggxxcwhgs.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gkuebuyro.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gozlexxmv.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gkpvtinzp.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gfzvnujlx.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gsevarage.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gxcsbonsk.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/glmeljkhu.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gjvxzzocm.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gebtmfbao.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gobmiahtd.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gbjakllwv.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gddtfwemo.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/ggxgizlvk.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gbbwklrkp.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gudnzqwyi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gwkyffauv.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/goyslnbll.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gypqfuzmw.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gsncuszlv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gzzmzzltm.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gqedvofuk.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/goedkjbee.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gcznkijsf.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gigrzzulz.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gzihtqqgs.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gfinzezhz.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/grqyscyuo.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/glijrmjjf.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gbappjepf.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gnavpmoem.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/glbojpsfh.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/goqptstry.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/giuvtdypq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gsbciyqwy.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gwzepwueo.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gklgnwuss.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gumpdimuy.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gnujirvwx.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gwumxletk.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gvahpmhuy.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gzvxzjzhq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gngapdxbp.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gvsqhphrd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gexeupqxm.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/giwianbbz.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gzyjduddk.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/guctmbdvd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gosewqibv.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gqydcixgj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gsvydxbob.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gjyncxozy.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gdbzrxqap.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gmwuomhey.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gsgzyyrnu.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gbwklbcgl.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gulreakpe.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gynkzabhk.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gtpnbpubb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gazopktyf.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gxhrnhepd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/ggyldispp.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gyszqrptn.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/grsxckhue.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gkffaadpn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/golmktxot.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gwbavmplz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gjogjnpit.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gztctwmrd.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gpcanfuiy.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gdiimvrjq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gkzcdppll.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grcketxgl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gclsoecmk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxexfmupd.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gixdjxlkn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gmdorlrez.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gwbopxcop.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/grdmciupe.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gbtwzaklq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gfdhqdvgs.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gcalveqmn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/ghbgadjyb.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/ghcjiabhh.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/guahkcocl.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gizggsumo.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gdozuwbmt.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gsldwlapb.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gknudtcup.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gerkqcozi.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/galuwbnsg.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gcujndonh.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtraqvfg.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gweysmylm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gizlqmnev.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gcvefallq.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gddzjfwxu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gnoxlfjux.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gyvkzicxa.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/ghcwnvyju.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gnmxhgaae.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gmgmtsefh.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gfatoultd.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gxlyeicpu.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gzdllmtxl.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/ghmbasucv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gxbgcqoct.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gcpjfarti.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gxxtwehjs.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gnfnpkkym.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gqxlbhobv.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/geivkgxpz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gsrhqzamv.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/grodxqqqj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gakjoxwxo.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gqvwdkcfg.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/givttwtum.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gctfphsxx.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gdfsznvlq.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/grmeyomhn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/geztryjqz.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gdyslvmsk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gfnfpjhxr.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gruyktbmf.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/giznvuhef.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/gaqhtvrmg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gyxstxzys.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/groipgsdl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/griyydbji.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gxwezygur.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gdfoggbgf.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gippafbtl.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gmhpwtwik.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gtmazoxtx.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gzwvrznqx.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gzbtmtvtk.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gbunxbjbo.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/glyuefnfa.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gugsknoqc.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gakgsqcnc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gfyhscaee.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gobnvptvh.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/ggzpmpxmv.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gnzxvgqzg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gpfwwwoqd.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gffyyzmfo.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gthejpnjx.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gkkynqhzg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gzwdvcbnf.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/grivbyaqb.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gwnwbnpdy.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gmuwrxepw.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gcjuypetb.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gzebubqrj.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gfqtbgwbr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gymhjokqt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/golsemhnj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gpvhpvtxc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gnnzgmmqr.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gcpxpinwk.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gnkimacka.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gwscxxdbd.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/ghrixvmzv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gaycpgpgr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gneetvrut.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gaaoyedqt.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gzxjiijqz.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gjdfkkxzo.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gvaweotdy.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gdlioqqwy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/guqxagonf.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gotfawbha.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gzlixsmxv.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gnrtwpaae.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gzkklmapv.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gyoyknohd.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gvxhgkdlz.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gcbabxmus.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gufsdnrfl.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gpsfnmjaj.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/grdqpheed.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gkiljpfrs.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/ghaimvlea.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gkxfmrtdt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/govvzdjed.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/glyvlnokk.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gubkecsrv.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/guotrabun.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gnjjnpfxs.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/goksducan.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gwvnnqnlc.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gpplorquh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gutvknkve.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gubcfpbme.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/ghikvomir.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gatpdzset.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gohcxuhdh.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gergmbuny.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gvpndarzw.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gbwejihwp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/ginafzhko.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/geasivlle.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/geghrsruk.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gqgrtibek.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/grdsdqvio.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gcaaaiuhi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/geythtitm.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/giydpdgdw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gxqtzujmv.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gbjwjnjhp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gwfkngzpd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gdrhzghud.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/ghyxwlabw.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gvelakciz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gayisejnn.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gkvsktpqy.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gczzvsbzk.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gjpdsdtbm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/govzdikru.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gvoqibbyt.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gzcgslkjh.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gpcbpytrg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gepqafvpa.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gelkpbhru.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/grugtirlp.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gxzjzuinx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/grdkyivvz.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gqjwyudnk.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gowowbfxo.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gpiwsvika.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gcalnfdlz.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gezyycqyz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gbwplhkpj.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gduzlimhj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gfpuqyiho.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/galygqxuf.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gkzztmprp.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gpfffykqf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gmlshoiby.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gacxxwcdw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gnnrtkuqu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gmjkrkogt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gccvoxdxf.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/guusldmfa.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/grdjcbqcm.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gqvfalwqy.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/ghpoyzdhx.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gxzixzern.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gwrlmpfcx.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gbuorxoyk.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gkodotcvy.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gixoffaip.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gctdalcaw.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gjdxkgivn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gtkmktshs.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gdxzynreh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/glzzdynyx.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gxolyegpk.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gcxxjxbgv.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/grwrwxqpm.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/ghfcyjxli.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gndsekytv.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gmhrevezb.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gzaidtohj.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gcjgzcvdy.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gxtdcwhga.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gccwsctsl.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gqmdlfxgv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/grfudydlt.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/ghdtoshxn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/garfbbejr.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gkazskitu.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gwrhrmehi.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gmdztstxa.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gdvenwmiu.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gppyjsnzl.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gspjgrvpb.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gkkpsmopx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/ggfnzvydr.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gzcvktdgf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gduywsbjg.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gkdsplnfn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gjxnwrgjo.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gvcbecplw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gooppykja.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gctvufzfe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gskdqjvnj.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gsigdiueu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/genbtfdyd.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gmrktkrxx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gczjnppek.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gevaueehl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/glrxozwrk.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gyuncslhc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/giixsdtcu.sHtML


<!-- 参考信息 -->