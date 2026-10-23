代发 wailian999

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3waklxirk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eikvcnfu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3lxgastvy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xsuennhj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3zwhttdcg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3yvhegovg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3berijsyf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3cgwkrvbz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3qnzeeror.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fchfeqoc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zhebaasg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxfbrwva.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kjpbnbhp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yhhqfajl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3wcsskqms.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lkgktzmm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3aglmzwua.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dvjpfzzn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ecbutrmc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3muarqxof.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3peacatli.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xtupxyqi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3uonkzydb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3lzatykdt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3iqfcisce.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3eqtgukus.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxmbcndl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3eqiajemt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qnzfxfhr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3coodqwsg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3gcikcxbz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3yerdqldq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3leuiwoio.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3truxpimc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3flbowigp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3izrlehgt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3zisstplz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3sltzevok.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bntnyswm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3jldjtsfj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wcxqqfoo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xgxpdyzs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3unwlzczk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ifvjlihi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ewfwhpij.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fiosvcre.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3qrnakjxz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3zrtykhna.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mprdurzu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3auzkdlpb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rhwcrola.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3iwkbfdmj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ykjdwxpu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ivkmzsrh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zvbzwlmo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3mfqvozax.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukkwpbav.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nabrdycs.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vktnbcgq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ulqaepls.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3dfwbmpnf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3skzneqri.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3kpwfwhci.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lzxbssza.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ctzfritv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmvzjrug.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3tsyahdxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akhseoem.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jzatnhjj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oxhhpvzs.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wontqoah.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3cqustjzf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3sirauozg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jsfyuvlp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tewarrqq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qmedfeyv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mmhbxxnl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jlybuawy.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hbcdznqt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzjfpxrb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kybgljgg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rrixxzty.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3swfenmzo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uletrban.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fcdmvtez.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3dtzlrwsw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3atfhtjhx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3verxsbuv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3bvpljbyp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3mslaubrr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vtrbybju.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lqbvhubm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dijqxexv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vebfjxyf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mhhfpazr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pdupobol.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3kexkcmdk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hsaixlff.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dhlddqaa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bkduxsdl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3htpeunht.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3bcemeofb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cqndpsix.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3vjmsfrqm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3sdlrncxt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3sfesbmqf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3mcbkkdyj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kcxxtrzy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3evbpuifl.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3hqffabjd.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jrugkzvm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3pinawzgd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mwrdonlt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3hzpxlxaa.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3mpkgehwb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lhgxhgaq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3pgyygibp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3woqersrm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3fmnazxgv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ucnbumpe.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3byuyzhay.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3bhcyoyav.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3moyxceew.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3sbvqksnu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ygdbciqp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pusrqwue.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3czgncduu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3trnwcybg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tcnjdevg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ixkeynxt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qylpvqmz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3dgvysvua.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3trxhvasv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3jgmdwwsd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3gbjnoyjz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3rcufvdvc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3qeezyszc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hniljdfr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3gzumrbiy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jjidupvo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3waxrcsau.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lqhtwcsb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3lnnkrkne.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ujllirad.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zyiujjfe.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3nrpcdryw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ibqclfaj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3vxoplotj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wsbhpufx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3sxuupwoj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3jskemqbu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3drlnvgso.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eldpeaac.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3aoynipdl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ntuzbrca.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3zxyugarm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vdonmvtm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3uwwmwpbg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3wjozflvq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ozywysgy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3yqpmzesz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qybludpw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3olitlqwu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3kwazejqb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sbrlpyil.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dldbgbpc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hlhmugja.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3vwalxbzf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ftocjkfs.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gybtltky.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dlovaupf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ssvanjpy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xsqszfjc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ylbxtzsv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3snyurrco.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mpsrwrwc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3dahxdsqh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lvmfcdrx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxbrkbja.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3cbfrelus.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ftgjhoqx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3aghtclza.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gvpsmyzm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3plffdwcb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ppkwkcui.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lalqjoxa.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hwgqlfcf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3qcyxalxt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3zhsiwbur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drtjnstq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3holneydy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zlbjvexy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3skdzaswm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3azendqdw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3biluxpqr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wykekrtj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jnpbitkb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3cbpgdtvx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3poedofvb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3dslftvae.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yusqzxvl.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3irplndlk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3eezlzerm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3krmcvghe.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rxsfhsgn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3utkquyvo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3wimkoavy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lwnrapkr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3rilgudcj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3xtdmvfvv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3wczfgliu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3kormwslg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3psagmdwv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eiljtpuc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3jjaisiem.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ughwxaxl.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3brsupxcj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zxomtkbz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3cpfnfqdb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3sqqqbmyy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3tlvkueta.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3snocpifz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3rdbpzgnk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3mltzljey.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3jbizhiis.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3apixopnp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3liewtfhq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ysfmovly.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mxduilqm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhklrsel.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3dtgjzneb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3eysjyuht.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3teoilhkk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ronoqmpn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3twxhelzi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3qzptxowq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3sxxawucm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3llzjlhlv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ccavuztr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ghtcmqwp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3cldqgwqz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3lzusmoso.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3jeqjeafc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3iwcnvhja.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3mmppvutn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3bxmxezlz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3kdmgqryg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3zvbjcfxr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ajynqdkz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jtvkqufj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3fcgcrmai.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3fijjdhef.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3chbipvnz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3juieajvh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3wtscegtf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3mzocqvun.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3kerlwxdo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3egzzulgg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bvnygule.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3kybopkww.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ueepkrvy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3nxrhdfdo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3myudhrwk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3cueydmmu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3lkdivqkf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ufycyqkx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3bnlirwve.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3zpypgssz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3nbxhooog.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3nvwcveqk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3vrozekza.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uiyegbgk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3lcnrkfvs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3qblpnulz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3bpzgfkia.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3emaegzqv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3euxkiigk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3eopxejsr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3rnclvwmn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3vpwsaier.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ltwjsuau.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3paqsynck.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3utgxxdmx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3okqsbhwr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wvzrnauo.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3fdkvrzve.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3hxmvbekp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3nzewhtro.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3uqfluvnb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ifurawtl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3cjeldxgj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3gzkfpjkh.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ddckmegu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3wyllaark.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hiqhpkkr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ccfytvoj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3lolkfgdi.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3lrjjthen.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3iaaorlvh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3eibcwwtd.html


<!-- 参考信息 -->