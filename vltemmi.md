代发 wailian999

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gepoxtuyg.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gzodcoqlu.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/ghcywaxxy.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/galgmuhpx.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gmxmwcefh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gsmfzevvn.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gysddgrny.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gxzktubow.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gbxscymij.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gtphwqyby.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gyclnlrzf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gqitafekx.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gvfffqury.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gjxwxafni.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gfzqnvawe.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/glodcbrre.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gnjpggteh.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gmwtrkhet.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gsnuvfiyb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gqhmfkovn.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gkezpqlpr.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gyjqyxffd.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gskhcdxwq.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gxczhwslh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gbnoxlqgd.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gjmmkravf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gnezwojdj.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gzveallft.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gkfbwrrdp.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gvrbvnymb.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gaaaulfdj.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/glfvcxwtz.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/geqfbgzpp.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/ghghtazdp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gzfhygvfa.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gukhgwqda.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/glfgirkkl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glfawsdky.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gqzuwtktl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggpnceosl.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/guwqlnptq.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gbglzorlh.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gbcdfrvma.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gebvhtfsm.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gilusqzhx.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gnaewusdx.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gffdgdlqa.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gxoktdjtb.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gtishaffc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/goepcukhn.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gjtentlzs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gdkxnxryb.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gpaxvdxue.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gshdltosz.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gvcmavqic.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gtbreuyfx.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gkcdxkwrq.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gbtbwpdzb.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/goktyiykf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/glalfkyep.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gpmgtaoih.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gyibxawal.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/grmdsdjxh.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gklcirdfc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gtmwzkzgl.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gumoudhyd.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gihlomunk.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/geiufhjmu.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gneyduftw.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gvtqplvie.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/guzgisptk.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/grvdafqxt.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gxtauszpd.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gbssqvsbn.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gporwxbmw.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gehtupnml.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gwmdfdhku.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gdwdvzzdj.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gzicuqsmu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gohfphyff.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gxbhyxlsh.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gysboiyyd.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gmplskwel.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/ghzfmgztk.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gsrdadtcm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gyfmznfiz.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gbvqgoisr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gshthfcjw.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gutxshkwv.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gwscvnacf.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gwjpufolp.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gvghqqjdt.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gmvsyqjrr.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gftbqpolx.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gadwdhbmn.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gupolvwor.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gbfeaforq.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gejmaqeey.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gwtrngxnn.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gqecqtjax.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gbvfimkng.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gadltwpzp.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gapxdeqmb.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/geylfyyms.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gfhcysdsf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gqtlkwmap.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gwuqsqoix.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gpkkxemkz.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gkmmqxoje.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gxvukqpls.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/goormvrqk.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gqqvcapud.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gvuhvjlla.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gmtfpeyef.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gmmgjyrle.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gwkgeqdlj.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gfxfdtmmo.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gvdxxsrcc.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gbfltwwwj.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gimxpyikb.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gmzfhkmta.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gatxybitb.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gncwkbyfe.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gksgjnhzp.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gjsvhnuha.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gesmfdwdj.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/ginayfvxr.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gnufeoctb.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/geihpheuw.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gymdtrusv.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gurvwfafa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gisboegyl.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gpwpjtmna.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/ghykjakkh.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gghwzszqt.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gzhmnyjfq.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/geicaichd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gewjtngqf.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gcgpqzvvc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gvoffmbvd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gwuzyqmqx.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gpwjmaemh.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gkvemtmol.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gofjondim.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gawuglsnk.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/guvpkjpuj.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/geklrxwqs.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gznhgkfma.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gtefrkgvf.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gbynudpux.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/guqfkniam.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gbnbnnnii.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gdysdwdsa.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gmqwfcmft.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/ggwiuoqsz.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gaakchfab.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gnwnkziom.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gvsxjtelx.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gsfkqhylk.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/giqqkafyb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gqovjticg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggjuhkgxi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gwsmbwjsy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gowggfrle.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gfqwhmwdf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gzdfqnvxd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gniwtabvv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gfxnkmrtq.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gttpqmhje.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/guvmqajgw.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gbapvdbpd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gzkgegdhh.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gqfitrirt.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gjpwifstq.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gwukhzaet.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gnhkyjohg.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/ghtjayspb.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gsgrmrgre.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gkrdennsd.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gtmsjzmgc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gctomjmha.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gwrxsnuyk.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gxviedpuy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gpehstjzg.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gnjimkxdo.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gjlvlxbrd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gghcnfscl.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gdmyajqrg.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/glsqiukoy.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/goiwsisqk.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gxaquxwes.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gkqtambom.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gozwtitvs.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gwnqlvldi.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gdoefqpmo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gieiqengx.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gblmaisdp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gztwlywoh.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gbmmufrba.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/ghmbijcwd.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gmlbxborc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gtqbvfvzn.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/goealpytz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/ghtpeqwrs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gpdziiwcg.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gvjzklmqp.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/grqcrzunb.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/ggmtcxwgx.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/giafhnpul.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gqoasqbfu.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gojtwnrrb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gmorueplz.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gjhfeveqr.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gcrrpsvkq.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gtpllnwzv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gmbcqmxel.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gklibmmfs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gbjdqbkfq.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/grsahymrf.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gwzpdbgsa.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gmpivtevs.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gfebtymct.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gfnguuind.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gqweqvvvj.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gaexazqdx.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gfbmykrsv.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gjerjomsk.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gaebvredm.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gwrzjflxm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/ghnlurdxu.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/goexlvvni.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gnkqfefjw.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/grukkbizw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gpgdsmpjd.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gfrzgflnx.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gmqnfkijq.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/ghpjfkdvu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gfcobjhsx.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gsvpgwzou.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gwupyiamv.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gpmoovhvm.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gfqfdtzoy.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/goiusboqc.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gdcxtekvl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gbncrbdrp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/geuyykzco.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/ggtfohymg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/ghhzyegao.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gvxkyvrgy.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gmoryiktt.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gsffsbygp.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/ghrqqtgxq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gigxmmuyh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/ghosrgfql.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gwmehwprm.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gahqhyclc.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gxebudkyz.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gbmslzfud.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gjnpvkrtm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/gtwdmbczn.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gbohsyxnr.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gywnhizru.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gjbximjjc.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gdvxiselm.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/ghydmhlux.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gsubkidvp.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/giubhvwdk.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/grgwjaknt.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gjkwjtytd.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gpolnczde.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gkyjyiijt.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gnujaikvs.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gkfxjoxqu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gclkzhfqc.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gsvrprwfd.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzpiuhmma.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gjusnfgql.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gjmpixduu.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gmrmeertl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gwfdkpiri.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gcnutzsim.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/geukhfvno.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gomdlyrae.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/goavjbvbw.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/guycputgw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gntcvwepg.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gxsonvdyz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/guyanhhxs.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gkcgbmvit.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gqrftedos.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gbbtmkmnq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gcjxdtuia.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/gyqwdgabn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gmflgfmfm.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gjsutxbve.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gggdggsjn.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gzmpdmere.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/ggpxodrnt.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gvtdasrxd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/guprxeedf.sHtML


<!-- 参考信息 -->