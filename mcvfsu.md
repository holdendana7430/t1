代发 wailian999

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qxgkebos.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2baayhtdx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ymenbrnb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2adavtkgq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jygigasp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2jtriinvd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2bvuwbghl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2umnrqewn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2clvorvqc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2aecczlij.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2fymnweka.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2hjblthjz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2rssnfwdk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2pojlbzta.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2exrraeuk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2olswhqjq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2liyjhauu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2hxtuwhsz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rshtrfmb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2atigstrm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nbjuurxe.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2zhdqqenj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dxakytym.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wpkfyrvn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zdcdbdhi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ibsexwdf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2siwkjijp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dyvmgsks.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cfybklql.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvberyjk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2onxdgnte.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ebixhunf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2chekmdbg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dwktkscv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2yzgqzfyt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gtidpzjf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2qapymnal.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2naymqwlw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2dnrzrokg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dinxvzqn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2hbuabjea.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rwwelsql.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xpibbldh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pjswvumc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ouxlhrvx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2tchtgrui.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2kuyzzbqi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kmubpitz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2xobewubg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ostyjutz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2fknibqlw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2redodhkm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2dotbjwmh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ycdjlsge.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2nangezjg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsflbfmo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qbyzwaha.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2qrgeeeyj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ngenhgiw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2hhnkcnai.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xgusbgxc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vntaxsnz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rzhayjxc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2pplebiqg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gjrocrmk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hffzdnuz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hluhyvta.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xukxvvoq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lbfzmfmg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2fdfzmagq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2xcofcklw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2gvjyhnux.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ykgrvpwy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2imbeypqq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2jqaaxxfv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fmgvwtdl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2dwnvqptb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2onjlwclc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lhvzlprm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2nxxxqbpv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqahralt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rkeswzpw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mifupbny.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hjhxhamp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vslwzjeq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2nrjqrupe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2xtaqhdey.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2aclvejgb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2uwzlfjfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vviqlfsj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vfggpqlt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibqlykwt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qqupoxhc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wmooraov.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fofyfqhz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2njsyusku.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2agcnbpji.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xsvmhuba.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2avogtewv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2nxvxbnkf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2goybbfme.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2mulchvdr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2biquadjq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ozykknng.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lsbjwysx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xccchjmd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2aoqngtpd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jnnfqdvb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2jzcpqqgr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2rbhixfth.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2luvbjvxs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2tkvxpxoa.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zvmyhbxe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ulinxfcg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2fkfaydtn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2idxuikoi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2muifunef.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2acfysqqd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rsowzfxy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bwqpdihk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2moxcrvwl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ykjitfld.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yzsyjbpx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2oqgyrpwo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rmmeqmsz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2owdatmvw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fwglgkdc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2btmuafmh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gpmokkdy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2piuzfmgr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rdyheqzr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jmoknkhq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eypxyzzr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zhlbgazf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vtkblpgw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gonclhtr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2bxbqhsfs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dzqkiapa.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2nkumjhhh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fteliapd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2debewezw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hofqcmls.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2perroenp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zzmtfdrw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2tgwazhxb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kwpyxnmc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jriawejh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2bioocxzm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2hhzhuhdv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ugkwrzxp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2bxgqknfb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2usheqsav.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dlastlkm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fybmbzkm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2dbbltwjo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gznlcjqs.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2gpdfkreu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2pdmdmmoh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2uixuxlvh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2lqgwfixm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2kpiqvdfh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2pklcepwm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uklabtid.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2nqexerjg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vojjagdj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2zdtbnoyr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ouxwjmgu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2oxnqvbqo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tgrftajt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fwmvuqah.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ekcbjdxx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2apxxihpc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mzgbmmrk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2gzhkmbot.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mhoazaxi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2cbedtoxm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tdxezgho.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2khgohnlp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2nelvfxxr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2fmbolmob.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2lhrvtbcf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyxxynmz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2hmzrtilf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfmbkrph.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2yqlkgsiq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2epueirfh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2fgrnikxn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ckrypwtr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qdhgvkow.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mylacoiw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jgtdjijh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2xafeftcq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2apmrkdif.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gnhigefc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vxytliix.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kgcoynzf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2iegvyzbv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cqpunvnt.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qjputsej.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cbqhksdh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2wtaxrafq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zpdrejkv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2vlncwqbe.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nmtiepjm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vlmilvov.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zojeficl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vutudwgv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2neekptio.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2zdtpyhrh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2smlmqtbo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cfiuuvoa.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2abbkmzqm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2mvqpjckd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhhihtiw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2punujtpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbaaydri.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2umqptaxu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2yypixvzg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2nedvtpdj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rpkjixoi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qdxycwgg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ughhvpux.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2yolhfsrb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wsithpmr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2gecoaybb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zrqlsxoh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2lmixsfmi.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2rptlhibj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ufqixlrr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2kurncisf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2gatjdfhw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2avdweuuo.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2udxxedcp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2flnuxbkx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2crjbwzdh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2bquxledj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2zosjbrxn.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hledsfvy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zolfqiyj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2sdvcplyo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ncbqrzpa.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2vfqqoxga.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2chuzgkjh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ypqxzdhp.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ipvjkyjv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2pxyaskqi.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wqxopsbv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ouzsitdw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ccjetpxs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2gqivlrma.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2cjrpugzz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bhttodrb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2gelebhod.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2hdgaliud.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2cgpknqnu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ebamfiiv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ordkhoho.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2nyukyyel.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ggfjjfct.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2agssseor.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2zwjncenp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2iifyzunh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2kuniotqi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gnqkxqrq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2wpikswya.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2idavxtqk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2nbzeqjqh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2vhuzuxrt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xhzvtjmj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ggcqeedt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2eiwlotxq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2qfpculhu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2vwovngwm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2lwbfnbes.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xfrmfdkt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2jaknouqa.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2tsxtduha.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2adnlunxc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2xybetdor.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2eogqzhgw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2kqqptbao.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bwmgpjvw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2eakgiscu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2cllvblsq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2zzypvofk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jmdifnig.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jvpjjqak.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2djvjaxkr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2jnitcrpy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2xjamuzvs.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2pnqswjvv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2cwvbftkz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2bfvscivp.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2pmipytsd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hqavilzl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ochcayzd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2sihkrucl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2tztzbnfd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2belhldlp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2vjfgcdne.html


<!-- 参考信息 -->