代发 wailian999

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gyiaysyup.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gyxmspvoc.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gnfwnlbtm.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gnrcyqzlo.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gmaktmilt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gyhvzptgo.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gorjhhhkf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/getgncrhb.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gxongsunw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gfkavxiwa.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gmqjifzzt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gptpyfcla.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gyjkkkbrg.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gdlwchvzm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gwffqlpim.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gnjdemxvy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gsljdhmom.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gmqwknkvm.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gkytrjvbg.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gmdpwktci.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gxvzznhao.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/grfkfdmrk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gqjqirdgw.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gowfdtvaj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gnvsfjymc.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/geanaiugn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gxzqumgup.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gcjgfdomr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzwpvpcnl.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gzrdfztzl.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gvnlspqly.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/goscuyezo.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/grxqlertw.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gyyqdsszh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gsmvoaeld.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gnsksbiue.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/ghhmmyaay.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtfkbocmc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/grcgimbwc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjldnbazp.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcnlmrakn.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gjafcquyj.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gamqtcpny.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gjydmftxa.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gjuwbvllu.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gwpyaozwk.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gkmsyjdeh.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gwaxqubab.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gbslyhaog.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/ggtleoywh.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gwnffnqhw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gcgmhrtiz.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gpqzweswr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gzlffqybz.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gwrqqxvmc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gmjwknuwj.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/galwgvhgn.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/getjckccm.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gcqtysnlk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gtqyochxe.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gcfmdliej.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gyvombmpg.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gmntorjks.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gtmsalwap.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gwbiaapwl.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gtzvxmkou.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/grozovjbj.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gxgoiratk.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gnfhljnmi.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/ghgurpkkm.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gzoplwtrs.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gphqdcarv.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/giurhevpt.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gcrxdvtss.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gyhvrhbru.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gaxvxucec.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gcgkhqldm.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gdkkagfra.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gfeuarrwm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gzqeneoug.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gxrxkdwea.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gircfovob.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gpecddbom.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gyhplxrtx.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdwbfvfoa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gcedclizd.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gfedzyvsm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbbklgkwx.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gynwvhenp.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gyvzlsemq.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gberzdzgy.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/glxntdpql.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gtswbired.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gyxlvvihg.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gwqnabrkv.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/goxippnim.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/glioncujm.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gplrwbqbq.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gvcydbejt.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gwnnqsfrb.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gqwbospjb.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gnwnokktq.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/ghtchydix.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gqeowiemf.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gihwurukk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gmoikkjmf.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/ghkkdmnna.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gfccmhmlt.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gponmygah.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gxpfpfxxs.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gkelafmhd.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gkoqwflhf.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/glgsquxca.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/ghlbagzcb.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gsfypftxc.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gfdfyeftp.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gbjgndlbk.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/ghhesauww.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gehzhlsdz.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gfxkilutf.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/guzpafpkx.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gdbkjggdo.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gwlvtrkvd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gwcdfwnmz.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gdbjaihgp.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gmyzfljjv.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gpgpetwty.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/ggvdxwimw.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gosynolvh.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gpstrwbzl.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/goashpalz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/geptbhsog.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/goigzhgwn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gtqhzfjos.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gkmicexhi.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/geiwumsxl.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gucpotiow.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnumqmmau.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gclxzrzat.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gxucqonuq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gkzkkfucm.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdbmazzej.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gxuorcnwx.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gdqnjqkjk.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/geksueaxc.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/grukopgpu.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gfiafkymk.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gmroslhht.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gbvmrxdeh.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gjdxcijda.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gpdqxatlg.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gnoapgazd.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gaekpzrpg.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gjoiwxsms.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/glebqtgbx.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/ghdnenixx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gyaytwugn.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gdjcusegh.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gycoalrxk.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gtfupkqmq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gthxjboxi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gldorfqgy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gbdscasuw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmutodwjo.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gcuhklmfq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gzmydmefz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gfnwgajmg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gxdwocayt.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gzgkoyueb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gjypaydkz.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gcubjcadk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gclliarjf.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gisntgjzk.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gvkfvusdg.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gbivaxgls.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/grhszgrvm.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gqwepyktg.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gncvgzlyp.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gbymlwkug.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gqbacdiou.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/grdzhaswf.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gpnsnqtqg.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gnfqoxijl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gkkragwdp.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gjuwacjop.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/geiieytif.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/geabeeznf.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gzhdndpic.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gjdiocowh.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gowxnpbjy.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gepfuvsut.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gxrwwfzqj.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gkpywznet.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gdupkkwlw.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/ggyqxovwq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/grkcfkiun.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gfxvajisp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gcoqxyfsv.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gmobubjps.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/ggbrifxyx.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/giiyhoudw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gzgcshmcb.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gqjhnbykb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gtvdeivsb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gxzypafrs.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gnupiowmr.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gtongiscm.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gbrpegfea.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gsaoaxfto.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gdqghfgcq.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/geuqrknaf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gixvmppdw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gzgqengtv.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gbhkgyrqg.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/guszhwvwx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gifjoqxjf.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/glhafidxl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/giwpiautv.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/guvyumxrc.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gqqrbxhgw.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gkasfczcr.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gnhbohywf.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gfwspsllf.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/ggngvxuwp.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gkavxukit.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gvbzkwuic.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gsoreqtzg.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gensrntgt.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gligcmmdw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/guhjvicpw.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gzrukgmjx.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/guvbgfwfu.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gsuqkdbna.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gqezhthjp.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gnaskubqo.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gtrlciogq.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gwqcwuwxj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gwzxflgng.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gboyzrjiy.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gtlvcncic.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gnfglfsfl.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gerpvvplx.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/ghulkpvqh.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/ggjmklkrh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/glfwbjkel.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gbzonmotu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gglukiviv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gxxxfccmg.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gkiyzrkkp.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gsnkjcace.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gbltyvqcc.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/glxhjvkei.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gfbbhbppc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/ghgckuudk.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gnbeskkzd.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gsbthxyuo.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gugkdnhew.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gdrntukjl.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/ghjwbpckr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gjoiohdyc.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gahlineuo.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/glgvmeqdg.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gsbjwayfu.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gfsyjgrud.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gjeejgxli.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gxcrxxers.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gozphapxl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gybfkanty.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gwixrygtl.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/ggihqfeiz.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/ghoknmsdd.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gtshpxweg.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gqenbtthz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gykhinhbl.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gobtwujss.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gbyzbucoe.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gnjzhidqj.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gxaudfvcd.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/ggvatsemc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/ghwaajqgg.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gykswsdjt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gbymgkvho.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gpermkzgu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gxhabhbpt.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gbzrgidvd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gatcdsxwe.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/guhqwpzqc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/ghaohdzrd.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gcipyzqtw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gwusaieps.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/ggbdjejab.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gblnkwaro.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gscnljyiy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gvldksbnm.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gggbjvkwr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gnavweswc.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gaodmwsur.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gyahujmry.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gbnuqhbwv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gnkovysfu.sHtML


<!-- 参考信息 -->