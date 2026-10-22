代发 wailian999

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2tvqupueg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2cakkfyqf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rjxrtwzq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2woyrhkro.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2abtvtpot.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2keepkrfd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zhimrbui.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qgwgsakz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xzgpectk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2newzorrx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2itgtysjx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wteohrkx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2upmgjvnj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rqhcuxim.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fdkmltmw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2vtnkavsr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2eucjqyol.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2lgrunjxl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2appcmjgt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tegeeqts.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2rpxeptxl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2gpilpdmx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2jiafreac.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2fprrocnb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2kzpqsgrq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vzqujdzb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2mlxbkthh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tyelxqep.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2wibjyokf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2coiurwhv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jdoqdtrw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ndroqonb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rzzokkcd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bldjjxts.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2epmdqpcg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2pmqeuusi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2nmouvegn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2izxjubwi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2gfmabfxg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ysogxsig.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2vgwbaarp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fezzghed.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zrauzhhz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2imzfmdqo.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2lilppyxg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xfkuuhfv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ncxzasjz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2hsqsypkh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2fuaqglbg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2dkdglyqw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dnepggsm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2gvqtlnth.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2sqljuuxr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rrxjadsn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rascxliv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2khjgsdnr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dliulquz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2egvamzsy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2mpotyqfj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyqklrkn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2msjpovbh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2yxosyvzx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ibwlgpio.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2qqyeneum.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tpfoaiib.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmztuunb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2oxdrdhhm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2frrxacno.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vegbgbzb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2sbxlkueq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2wnhuuuiv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qgonjbbi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkvdyvaa.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2tifdxwsy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qkvhdnsu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vdkwuryh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2illllmho.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ogtfmpmf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xyubrmhq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2lsyukere.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkyndyii.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2rzdwpjqa.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pxqmiqun.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2rteuwbdb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jfoywwlq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2cvwrokvh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2adyxqbxc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2jxnttcol.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qooeueqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktsysqqo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gcxoyqqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtrdhxja.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jerbpmvn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iaxpghfa.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2eiqcyhhd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2mtildslx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2sjazpxdz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gmcdtrcz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ratnprbp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kjqmpgmb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ilxhbpgj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2mmpwtkku.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zshjbvom.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pbmhwwzm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pqxlppek.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2pyrffgye.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gxtthqfr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kunujcgf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lqfalqxq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ndhpnlhv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2cajcbtaw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zijvjsuv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2adfzeaes.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2dhnypvdv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pmsxfoll.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ffakyenv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ajtaaptt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jaktxtkh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fvoptlxd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2svcvzrvw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2wniauewo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2agolkdpq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mouxlnmx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gjcozkno.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2yinzlztv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2mcrsvmgc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vhtrytcf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rsoqtqyo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2etwbaahy.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2crmwlsbi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2yaebeqqi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2euvtgfsu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ybvfmxoh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2gukqdqkb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2imdgabky.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jjwplzgk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zugevwzs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2pvtkyszz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2bahbxmzm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hpsybjko.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ngewboba.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hqkvfrcb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2hwqzviih.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wwgbfolh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2jlopxsdj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2rgcslcyz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2brhsvdgr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2fnyyrorl.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ocaywdon.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wtflnhbd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2fchigwig.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2xcelctug.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dtezhjsd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xngzllkg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ychsgecd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kuwkbraz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mkdhyvmo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xwcieodv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gyvvklen.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ssxhbdvu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ejzlabjo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2zhequzzx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2mukxxdjt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2opssiqtl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nnbfqoyn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ubrjfbdn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zxpeipam.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2wmoflmtq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2byhpqvsi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2xuwergfb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gbbnvabr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2pmuxqysd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cgdptlam.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xplqexry.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qaensxqc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rtouxfby.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jtprxkjt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2snetarec.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jjckdyor.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uodhbrdh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2znkhqhkw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbrkwgat.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2zrzmqmzk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2cuofoaxk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2kxfhahvf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fxbaxdpb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2peyphccm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2panygztb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dchpqykp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uxkuimho.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lmmizvfe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2nohajkvx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2nauuavqj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aangegux.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uvarednq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2qtbcafzm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2hrdsenpl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qbqpbego.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jszwlpgg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2alyecdhp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tsunsavb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zvzysjlv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ynoariow.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2vjgjquke.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qcpbrmzf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2djzjoway.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gilagitw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2djwejvmm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tvurcoyv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2kljgbttn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zsakdsnm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2pmbvzfpw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2oavbwzdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwuyxeag.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uwhakipu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nctaaopg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2flllzjas.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2oedfrmbc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fbwapzse.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2vtbjitic.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qxxvzmsk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2jojasmzx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mtsdbviy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2tllfcdoq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qykzqjsa.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yfnivcem.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gdcgvtpm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2axnqpzug.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2obkrozyu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2caltmoer.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lkctbruk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2cwsmhwlu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zxzqhxab.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ugutkxcz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2xlpbakay.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2usjiyzjl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2vyukjuas.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dhhfchcr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2gvrijecm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lgwrcixo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2acgzxqfh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2fvinuctl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ylifykec.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2mbtzvnbf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2plsbpwgj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ockrsnpb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ckxgzkxv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2bqfzkkdc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2kpzstiar.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2wvcyqxmd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2cxtkamlc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cqpibhtt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2jfpvgzsp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2klwsohyl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2hgazibtk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lmbkdqjp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2pxngldth.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2dhfilgbj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2auwbubam.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2cqoxdeym.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2xnbntmpf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2cupatuwb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2vtnuskqy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mqlzabjt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2lweanfcf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2aijqvkvg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2kngleyvx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ydxlxciz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2tjvwlkms.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2mevmzxek.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2bowhyugv.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2nbujtwvg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2madmmgik.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2uqhtaqiv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yqxttinf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2srpgckrp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2oezemufp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ebapqiut.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2hmapzpwz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2nbhpdbgo.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xrmrqlyc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2pfzrldnw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2bitspzcw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ytbxkrnm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2iuhojuks.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2jfcklaie.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ophquixh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2eqiihqon.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2msriqlji.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2wufjwifn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2eiwfslhn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2wtaekgrk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2bsqycnvt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2mgewband.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2qmtedlwh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tshdgvnp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2hgsxzpqj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ydlvktgr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2auixsguy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ltcajoxf.html


<!-- 参考信息 -->