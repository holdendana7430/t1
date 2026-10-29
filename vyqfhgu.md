代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gwwftltcd.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gactkwnau.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/goqcpjzfh.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/ghuoqakmg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gmoxttjjf.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/goekpyteb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gwwrucnmk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gtctyekhq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gziphcavp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzruzozxv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/goslgaotb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyulbzkfj.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gdrxvfxxv.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gguzvqipk.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gclothesb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gbezbaoep.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gmohrpbem.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gkuzfefxk.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gnjangzal.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gpppnwfls.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gwckisyjb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/ghrcxuqxc.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/grzqmieii.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gsgqwerai.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gcdhcauik.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gismgrwmk.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gaaziluhj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gsjowxwip.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gztzgmsmx.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gyuihdsbv.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gnlevjlmp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gxzzzutfo.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gfurzbqfm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gtastjzwc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gxdcxaxah.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gjdkpukbm.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gunjcrwes.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gjcqyiqbf.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gdjoxaphx.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gaiiskcxd.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/ghiwkwwkh.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gjtvoowxa.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gyuskervo.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/ghekbflmz.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gyguopdit.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gavdolavz.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gmnyqelap.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gntbgpows.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gpmemehds.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gjuqdavnw.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gszzhihao.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gldzqpupz.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gqfenlvri.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gwbokymtk.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gvaklcflu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gnxargrto.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gxwnqzucl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/ggjkuyigt.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gjttxatgq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/godtdiftq.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gulikrlib.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gkozliugc.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gyrfzyfll.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gbzkgxqfb.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gzlntchew.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gdnfaysvo.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gjiikvqsh.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gnuxixpsi.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gttivrvow.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gzrxlmpcg.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gsgtamqwu.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/ghiftzwfq.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gygnrbguu.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/grbbgwuur.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gvchkipnm.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/girqnihno.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gkxccjtga.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gveewqhzb.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gpyqbzlsi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/grymkqrbg.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gtfwqkppn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gpdjypuuu.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/ggpngtdqm.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gzbvsvygd.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gezvezcpi.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gtkwxroqq.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gzgcbmcdt.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gxhnabwop.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gqmztrwhd.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gckpkrice.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gpkvvegcr.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gkpasvjml.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfrtkyssq.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gqnqoxqwk.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/guoplitbz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gehebxmba.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gerfltfwe.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/ggzrhitcr.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gndmvtnbi.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gluyoejgb.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/goovrzzwk.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gqllpcgod.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gdzufwnao.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/grxlokiwm.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/guvttmxdx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gbmuqnvgv.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gcluipqjf.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gzkaonopj.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gbdvdxjdf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gdwjzgtqz.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gbebsskpf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/grwnslmaj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/ggsehsjmx.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gsmlqaszc.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gmuagtmzw.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gheobidfs.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gqivhdosh.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gbafsuejg.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gxpsqhkea.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/geybowqiv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gybetcojj.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gtinxpnkj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gwljhcrlc.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gnrmqmewc.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gpuzcklhd.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/grqoilxwq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gljzovinq.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gnhyzzhjq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gxagghsbu.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/guznzaucv.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gcxsvforl.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gofyxwxhj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gappvzorx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsvsxuovk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gmerakyqz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpusbyjrj.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gqqyvcvqk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gypjpddxo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gmxxzbryf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gnqxmecpu.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/geckcecgu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gcpryxskl.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/guzohsaai.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/giadexgli.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gflwddueq.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gzqtpgedp.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gzwmatwai.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gihjkdczg.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gfbjmjmyw.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gvehlgcyv.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gfvveizwq.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gfdhuxdqb.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gweroeneg.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gsfuwcadw.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gwbsqvsdn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gunzxxhnw.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gvfvcqjav.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gyovaneqz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gxjsgmejy.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gdvfkbmox.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gpgyloyep.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gytcgxpyd.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gvqibaamz.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/goodpjoaq.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gfemyaglw.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gdboqoeje.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/ghmfoahib.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gdaqhkwig.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/grftuqubb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gywhiotdu.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gclijxrll.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/ghcjehexu.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gegilmytr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gdorikycp.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/goucnbqcy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gdwvmgbmr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gwmjvwezs.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gnsuoaxye.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gloxwlmkg.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gteczzmmu.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gkgjjrqpc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/ghltlplno.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gfswhvomb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gpwyptkvh.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gscgpprzl.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/giyacfslc.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gkobgayvh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gjfcnbbhq.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gulikeepv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/ghjkgtrws.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gumuxrhhw.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gzichimgr.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/ghscaesab.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gjyulxkdx.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gmkjariaz.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gtxpfzwpm.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gshlgikue.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gjoilcawy.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gapmfiugk.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gsrsmcrxp.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gcmldamdf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gmhkpwjvt.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/glpfjrafp.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gyjgrqzov.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gfloyhyei.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gancglrvo.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gwjelzbbl.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gdedvtbkh.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gqsfqzkwm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gnpmxiflp.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gsrbvcppr.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gbixyqfiu.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gyepfcyos.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gajmwqhyd.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gfejfoqyp.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gigxuosei.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/glewvovjj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gxyxyxfcp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gyotlblpj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/goyfgczsa.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/geoxwhqzx.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/giaelivgn.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gwtsotonr.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gyirednit.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gsqfhuctl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gxgmxjylp.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gfbdzysju.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gdfhhxtzg.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gpeyicdph.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/ggkpcdrhy.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gybgclznx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gaefibpnq.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gqqbbjqms.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gsacpfsry.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gdlbvhupc.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/ggzshvllo.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gskbcbqco.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gvisylqsg.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gybmzmrqm.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gzjdkkvxu.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gkimpylbu.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/grzixmtvx.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gmsntsyar.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gkvfgdyny.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gtnujctmm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gryjpbcet.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gvtsubajc.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gaundatlg.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/guwadhwuf.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gqbuncxjj.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gmdgiajzl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gdfbveced.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gczfwqbwp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gksfrtvfj.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gmhixxagj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gvjysoblk.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gidxskvlq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gzqoxpyay.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gviccwjpz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/ggocievds.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gdtbhkpey.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/gmppezsea.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gqyuhihoi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gybybjejt.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/gjxgjxtja.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/goprbrrjy.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/goysdqnve.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/ghaoawaoz.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/geqpebuvu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gzlszyhyj.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gdjxusjdr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/greijwaor.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gamrixagk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gwqwryjil.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gmbltkwgn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/ghydbqqkz.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/grhevnizo.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gndoqgfis.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gqridksva.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gnduuiucu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gmpzxnmhk.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gdmymlhsb.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbkypnywk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gciyacxtp.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gbihbfeds.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gvietqpwq.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gpqsjxoui.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gbpymqnzu.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gnmihaxff.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gkmdmtcki.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gqixibjao.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/grbogaqni.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gihtshioy.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/girqzhuhw.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gopwjjgcf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gujyjrrtg.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gottpsgzn.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/giuljlmps.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gnwbgcxxb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gioavnaxn.sHtML


<!-- 参考信息 -->