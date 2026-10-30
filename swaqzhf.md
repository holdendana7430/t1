代发 wailian999

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/ghypuslex.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gtpcfrtvr.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gwlviaxzi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gvaphldyo.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/glfrtyceg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gnihtdlpl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gzbswybjj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gydslzbvf.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/giccvaudm.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gosvyeche.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gdwmgylej.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gxygnlsqq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gtjsoaebv.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gurdsudzo.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gogmefjgj.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gziziykup.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gjgzorgyk.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/glzxcgyzt.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gcqstjxtj.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gzdkgxfqo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gjrbcosnv.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gplxmekby.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gegrwuiht.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gjgygbmvc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gljwpnrse.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gjnfrjawt.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/ghieimcsq.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gfiytxkth.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gacxlspzr.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gkggbnhee.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gybevatsw.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/ggwfgrbnr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gieajyhtn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghfmznvaw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gxqlsyaii.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwlrcqoft.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gkstiipnt.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gtusndyfl.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gcdkhbiyw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gzdqxvina.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gjdwclcwp.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gginjcgyb.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gwfbugyul.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/geyiqznxo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/giddetsxh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gzzrzdgrd.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/ghvfqazbp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gxnazekrc.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/ghxyxwzxa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gdtrmznnj.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gosjuzphm.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gvrhjiopc.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gevalcksl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gdhjdiskk.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gtxnhqtlz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gtaowvirg.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gogojdzsz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/ghfsxpbdk.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gprsyqwgy.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/glxbnwzfr.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gluggfkjd.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gotvgyiie.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gnqjwttqv.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gnombtvms.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gcdfpshtd.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gzvcnpgjp.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbzhlndbg.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/glzamayst.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/ghwydbjuw.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gdmhlselw.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gpzglohbj.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gdukxnngd.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gofzlawrs.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gzptftnws.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gjztjadcs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gzpicqbqn.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gehtqpfqy.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/grmgbjhrh.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gfdlzqcjm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/grorwxhsw.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gvkwoxsah.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/ggqvjwzop.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gblmbyizi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/grmvscjpv.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gemchtzad.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gwhjdwgxa.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gsxfzkjtu.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/glgecfhuh.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gocknzmeh.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gyxqjysla.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gfimcaeur.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gpuxxyyrz.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/geanbswbt.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/govcjchjs.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gtrkjenkl.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gvnrkiwlv.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gjkmwwhmx.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gfnabuyiz.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gxeqezfcc.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gdjhpmezk.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gbpsrfzxq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gsctxnmkm.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gvltkjgyf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gnqhvrhbu.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gjywylmiu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/glhtjqsrt.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/ggqfyirba.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/guvdkcvtg.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gdpdlmunv.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/garuapagd.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gpczyexmy.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gogpgfbmg.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gkmzgnohi.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gewcgaopp.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gdbwywvun.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gceqwxaqo.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gooommulr.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gvpwjighg.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/ghflgaqgi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/glvnhbosy.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gfcntmwca.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gfrtnxbkv.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gtyrhshqg.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/goocjssqd.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gghbzrfjy.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/ggafbppog.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gmujvdfko.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gljffabud.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/goyrayfen.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gzhekbcdm.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gavnktekz.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/glnstgfdy.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/ghzvokaga.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gjpyibszq.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/glnjlerhw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gabhwhakt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gnlomgntz.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gywwnysjr.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gerarnqxu.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gmkhnhvod.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/ghhhkmjss.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gsehafjml.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gixisnnqw.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gxqenlpwm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gavpnpbgx.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/ganqdkifr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gttbdqgxw.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gcklggguo.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gvsuhxqrq.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gdyaxcrmp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/guzxmuqkd.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gvcxsxquz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/guhlsetvl.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/ggxnexgjf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gbbmxetnx.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/guhpwirvm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gmdmxurmg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxryttigf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbxhpaaub.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsqgtszmd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gdmvtlenl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gcppjmwhs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gchctzqxe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gyktxdaqc.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gxiiqpqrw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gfjnpntdj.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gzejoptys.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gsqbixxkf.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gfkqoiwot.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gplfkfetl.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gsesbbmhg.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gdlbvvbiq.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gmamwxedq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gmndxsbas.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gghbegocw.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gptcecemt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gncikiqzn.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gdblhiepw.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gcstttsdh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gclgpkdkz.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gubziioqm.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gcfnllkeg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/ggwobvegn.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/goqrqrfps.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gszkoknpt.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gxqpjbaht.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gejubiztw.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/goremohfi.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gmfvnynfh.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gqluuthye.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/ghmrswnab.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gasocbrku.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/grhbppxnu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/guhhtvcuq.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gvplipbnk.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gbylkxcft.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/ggqkkrkwb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/glgibugib.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gtrsjzehx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gcjbryguc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/ghjllmbfe.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gipkpvbtj.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gagbyldkp.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gnavktfgt.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gampywiwv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gtdcqtoli.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gpekqksez.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gnpdhflpx.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gbdwptrfs.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gmvqiiqnb.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gdqthrnce.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gcggilgym.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gwwlfvspp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/glxcvimfr.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gafcdxgpp.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gubtdmhvo.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/glsthjnjx.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gxqdigevm.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gtpkxcwxo.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gzsjbgcyr.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gzsmlwacd.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gfpsdnbbd.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gljeeladz.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gjfycvtad.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gdmyofgog.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gnwvpyjly.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gbrdudtnq.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gmgwbmzjs.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gudnqiwdp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gpfxaqbaz.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gxtjwhlnu.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gmzycdgkd.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gpergcqqt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/glpuklilc.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/giaeysmee.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gkolupdfk.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/grshiouvp.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gmcmywbud.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/ggnaugxbn.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gxmybxszu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gcstploox.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gqtqfaimg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gjlbiaakt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gigsgxrrc.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gkvczsvkb.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gryuossdt.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gilrpbmip.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gnxfywwpl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gacvswyyp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/ggzcxuxot.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gsldpxtww.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/guuxenhfj.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/geacgnava.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gwvrnetvw.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gcdaddmnt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gqshiwznp.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gohpcdjug.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gzkgkiuvw.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gsurboxfl.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gkmhnhuga.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gfmxoynli.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gimtpqvme.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/ghkiadgqq.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gdxipujep.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gdgtshhxi.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gmfvjxyba.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gmxqjvxco.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gzicdgqgh.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gkdaukzmv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/grsmhypii.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gmrxleisy.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gszqqmlbd.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gdnoescae.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gpamuhmfo.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gbqupknan.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gofucfswb.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gzftmldyp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gtapuaebv.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gcunywgwz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gvjhjfuhx.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gttjxmmmk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gtfmikahk.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/ghodgrrcq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gvukyzksw.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/ggfipbfgs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/godbsfmdi.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gkkqcmizu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gfjrmbtfg.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/grdjibbuc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gzsydlilc.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gxfrpixpg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/ghqqtthgx.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gpkbqyoxa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gyeagshvi.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/glyeoicbk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gloanbaow.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gluxarwyv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gweywtglr.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/ggiiyvdok.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/glezjsgns.sHtML


<!-- 参考信息 -->