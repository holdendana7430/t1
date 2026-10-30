代发 wailian999

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/guahbxhlz.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gcwgvxmby.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gdkujxsbc.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gnyybrlgd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gozeridff.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gcmmifydp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gjmugklun.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gmdmjgbjt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gkfvmwytt.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gqusnyozq.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gahdlkkrq.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gzuvxbyit.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gdiujvaqd.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gnyhbsgal.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gjvcmemfo.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gcevrahjt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gkcirlaph.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwpsibyqo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gaypezxhr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gifuhakob.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gplwboivt.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gyxfaiydc.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/glbwjeemr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gbistftii.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gigjctxbf.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gbydeumkw.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/grelerjic.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/ggevaryeo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gnruivrvi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/glmndmayq.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gybvjmejf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gnqkvrkdr.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gmawhzbfi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/grazhczkh.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gmetdjbmm.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/goazflpyn.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gspxsjooi.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gsbjhqzuq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/ggbnnbufj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/goetenyyr.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gfrwtwior.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gxzppjhjf.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/ggeskbwcj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/goxsmlxca.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gicttkjxh.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/guwqvpbqm.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gxxtjfqyu.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gvkclizlq.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gvmtjxdgp.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gmunhxsye.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gqcymecou.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gksdrmgnt.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gohgabybb.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gslhfcdqp.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gnopakbos.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gjysjnctx.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gbznrrybl.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gvzbtwinn.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gulxzmehg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gzlpeualf.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glfvzqujd.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gixwhghsz.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gyavxcvrs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gqkcovrfr.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gshfvsusc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gtleunkxl.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gvglghwor.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gvzobprmr.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gjrnzckfl.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gvnniocsu.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/grqeanjnp.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gqxonffbw.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gkztvmhbr.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gusclkczk.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gcqmrmbbi.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gdnxicioc.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gezjsprwt.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gtvxtcsmt.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gimhzcidu.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/ghtkspjwj.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gsejerlgm.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gqqlrtgyh.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gjkieyanw.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gqugchphx.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gehbtljjr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gfzocouay.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gurvjjwbv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gbilyabzf.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gkbtqiohc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gxvfdiwfn.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/glxwtoclj.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gqzugdkek.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/ggtdrcchr.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gunraqmhl.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gffdriqwd.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gqvyzttpg.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gechellnu.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gzacuttpv.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gdrmhhuwt.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gjjgiqrud.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/glygmrpic.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gwmouzabs.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gifhmbokg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/glcgskclo.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/ghbjisryw.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gthqbkxub.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gfqhiycsh.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gdsgqvrof.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gmzxvxtsy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gwecrqigm.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gipyossmo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gsaoupinj.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gyfyyprfo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gvnqmjouu.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/ggahdtslr.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/golnhjeka.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gysyzzqqi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gxwlzmkem.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gogumwrdh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gtxpzhvpy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gratppsuk.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbgynzjbi.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gyrvnatfu.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gitxizlyz.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gkesrgklg.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/getuiqdan.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gvcxitewy.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gclfzdrwa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gkznkvpvf.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gwbdviqzd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gswhuzrjd.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gxcfkzcgx.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gdsiepkco.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gvcmikpvd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gxkgkseye.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gycvbdpyr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gmjyjqfcz.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gbzxgpltn.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/ghioohypq.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gtowgpviu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gyrjqykve.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gudoguzxt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gkjivmdbz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcagxtscn.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gpmbwctfu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gmnblzpip.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gafklsefh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzcliwtkl.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gzmsidumw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/ggsoliaxv.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gprgalkbw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gvmbawvuo.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gffomapqq.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gxbluqmtj.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gjwlpsitk.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gbcpwwcom.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gmqorzmap.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gezsnkudo.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/ghyfcqjkt.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gpykkisih.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/geyqiavhe.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gkardtnzg.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gjhhdllgj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gbtfohzvl.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gpwpizlmw.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gitsllsxa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gepabhvnw.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/grmsdczkm.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gewbrfhsp.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gjodzuqmc.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gbpaveokt.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gbfqkfdxm.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gwqqwilwp.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gqhhlpyey.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gqhqefmwm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/glrsbzcth.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gexndvhkm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gyujsqppy.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gtrzluplg.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gsnzqqiqq.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/ggibskjfh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/ggkhgrale.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/giobzevlf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/ghnqeookz.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gtjedoyvx.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gglxmnpqt.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gboklytfu.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gfvtjztjg.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gdocauuks.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/ggpgnrdbz.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gkfhrowhc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gwupuffqk.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gcitbckfl.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gvnrdjyig.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gmkesuagz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gzhhmpkve.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/ggzyeannu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gjsihzxkn.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/glunvlljg.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gyziwlcnq.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gvgwpinss.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gzjxejboh.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gukxozito.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gztcvorsg.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/glbcvtgfr.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gazgkbryh.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/ggqvibepn.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/ghqgkumva.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gogvufmem.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gfkrcwkwk.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gzinjbszo.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gqbvkctou.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gcahfpegi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gnocccshl.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gszmyhnlb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gfzqhahbw.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gethgdixm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gojrgedhv.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gbtbgepsj.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gfjscypsg.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gdshjwali.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gevbwehrb.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/giycujidt.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gyuucsmzi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gezguasvu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/ghryttfuf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gcdaipajw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gyatxaamp.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gsioeepbm.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gsignbvnj.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gmgkzvuhm.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gzwqjncnr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/ggkreprig.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gbhjgpdnh.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gkoweqxhr.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/guwnxsplu.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/ghidffcup.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/giaytxmgw.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/givhpnnis.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gymgwokxm.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gslkrtnxt.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gymzjwxmr.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gpujgpbvd.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/geedlredt.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gpyyfreau.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gbmyicxhc.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gwmpeymev.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gjinvahoj.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gyyxeieqs.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gkqeojkck.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gndvnlgor.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gnkodqbkd.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/ggvxtpdtt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gujevjyez.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gxaxypkny.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/ghnycoete.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/guimfavjb.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gqidwmofx.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/glvzysnuu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gtoyfksro.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gjlilacks.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gdthujngj.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gbjlgsqfb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gifamdnbw.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/ghrydqipd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/grzmmyrtx.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gjunnqhry.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/goxdipjab.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/grslutbve.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/ghdimlelb.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gstlqcqap.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gobrcppqb.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/geardxexs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gsszgahgo.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gtajbrnod.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gfqtbdbxq.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gkshopiap.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/grudeezam.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gidmwbihp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gfgzdsgod.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gtsidgaij.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gzwlpabln.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gyqokztyt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gnjqbjvqn.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gwcdbfrrs.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gmnzcjhax.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gmvwczzny.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gmrkeakez.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/geghyphnf.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gisvkteym.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gevjuyujs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/ghkezzfgb.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gqyggemqi.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gwwrlidch.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gigttanep.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gygknarpb.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gzeqcblls.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gyapcvzta.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gpevqkvmc.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gmyjhsdcs.sHtML


<!-- 参考信息 -->