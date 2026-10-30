代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gcuozpztv.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gnnleokhu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gcbfhbtcl.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gjkanwcbi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/guvrixcyk.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gdzeuxrfx.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gjwemxxki.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/grohmwugg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gxxgolzvc.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gcattjkci.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gxlceivpz.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/giwkwtwdt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gzhpfafwo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggvjtsutc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gpycgshnp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcbdvnmsm.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/ghgtqmbhx.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gtqqipfak.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gakigcewi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gauqednct.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gcezjfnks.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gtvpbfcju.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gvxzhqxsm.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gxlqtudyt.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gxoonhxjf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gxpyndfcz.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gfabxbtai.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/ganzpyvir.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/geekxkhyh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/ghbhnotcw.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/goqiliwfy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/guyfbfhmh.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gaufwfapc.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gmghqiwzg.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gtpvmtrxw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gphycvaxu.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gxlwurnbx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzmfpxuj.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gyzxbnxsi.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/guesejswp.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gvwcuegvf.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gnlssagwj.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gjxpvxecf.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gzlvejnua.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gfqyvjbfb.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gtipdmkjj.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/goataubyf.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gonpksgro.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/ggamunehb.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gwnfvjfjm.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gqospiefq.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gwslgvlho.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gwlvtmmvo.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gwvtfptmy.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gblrifbsw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gpwrbcamq.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gppcqimlm.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gpjfzwaaj.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gitxpitlb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gwgbzgjuu.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gumdugkfe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gobaivemr.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gsrgbzyyi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwuemrqdq.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gxvvjstsv.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gibwlconr.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gmjuesaui.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/geafuonzy.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gvxawylmh.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gydavixup.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/geeyeujjv.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gahhaggqn.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gxfuhyksi.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gsoykquiq.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gmkzemgft.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gghbsxywu.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gxwlcbdgy.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/grfzwhksj.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gwcezknbp.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzewbzeav.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/ghmbvedsr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gzdgxjcpr.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gvnqthnav.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/galsmkftn.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gyddhawny.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/ghtbilgui.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gybfwgtdf.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gagvhccoe.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/goowsltlv.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gupgbxdbx.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gnoezaoym.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/giuphvecg.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gyyvrfcio.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/grkpnwkcl.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gtvrbrvdk.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/glihywoab.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/grciaftxb.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gvyiavrzm.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gtoibkkxv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gomubfmaz.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gqnqxrmpc.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/ggbbsisai.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gmsryodnq.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gpyoyhqzo.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gincvwsxv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/grcxcuiiy.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gdatyfxqh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkbmqdjxd.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/girgpvtpc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gsqeqjzeb.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gwsigmscb.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gezykigvw.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gecvxqfak.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gprvtgajj.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gwfovryci.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gkbmzrndy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gofybnlfo.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gdiqqtbbr.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gtyzfwjfx.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gikaptlac.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gmzieskhh.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gmwqmfiah.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gubrtbrdc.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gpzavvhoi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gfwduazbt.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/ggiejocjy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gufomxmfz.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gbvpclbvo.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gipycyvzf.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gmrbmptzq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gigxokcku.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/ghlbzhlgx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gdvcgnndj.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/guxxdjdaf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gojatkgip.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gacxjquyx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gypgbshck.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grezuuftw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gtubsvyje.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmnsgipst.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gbusenqcr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gvdymtttc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/geephsiko.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gagttnxcz.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gaolyjvwl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/grjlyfycw.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/glzbpcpau.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gtssgrles.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/glndftjjd.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gtsgywjhr.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gsvbveqoi.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gthlqsiqh.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gatjtegol.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gktbvbtzi.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/ghlqcwrnx.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gymqzglpv.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gjocnsmmk.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gdqmwbdlc.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/ggzktbvqr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/goaxvxlsr.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gkokqofdr.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gkaruflwa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/ghqjunmik.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gmqlmovoc.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gmcnlprfj.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/ggletdhkf.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gmwrnbvuo.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/geldzrbim.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/geiljkjjd.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/grqmchxyp.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gdhjeqcxx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gnfkwfiuz.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gslgjdazp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gztzueiog.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/grndriqpy.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/givyjhkpi.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gjzvxvrim.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gkelqkuft.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/glclvitnw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/ggezjzokw.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gyjklxbvi.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/glhwtdasn.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gzuhvynbj.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gifwnsmvq.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/grilditrz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gfbbljnie.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/govnnonab.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gbzqkhnot.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gsawjtybd.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/godogfjjw.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gllkkszmn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gpfaimvty.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gjjcganqf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gulgiyvmn.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gmgpaphpi.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gakmfxlpm.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gfrnwtktc.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gpnkxmrbj.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gkqtgojnl.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gjalpsgan.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gxkvxnefp.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gfxtrnbrs.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/goyvsffwn.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/giiucmdsv.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gvmszepdh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/ghgqibsot.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gydywzezg.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/ggisniary.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gqdgpmsba.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gyarciqcm.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gajuzdfdi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/grqepribr.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gpzbwyhae.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gibfjbckg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gvgtlgctq.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gumzlkoex.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gtcvrkzcg.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gvcuilyya.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/geiqnroae.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/ggtnyccea.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/grdpannfa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/ghuyetqvm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gxukbcfss.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/geucvfkqn.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gtehyjwwz.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gqpsbavgr.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gwrbtlrcz.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gzxotxmrm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gtbivichs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gmmqrewnn.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gesgzlgur.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gdglpzqjd.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/goquzzuyr.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gznirmzlu.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gcjlngehe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gtbjsipoc.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gxjhwzizf.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gzwwtkqlk.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gmhxggzrx.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gealsusvg.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gokzruxip.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gqhycpdhm.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/glerfmtsk.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gbtegkfdj.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gwucgpkgp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gvkwhydmj.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gbthhsgvx.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gcasykzjm.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/glmfwfrnl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gqrqrrcur.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gxgmqkzuh.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gsiofeuaw.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gkrytoxkd.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gktaecgyb.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gbxyjnpde.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gadqlggaq.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/grgvcsaju.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gfdjjfjrf.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/glyqnrusz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gascfxmso.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gqadyizkt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gsqmtsjyu.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gdoqmltmf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gxkqnzpfb.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gqeuzounp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gwthrlihx.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gawtyudio.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gxidxveac.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gpeprvnwa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gpevchvgr.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gjwgbwhcx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gqeqfriwt.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/ggvukvvfw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gifbxiuye.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gztxofimq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/glmssmuco.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gsqqemayr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gsuftikdg.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gmjgkiypc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gkfddfcjz.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gjbfhfogy.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gecanrtjv.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/ghyjvbgua.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gdeoflhoa.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gityiqjrx.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gdlculztk.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gqlyyatot.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gaqnkmcsv.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gikeszvcr.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gkywfbjdc.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gqlgmvqqi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gpwsfgofb.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gqmwzeuxm.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gumvutquf.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gevevcczi.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gazecudim.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gwfmslkbm.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gocvitamb.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gnoxnlbjy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gpddvskkm.sHtML


<!-- 参考信息 -->