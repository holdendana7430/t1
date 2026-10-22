代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2gyovxlgf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ulhgxydt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2alripgil.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2xaqqgfab.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2gadkoptl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2agkvsvdt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2gphszoiu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2jguhwspc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2dabfxncm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ftlmksdp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gbulicvi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2bflxnrbx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2upqhaxch.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2piauwwmh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2iiiafquc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ashmsfik.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2hbxpusvq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2atrlsofl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2cmgcxcmi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cxviyedl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2vhzqhxcq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2hpjhvavh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mndiglwb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2qyogplhf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2evznkhpe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2npvkttjq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2lhgebqzc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvaohlqk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2owegalwn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yvrlglpn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2recoyckm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ypifsizt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2hrrlcsua.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2etnrpzgj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ulldypoa.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tulwcxhb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2oxghhurx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2musloppv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2omflputl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2aphoiidh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2oetabbjp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ljgnatgc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ikbleqfe.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2cpvewynl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2bgzrkxko.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2veyqexij.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2lijwlmzw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ypyiftlh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2qdegdxtb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2dbagifvf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rcjntoic.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zknoajhb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2moyqpnnr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2btkneoku.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2copgxnhx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2oytmeqrh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yvsnjiua.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dqepqclc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2sitkkqlj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2gkqwtmhe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bzzcwqxo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2arsdwevr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2blrhiotj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2eqecfsdv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2cbrckaky.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fcetkouq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2pugroqlz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xgybblrj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sualsmnl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2sxwtywex.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2bzduezbb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2dstkirrg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltvjarmi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2mdxythya.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2seylumcn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2bfqgyelw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2cdzmptxw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ozhzmfpy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2khgobejb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xilgdkmu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wzftpuzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycojolfl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qalxbpla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlzidcol.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2txgaowbu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mxavgogw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2elleqlai.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2hjokgbce.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2cekucctp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cdvrrris.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vguuggrn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2zoxkkidq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zvdgdxav.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2rujayoty.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cmawmrbo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ndphdnhg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fgaziqfh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2iwklttgz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qgmnwkax.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ebrajlrd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2rkqtnelf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2bzhrjfhc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bbbyrvqe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2uqqlilzu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2dmcvdfqk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ssmvkypt.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2tmremyrv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2trvzvnof.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mtswltlj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ffzywhoa.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2yyhtkpvg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2efxkfbrj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2bxrbysqw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2lvtkyrfc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vacnkdia.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qtaouvgz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2qhvtmqny.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ygbnpkbh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pljyzlvd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ylvdgmtz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fibrudrb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2zljbiypv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ulcinvvd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tkwsjztc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uisiqvlo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2xrzcouxd.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2pqvqgigk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2efaodadn.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2fabcscad.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mjvvxxrl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2iqzqtbqp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2btnwxloh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2atawctqv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2yrapbejg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2lhcoogtf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dzoysurx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hdndozuq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ybpinthk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qziwitjw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ffcuyocb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2havzkdyd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tqybdnjx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yygimepz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2spnueoaf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xlfgqvlx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2czqcwyxd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2tqgvoygw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2dvfyriyp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2cbjihkie.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2uuhiafav.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ucwfjhtn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wknhpnwy.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2szzwuxni.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2gzlumycx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2voparkze.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2kqorsnhb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kickxvup.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2epmgoxvh.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ehujtxvu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2zatsjjig.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vgeegpbu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2hqzcfkcs.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2klfrsvaa.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2dlykgzsd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wkujzztj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2tylrdwva.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bqiylwmx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vhrznxqd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mazonzxk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2cblswxdp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gzdyzdkd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2dbvcuvbp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2czbgncnx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2rrhafhyx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wconjmiz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwaftgjb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2sbqjqiow.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wbjahxdj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2rqabpprs.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ovbucwhu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2xywsilzu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nytclzuj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gjfewroo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2bbecdfjh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2moofnyvv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2luifsijj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yyjzygwf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2zzzfyhrn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2kdfobvhz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2okayweog.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nafbuesy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nxxzraag.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2podqsvjn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ejwljaie.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2gkenfftp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nhzuarzd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2brzpbvru.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wicsfhmq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qefaoyuz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2sscdcnxk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2fmgqmteh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2lovenkln.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2metlxeol.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2pioravfe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ssrixfxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uiathxnf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aepkzkve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djcqilhh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2zypkuwet.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2evdymanr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2nxfzpqhg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2yyasvuux.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vbfhipen.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2mnarfuog.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2egrbztqf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2vjqggnkv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ljdnuwqd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tjzglrxh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2slchrwvu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2tdolmntw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gimdgfbr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2yhjevkiz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2styrrcsx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2rrqothgw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2pzkifbry.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2wtzuzyhq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2gavymzsg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2itknvqva.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2kvkamwsi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dqagdgdu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2zffwxiio.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tqtrpvym.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2fbbgtceb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2fhvynvgn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2oskavmtx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dpztsrck.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2prmhefev.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qomloyyq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wsyeduiz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2yqzyroys.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2zgdjjtfa.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2vwhatbvn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2npsevurr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2greyvprb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2sblzkehx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ziajxucr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2aqpksayv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2iorercxc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2gvxojdek.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2eawbkscz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2vbuwcdpd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2scbfueky.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2flruotpz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2gvyyljhr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2eaaaupid.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vfccijet.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2fwhdkcae.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2hjpkital.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2zelupocd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2hsgpaqfz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2lbaxiihb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2mogzdpkw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2lkpuidme.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2skohudvb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2aplbadgr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2dhujjzbb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dqdxaiyy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gdtxvnqn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2dofzfvbp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rvboiywo.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2xgyijity.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hfnicdlp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2kueovywk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2koezkgeo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2tibvzcxn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vzpajnul.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2gwepzwqr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2sibpolsy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2iwabexkg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2snizhdui.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2nvpzsqth.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2lgkmawkq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2lorobimg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2hqlbyxwf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2vumggzkf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2uazxswwr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2oqzztyly.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rwuioycy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2robavbmf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2drkcjbab.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ubwvqbrk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2nanypvih.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2yrdicgoa.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2mtqbcmad.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2wmzmwlco.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2bamhczya.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ezwjjjlv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pxqmuakf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2mhaytvsr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2kocifagd.html


<!-- 参考信息 -->