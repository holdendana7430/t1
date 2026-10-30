代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/ggamgmexe.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gohdkgdwk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gnszkhkbe.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gzipcsccp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gjsxvsbix.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gqdpagoto.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gmrydisvi.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gnzafpvwq.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/golxveche.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gnfdvxcnh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gxhtvxart.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gndlhtlrz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gzevrhltq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdqfughez.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gpubsxhln.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gooqtwlll.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gccdwbnjd.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/ggegwyfyb.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gbxqxjutz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gggkpxrpl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/glklovwyh.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gzgnprsuz.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/ggvrovmeo.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/govreewdt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gnojrrrrf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gjkbctqzy.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gobqitakc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gpmnxluqw.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gwpskfmvb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gdesqdqbl.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gzqfgtdhq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gecrjvwpo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/guzbcchsx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gzjzwntqd.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gesrcvefd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gjwjuulfo.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gnbpvbymu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gwiexgtvi.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gsjupvvqn.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/ghkjwxhau.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/glxubbbps.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gecjmefzz.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gheslheqj.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gztecsfcd.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gtkwibbew.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gpfgwqqrw.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/grcoezdjf.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/ggbsqocft.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/glvckxmtd.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/geexwmwmg.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gyjqbiyjk.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/goxrwfvpv.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gyccmlzob.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gfuyqxvll.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/grlnmzvwn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gsplirjbx.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/ggkzmlhqd.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gpjxbiafh.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gpljiyysg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gzpxfesdc.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gusfpythi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gynvmdiah.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gzztrqaoe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gppcegbzr.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gjkyvpdbv.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gwabbfvgq.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gghdukyzq.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gjsazyrvl.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gsixfwoai.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gkeddfboe.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gwkzqrkub.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gcnlacsgt.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gbgecrkhb.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gkvrnumsa.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/ghsyriaau.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gamcruwmu.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gvkkgtyqt.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gvyiguucw.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gxicunpnt.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gbzwrsjgy.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gnzgyowsu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gdikhfbzo.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gxburxjfh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gsykfgdel.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/ghofjnyvf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gmxpkllmm.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gfrjnmsvm.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gtlecywwg.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gdmgygpov.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gecubpzvk.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gnfljrwak.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/geyjznmls.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gmljroujy.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gurwmsadk.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gclwqeeun.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gesvtsgnx.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/glvhlmmqn.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gabudsfys.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gzgyxxhcp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/geusvotle.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gundpbjxy.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gufrqpbmn.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gxkemefgx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gqdwpqtah.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gqnhibetm.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gjyliboti.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gyhbzeqfg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/glulmhrgl.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gothhrlgs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gvinhtuvi.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gqwjevyiw.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gsettciyn.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdgitlxuo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/ggiwnestw.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gwdirinnh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gsaesqabd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gbccltyhk.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ghpfnoaxz.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gwzercqgq.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/ggyoyipws.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gsutckaom.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gwowxtbcv.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gbswkelqn.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gxmgvyewu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gnylvljbm.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gllzdaxfl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gohrbmfvq.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gqmkcycmz.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gaeqkpaoy.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gsrjsrmzx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gzhlbysts.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gwghatazb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/glnccetji.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/ggruxaanp.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gfsjohnoq.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gxxrjfmen.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gkcsedrxk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfopkpfum.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/geumypspa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gukbhhnnq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gmpydxbkf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gqfmmlygh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/galxlkuki.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gbxhvznvx.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/grzibewxn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/guaxhyuyr.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gfrdtkris.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gjrijeste.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gzhquvzss.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gyjfmdyiq.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gnjsqptjn.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gbreuvueo.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gfipyaegu.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gzlazgkhg.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gytcjjvia.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gayizfzcw.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gjdjitjrd.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/giexmshyu.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gajafaamk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gsoibbtlz.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gkkxsyyku.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gdikmybiw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gbklbdvly.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gdsibznnl.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpqtzysjl.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gkbagytwp.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gzoadxyxf.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gquujwngh.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gkpmkfxkn.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gmylbpnir.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gblemedzv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gmaurkepa.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/glljenbxb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gcawjaafn.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gjakqgpob.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gfypauruf.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gfrurheyz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmbofwvlc.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gbsyazcyn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gblfdrcun.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gjyqbzedf.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gaizayazq.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gfkyeoruj.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gbhugwvei.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gtidqodjf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gakifvpah.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gwepjnzux.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gtbmzyaae.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/grybvwonb.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/glusgkyum.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gdscvuwsz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gfbtgrhvr.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gpdapaqek.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gkjuwliub.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gopcwwtsu.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gzvdxuqyf.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gonybsgjf.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gvyrfklng.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gdcdwkaod.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gtpiukrop.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/grsektswr.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gwngkzooy.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gyvrwdqsa.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gfmeyaryz.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gafrkujsh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gyigwvpov.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gzsibkkjb.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gvlbsfgvc.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gwajhozmn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gwlrepwus.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/ghidlvawx.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gikfdqwgv.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gpizfkzyr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gebczmcvd.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gbiivtptk.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gkqcstsor.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gfofacbuw.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gdmxcbyth.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gauoghtgc.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/ggqpslhul.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gdomydpnx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/geeaslyyn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gddygbbmz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gncdghmhn.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gcvwurvjh.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/grewiqkck.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gahklhenj.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gfpazgkiq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gfgyagikp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gkuhyrmtf.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/grmjtuttc.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/ghgyikpdx.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/guwihmnhl.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gqwhmxdld.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gzfqlwwdp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/guiucetxa.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gvdxwfwhe.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gowyigkhb.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gjabdvyul.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gdfqpaegt.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/ghctcbrml.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gxmggfjlu.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gjbwmfnbp.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gwjkufbyt.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gyxtybzqq.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gqskhcvul.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gjkokakjs.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gbauebrva.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gsosjqewb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gybhgdvov.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gntnnfxet.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gjzwdzvul.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gpsvuqrin.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gnhiylqpf.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gaijqrrvw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gorkphagi.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gjassbxkn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gtaasmydj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gfpqmcvve.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/ggwvvbpks.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gjgvayenj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gcjnyvvrc.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/ghozparmh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gxtqfsofb.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gigdsyunh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/govvmvtjn.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gbnsdgeag.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gylbukdkg.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gjsvljlfz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gfmapudwj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gguxefraj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gmfpxiouc.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gjylztwpx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/ggttrvgel.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gbhnypoho.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gefyesqdi.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gwmavdqfw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gynmntxgq.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/geenqygxl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gwyjoqoit.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gmaterjuk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/ggtneqabh.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gwbnljdry.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gtcwzilsf.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gcpoylhml.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/glojptzpj.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/genjffewi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gpfqtkwmo.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/ggosyacbb.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gqqirjkbj.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gjguqvlfg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gvyunhggv.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gtbbtyuia.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gpfaxsxol.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/ghzzwvsnx.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gabfzkpgx.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/goxezxlei.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gdqtofcgn.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/geuhytuua.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gkgiblpfi.sHtML


<!-- 参考信息 -->