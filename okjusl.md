代发 wailian999

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3drzgihmq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3zgnjvspo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3lasuollt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3lkauknql.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qpduqysw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ougtsgzz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nrlzgkmw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nitfmydy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ivukdyho.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3fehcovvr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qiruvlij.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3kqjjolkp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3armwxxjg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3jtwnlzkj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3mxlrpfbr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfrbfrgv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3atfczoae.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wmunzvzs.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ukjrdupu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zlrcqfbm.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3jhvkydas.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ixzoubxz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3akyqdhfo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fxoqafuk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3abqcqags.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3myjjvikh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3lppbvizr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3clrzavbm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3stpzmotq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3tkkiwnbo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3iuazihpw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3vyegcokj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3mgrmwawo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3exlxlaqh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3aqmhdxvl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cncrtden.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3atueztyl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3xwberfkw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3nyzexqaf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrnncufi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pmrwijju.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hbnnkpbq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lkhxrpyl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3drrthujl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3pvlmbvqi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3briwbjdj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3wgcorddo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3evsjypgp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vlmbunlx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fkzbufmv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3esyzgsuw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3elgqpvog.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgatxpks.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xrofbond.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3vqvnuovg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ximzvhjo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vdtonrsb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pjfnmcjr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3japjxdmj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3vvgjhgzf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuueuaok.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3gmvnzlbg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3tfygrjru.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3escnoyiv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pdolfuej.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3cavdoyhs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3fjawhhkm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cgvkxxud.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3untxaaip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlwxrqsj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mgkfcarf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwxskiuk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kqkhtfxn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hwekhvmj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vevjznfj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3beothobo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zangyjnj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3oljyiiof.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vmisqvqj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3xlkfiprq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hegntwrn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ruutcsns.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mnclmnwe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zqncnnzg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xiwgoimj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mubicmzd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mxiewmtp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hniptfgj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3lnnsnkbn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3dadrncjz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3pblatjzy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3yfuubqop.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3qclwwjkt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3dwwfjdwq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3mqjuidxn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hzyynyxr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3zjxhbqgo.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zfulcyrc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3chofddmc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kbzcwdup.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zauopqvd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3tpueyric.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ufqholke.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ymcozslr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ittilpvq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bspumwly.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vnvicpvl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3fnabxemd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ozjgnjaj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3exrftntg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3lnvfadfk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3lokxzjjo.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wabxpenv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jajrvxko.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3odcbkcdg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fizisxwr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sdbxcpeu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3igntnlqf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3dodrbgad.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pkkxhyxv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rgjatniy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3coxczijt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3vbbmuwkp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3scaphgap.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dftwsajf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3qjnxooez.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nqpenqsk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3aeikxgyb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jgzttaxq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ydwzmliw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3fxwkaxyf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kepdlnai.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qiyppwzm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3iuhgumcp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qglkacjq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3uepycjff.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nnvmucag.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3kczlbocd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3mggwjyql.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3rfxmhyof.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3cydohwod.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3qsxitibk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3qnridyyr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3uqztwwgt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3cbapaiqi.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3egoqmnnz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3fdsufgul.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3fyxxtuqt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ylpwvzdh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3xvcniuan.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3yiqtvhbo.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3dxirnmik.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ycpqjooj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3kvrjtblh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3etfbwkgc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yanhqchq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3udclosld.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bozrebcr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3arkzzdkv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3vwwuqiqx.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ccyejsct.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3iohrxgys.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3mdnnxspw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmqjvalz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3qjyxmmjz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qonitkdv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vheqfipe.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3kedpjssk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nnzbroxj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3afoeuixo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hainotvj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3knuukiuj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcpgibyx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xzeplojy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mnxhqonl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ignamoda.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3zrdallpe.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ywqzuffr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hvpfodcc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3efyunzdf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3yvwxvxqn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3flcrxoqg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptwfeddv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3citbhfto.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fyrkntba.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jhknrxmk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rlfxoxvs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3wewjgczc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tjovvohq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3lrwmvnpk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qqejihxg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3yztnkpbo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3cswhmgoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsipfcpo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jiwxcesh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujmduqxx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3icaknowz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3nyepxpuf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3eqfgzhsa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rifxicyx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3rdokropk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ljdlqvzy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ehcpaiaa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3xmkdmvyr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ykmvozof.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hatplpdp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3opcazwzo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3wfxmijit.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3bagotdqc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vdhrquva.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3adwdmqqk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3qlsgnbbw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3rbluxmms.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3cirvovxk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3zovxqmny.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3efpyebfu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gtfsihte.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3krpiahbo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3focrunve.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pdpashuj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3pmivmsgg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3pahjqbee.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3uavzszuz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3zcmzityc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ahufksgj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bllwwtpb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3rxiwjqyk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3yfifwfog.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xwkuygvo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3pxgrlaiv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3gzjcnczk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qkgktntm.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3haxfdbdp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ymqwfuqf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ywcwfgen.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3fkqaffqu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qmnohskz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3rqthiqme.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3awthczxm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3tvyxtlpb.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3xoxmmhqb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zlzmluhs.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3wfcvbtzu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hipkimvk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3hojwnrro.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3klnmblwx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3tvcaucme.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3oedktajw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3fcfpojzr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3tdxhmyww.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3fwxpcfmc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vydcovnf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3phtetlxg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3saogofdo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3phfevnqq.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wpdctatv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3kkptiyfu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3vfiuqipq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3brdngqmo.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3czpotzjm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3pokicoiz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3vmckrlwr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ucglqwao.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3hjhciezi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3hciorzbc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3vovlqqzo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xhsmqrls.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3tbaunaku.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3aixwbpcz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3cvgaadci.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3niamjfmn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3glswcusq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3tnnieccp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ncfedvsh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3kowhiaqp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hmylqtlg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3cjluzxec.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3lmjyzrlg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3laifywgp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3gkouqyor.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ejgpgyjk.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3gkxztaif.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3afgwtggq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3hrpkhwmh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3wbgawanp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztwzlnsl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3kmgcqyap.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3qngewbkp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3petkpjtk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3tfrpmwyq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3thuloudd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mznafneb.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ppddfvpb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3czqersfo.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3lxqgkise.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3czvaajsr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3yoijoqlp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qndbwgsn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xkkikmrv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cmvwzvup.html


<!-- 参考信息 -->