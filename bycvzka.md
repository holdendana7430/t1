代发 wailian999

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gjaiiohmd.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gybjeuuma.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumptjxoy.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gezmaeftk.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzqipkpe.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpmskasty.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdjwymzz.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gveekrlgq.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gbdyikcbb.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gbvmiljyz.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/guixvfvbh.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorkmtfad.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gourolzan.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqshgcvhz.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfychssos.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/glllwuhjm.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrhopmhz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gffhuzzmp.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gqybzcczc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxeklfyp.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gpxjvndzx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grpuuqsrg.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/giarhigyi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghukgqnpn.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gdqdbteyp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyubpmfk.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/grkmseury.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmuvlrfq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geunidqdx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvluwwgd.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gvsphbcwm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjlvgwzc.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjusbeqj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gkhrcpehi.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkpteweca.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmunauwpi.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/guoudojcy.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gvaxoghht.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gofkuvglc.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goajxtvph.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gkigdnrmi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsrhmjie.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gujltugrr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghycwffql.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcookjpdp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzbarxtcb.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwzwulejc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gowvyguxd.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gejccqiit.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glhvwvegw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghesojznz.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gfovhuyxg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gccgjyiuq.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gliseidja.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxehnbrvz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/glowawtzc.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goljuwfzh.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gupqrbnng.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpztruznl.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdgasqce.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gojybcgof.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoihdidt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakpjbeeg.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gpswdgjkr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzcjyinj.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghioryynx.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbbjelte.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbhslttj.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gyhagxzvs.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gkjlqnwvi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gktknlopx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksjfyjnk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwgkrykq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gujxygqni.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqrzqdwn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcawsyfh.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gznpuknns.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqduxiozo.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvlknjuq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmisdhvk.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gmqitlnzp.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzybemems.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gaunbdhju.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnifwhxi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtejgtbpj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giknfetid.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcfeoiex.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gxtzxyrtz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghayuszat.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpervyyp.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gchwwypmq.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gixezdmiz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfsexxfi.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gphxmyzae.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gztvmjpnq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gpflvrtdl.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gqjlvfqli.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gzwhjizff.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwplfulk.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gosyqhvkx.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gmwzpqdat.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gsbocluvu.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gpcdklknp.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gblywgeri.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerciwznk.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggueppxyk.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/geagjnmmp.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjupeegg.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxqslpfs.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpggplqrj.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gwuhkzqef.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvquhuglg.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzsnafgc.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfaqvxmj.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gmudkgsqt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/guihadhqz.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/grxlcqyfz.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gxyjnjwsd.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjhvuwbk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gchefymqs.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnvxzzau.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/glebcxpkb.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gqlcpvrzk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gdrankhpc.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyoncjxp.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjfepxhf.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/glflptfoc.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gbjpisjkm.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlbfwakd.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gvdcbouxz.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpbkgwoe.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gkyfjdugp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/grohxotmv.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gzhcysaig.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gurfgkoml.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkdbaoym.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/genuaiavc.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ghbkxnefa.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gffhylmql.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgyfwpdl.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gmiimogbd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gtujpkzbw.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gplokayqi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gpvrdrdrt.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gbmulhips.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/grherefob.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gavqfxcny.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gnjlohalw.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gnmlstkam.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gzhfslztc.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/geybklygr.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gzmbysgav.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeiwkqjn.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/ggiebsyqb.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gzqoghiat.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gteryeojv.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gxtibmiaf.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggketsdgp.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrfbdwhi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjvklvdu.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbnqmvik.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gmzuejsqd.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuutubcw.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghvhkhjgk.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzmbgofk.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goqvdzfbe.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/glsbltjse.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtmwvxhsw.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatzmwdlv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/guwkburfv.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwzvrhjd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gymaxdvmn.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdhnqhlr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gprafkxad.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gahdofkro.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/grlukuoju.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfvxehuq.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/guqexndza.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmedhmkki.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggjdtflv.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gqudqdsug.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gxyoukosr.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvplzhcyk.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbeodzty.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gclhqpldr.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gxumzupfp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqytcwmky.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gnnhuozzr.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gqdqfriev.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gopbadlxd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpblndarf.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnkgapfu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gxetgnowp.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gkwtsorkc.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gktfwrruo.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbjrmgsg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglionaxu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmteqfvye.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gwdnjewbn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grtxsfdgm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfvwipfh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gxppoeyxk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhzcachh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganoagsoc.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gqnqyrjfw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlohhage.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaktqdos.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gmefdkemy.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gqxpsxyhh.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gixwmsoai.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdlqteev.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatpkrzmj.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gorvmzouw.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekstcudr.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gxoekfvpt.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gycfebcon.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/ghhijszqw.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gggubjjld.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gutkeajis.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gkexsjdaf.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gikvvvzxi.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gtwhhwdqr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gbhpbscyf.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkmugxiy.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gvvotqyut.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gnhaqaced.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfllmaon.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gmedjqhgb.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gmnmgurme.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/goeknzysz.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/giiqmfsgf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gyhbgrbhj.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gguaymjyp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzscjoiol.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkthpecyj.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/guajzwcej.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gbtuvrpuu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/goyexojsg.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbqttfnk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gimerjwen.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbjawkat.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gdvdvpjhq.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsfnrigu.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/glxvjugsd.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmwhdsunt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gxawqqpog.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdtbthse.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gaayjwaht.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gocwevgro.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/geukqbhmy.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gzmmcamhm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/giwtofpzk.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gvjalopdr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gexlejxiu.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gibvvmmiv.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmpyvhje.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhfvovtm.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gkxeczmns.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtelpkqg.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoqtixnk.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/ghzivnqes.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/guviozwdg.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqabqkrk.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwmriiqb.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gwgzyhkto.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gopyeygbw.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gcpzeyhyw.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gcibdflkb.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/grtzltyub.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gretgzgxi.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gluymcgyx.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gvfuvzqjr.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvzjsuus.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqrkoyiq.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmocdtwo.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/ghlobkojj.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gyvjmjmwh.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfxiauxd.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzlakmqv.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/giezwzoro.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gcougphtm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxovnpcd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/glgywnhoj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/giqgejwvb.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gjedydjqr.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbyopurf.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gulhhgwvz.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/grnoxftey.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gegwpevlh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glblhjswe.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfdkfgff.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfydeltf.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gxafpqvwy.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/geqejjjxk.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqalwdit.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpnfvftw.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gnypbnidh.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/glysuhcev.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gqponmdtp.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gewabmxgn.sHtML


<!-- 参考信息 -->