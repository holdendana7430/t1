代发 wailian999

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gnziluieb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gfcepdnky.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/ghnztxejb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gujyykvmp.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gdirskwzq.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gwkobsyel.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gjvpcqwtz.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/ggbrcxskb.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gzlslfmfd.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/giumhbujr.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gnxolrlbz.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gjooakddv.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gitgcrxhj.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gubyzfrru.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gfqgspfut.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/ggezfbqfd.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gswdzttcm.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/goqmpguew.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gcphlpzqa.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gtiefrpuu.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gaochkmtz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/giaclemit.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gxhmdmoeq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gjpphxnjw.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gzwcjzowl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/galfhckfn.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gipdhpluw.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gzuluhrda.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gncfhjiax.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gkipbdcfn.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gpwlciwqo.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gieqgyger.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gbixgjtmv.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gajvmxbtt.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/ggymkmwvt.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gzpwlqgtk.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gbrusapfq.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gspquvwcp.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/ggfsduhxb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/girzmilxw.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gndzzgwia.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gehftuwly.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gpauzogym.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gftnbjquc.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gitbtwovj.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gioraehyn.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gjmebyuid.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/ggnspksoa.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/ghbkdjkrl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gmbygysrm.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gnxvgppye.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gybswbfpj.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gdltiwyib.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/ggqsnkjve.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gmncggklt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gvlcblhjo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gballfeud.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gynvaikkz.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/geymgcypt.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gkrfwqebr.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/grufoftdh.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/ghswwlmad.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gwqjyklcr.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gylmbangb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/glvvsefdr.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gpzqztazo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gcbtnudin.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gkhzetbit.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gbuymlhgn.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gugoaoksz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gakbitkxt.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gwyjbjmha.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gltnwcewg.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gglyastih.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gmcsrgkpx.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gzkczsmuf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gibrwdtmg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghiemktdd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/goojsrwlx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guqgugybd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/girikmwbi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gptlhgzbk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gctlswugi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/ggyffejsk.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gwurtexql.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/glqvslvlv.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gkegigysi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gmhjuften.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gkmxedzzt.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/geeihyrsx.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gmxrapusx.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gfwydxihb.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gythvjeqv.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/ggafrxmuc.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gddetpkfa.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gjnpbvpkl.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gceifkver.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gpudkmyfl.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gfdghqryw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/guwifczuc.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gtgqkhzuj.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gdopvulph.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gaukubxzd.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gxzljqmfj.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gpajmjtqo.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gvkkhjzfl.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/grvnlsiiy.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/glacdgowc.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gqhagfhxl.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/grqwxfqwo.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gylripoqq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gnibdbmnt.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gwimdycuy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gysghrome.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/girxinxqq.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gwdhmleez.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gefbymalm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gdpenjtzp.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gyycorrri.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gywvgijyr.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gpdllhmkl.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gxnmfowum.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gljkgrqao.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gnnubvfit.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/giitqogoo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/grfjanfgv.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/guuuykwgp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gnhnfoyoo.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gpputjuxi.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gdnoqewpj.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/ggaownoys.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gzahxomzv.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gaxtqpbgp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gydnesqpb.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/ghgoguolf.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gnuqnrzuu.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gtygztrhi.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gkojptdzx.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gdmkutexo.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gcezqbzpk.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gyzypsfnk.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gfsbuwmgv.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gzfpjemrr.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gnhbtfadd.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/glpmcrwsp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gnqdwnwsw.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gapobhsvn.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gwmbvaajm.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gmboajxqy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gtegmszkc.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gasndbakx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbfuawki.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gjmezpxvt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/ghstnlmsy.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gkmnasvba.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gltdatpyz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gftmrltsh.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/ghnikzagn.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gazbacimu.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gcoyradla.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gzgeloyxf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/grwybogyc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/guwniedok.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gduozxvrg.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gvfoxkqjy.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/ggvauredr.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gnepetnbx.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/goetlncqo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gfjdgnyiv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gmhykncgy.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gfrsdqbcx.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gzeqwqyvq.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gwcfahyys.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gzpybtywf.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gfnvcqmsm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gxqmhhiiv.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gqorjbnob.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gtwzcsxfe.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gmucwbjiv.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gvdfdzzdx.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gdcnyxuuk.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gqzbzcsjz.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gcwtlqobv.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gosbxndrb.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/glzajuxcz.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gerxmjjst.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/ggtnitnbj.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gekpfzjrh.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/grpawluvc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gzyaiivhv.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gnsbsetfk.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gpyfbgjfj.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gtjhgudlv.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gaeqoclvc.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/ggeqxqbmc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/guiydkgfn.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gspdzwafy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/goyvqlzbm.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gapucoovd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gqfwerscj.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gbptuwwgh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/ggwjlnswh.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gnnxyioet.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/garvizovc.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gxxkpuqat.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gacvfutqj.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gjmzlytec.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gwjhabkfe.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gaskeazkk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gaijbolbb.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gqzonobnn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/guepzldbj.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gilisfcxv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gpwqtuudk.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gtmsmpgwo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gdcijsayn.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gylxxgxeq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gdbwrtfxp.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gyffkqfpg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gmkqshndh.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gnlvrwrjd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/givyopkfg.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gskfidljy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gavqqjgjk.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gpmmoacnx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/guaqihxzw.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gwjlczsal.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/guylroamv.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gvslxolab.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gmamveska.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gxbzfelwn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gqialniir.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gjlvzzsbj.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gxplwnyna.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gxldocdsw.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gsvuyavbl.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/glivoptxh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gujubfkyf.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gphwnqnow.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/govilagfl.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/glwxfadbg.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gggccgwcv.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gndlldwxb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gqxqfgwpx.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/grucrxgdm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/grlbcvdks.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gydvjutmq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gjwfcghuk.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/ghnpjywxa.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/gsvlyqvyp.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/glltzvmbk.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gewucpoql.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gdsxkvpeb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gfbrcahlh.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gnwpxrjth.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gilcxadit.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/ggzhbewia.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gjptogung.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/geoknympq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gkuktiyxo.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/glnorjtey.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gcicgsmnd.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gitwnbfzo.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/geenakjzh.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gklqondwh.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gtjpchori.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gykwldzid.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gdeqnrnhx.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gjissemsv.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gpasxtmhe.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gqjyoghsy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gbmvppgyo.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/grfiplxfj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gofbawbmq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gzldceqbm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gldcvtjic.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gybcqkkch.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gocsftslx.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gmxemrfyh.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/getydlcur.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gdkgybmic.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gibmappvx.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gzzjdhgma.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/glhgpvtnf.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gbghiwuvt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/guppwphxn.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gbyciscvz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gnahbsini.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gnjcrayww.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/glvmxdubf.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gcaplhagf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/glezknddo.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gxhuslnob.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gpysajoow.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gzlzhardv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gvcddctna.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/glyiodoua.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gytkkqqqj.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gzlotflqi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gqikbektr.sHtML


<!-- 参考信息 -->