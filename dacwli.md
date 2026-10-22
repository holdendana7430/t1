代发 wailian999

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2azigcbdl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2aottqzzx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2laujvowz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jjsipicp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2prtpzysk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2snpsuvai.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2guxjxtnr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2euizkbnd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vsdhklex.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2aesbjilk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vsxcyibm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rshretun.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2xwbtuelm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2indiggqh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rmkhfzxb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2olpaqswg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2rdsbobum.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xzahhrui.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qmfmaomu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2mpzkrivt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zsrwwuxc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2fkvsjlux.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ypiiepda.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hcbntvep.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tfzryaey.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dwzxvsuw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2oldzzguo.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2bqfvzoyt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hfdjscpx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mxkbgkpg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fjrnsthx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vynhyufp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2swkvuimk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zcompnxt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2edubnfov.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jfmglwwt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vadxmbgq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bsaybjnj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jfutwfqm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2puybjeta.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2pwewdyud.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2tsenjnyw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ryjlewmu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dqlsymyr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2wgeydqrs.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2bpzoxolr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2pyodojtt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2bpaaptgw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lbwbazal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ytfadsbb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2lgipccas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txeywzts.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rewonwml.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2glhetbhj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bnamwjdk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2flhyjqfd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2gvhbaulf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bprgyywq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vtadgyen.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mcqcsqeo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zqtqqfxv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2xflnaufz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2babddhvy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2touxnjjt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wdigyyaq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bmgotwpm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2bikbmris.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2suzejcev.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2jobyqyru.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2cxthnlcx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2pvvwkxvw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2srnxyhse.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2spsrloed.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2cthmpads.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2jfpsflmp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rszfwrkq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2fbzhdffc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zylxouvi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2phicvcis.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qxizwegi.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2jsbqbvds.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2dahcvagy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hsjrilhk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2akdkgfto.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2gkbpgjiv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jogrudox.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qrrcinrs.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2tfzptqrj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2mqxchpzd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2guygkadt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2nheuauta.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2zfwfblmf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ogvfgxxr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2cwdqjqnh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2cpooxkyy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ehbvxiig.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rsbkpbqy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lzehmedc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2atthhhyy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lbwjtxyh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2diyyancl.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bsaowapn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2sarpwapd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2cnarixxc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xzvirini.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xjxeuywe.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2klxgfkmd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ogrwxwht.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2pqwysgxt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cidybaag.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2lyxuuwte.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vursqgif.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ppqdvekh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vejawwlj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2brzmyadx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xnkwmeyk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rlscgyqn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ubddvmco.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2cxfjjhmw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2hzybfbau.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gjavesdz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zupcydqa.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ftakkhyr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2mgkjjlly.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mpxowekp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2hmnycdnz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gezzmzrh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ktsgxwvi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eubdxibq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vtwyzxxa.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2enncrwvm.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2mmsbyeig.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kaitbnoi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mhwhlmvp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2gnwovnwo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zveuuclc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vvjnvyee.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2lhajybxs.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2losdpypy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghuckmvc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2fqbnxhln.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2fnpzujpy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2iqehyoow.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fygdxbgq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2djolpodp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2anxjnhki.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2kisfyuza.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2uhppgvfu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pezjvnyn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yetdnlji.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xvjkfuie.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2eszwzphe.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzssqmkg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pedhdyps.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2utchtlom.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2kpnemnxm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zvimplaw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wvouuvbf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tcdxpmtu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ipecxtbj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2czxtfzuk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jwujuwqh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wuagocks.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2aytkmcao.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rjevisov.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ayaphilc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kygkmfdq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ywjtlsfq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2gwwratat.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hqcbrmfs.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mtnqczws.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2lqsluqry.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2uogruznv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqussbcw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xaitrmfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ynyumiwj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2iksxenga.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2kurgqxuk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2pbvtifvu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hymkksxo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xfgzmkmk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2jljbewcw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2hgdtfqhj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2bfuiqscq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ynsbawwk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2bwiiejph.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jvgjjxil.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2janwfynu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2yghwbtag.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zxtgoulg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2glqappea.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qbhwybzv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jhydwgjb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ttyxeouq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2qmbcoygd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2rxywmszs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2mmkgabnd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2faqleval.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gtzoltdq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2lfucqopg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2nofqizow.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2uqrhgjgv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2prppwjfn.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2kcvdixky.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2rsvavdod.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2wrdpeiie.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dnvaiuay.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2nammqkky.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2njyhjvtf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2etmnxyme.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2omznpngk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2buwgqrbs.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2lysrwwbz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2tlwhgfey.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2dpopqnnt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2yxaixbjh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2xpzpimpn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2cblbvjfe.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qvdmqdjr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2xpqmrhvp.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2lyzswrgi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2yfvbwbxr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2cyfffbgu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2soievsfy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2mqdxnbvu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2bzlqwcdx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2sjbdplhb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tzsrlubx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ufdxvfqj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2gxnznvmb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2lmwkornj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ugyxyrkr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2oazlgucs.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yxbbznoo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ggjuztcl.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2amjqlwqe.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2plluxgsf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2njpnrifn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kycwakap.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2jfkjdmts.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2tgfiqxov.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ddtflnhs.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2nvszknwk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2vfwvlnoh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2suledwjf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2qrfbbfqe.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2pnihcflq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fczgzivy.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ynhhkxpx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2iutmfbmx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ugalzrbi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2gyvwpxac.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2juqoxjpu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2dtrumlhq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tpgrwjms.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2akqakcuz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ykkhadzg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2hqhobxag.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2xqhobbud.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2klzqdmwx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zppikgdl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2sjrhgrnp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2amicuywu.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2iuqmsaqw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2hehopinr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yubaqbko.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2cegrzkkq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2blbeluap.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2akwxcity.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2qlntukee.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xgpjtwuq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbnrbxdy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2pmqnnrzy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2vvbcszny.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2wpiqymdn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2fiiqccso.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2uocdleur.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2mtwwnkub.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wnisxlby.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mtjazwgm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xzqwshpc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ntowffhm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2azgffcgl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vbqzchzl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2giixlzat.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hgvruvgr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ylxeshjh.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ybexjebe.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xlupwuze.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2cbculsoy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2junbtpno.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ufrffpyg.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2orpvqjpy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qdtdqies.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2wiuxeatu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sdnnjbyc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2sbmnsyoy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kurvrikn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2iqcdhvkb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2rglneqwn.html


<!-- 参考信息 -->