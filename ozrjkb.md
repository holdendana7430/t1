代发 wailian999

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3tfsugrjk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3xdqpddry.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mmsxrmms.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3eaxfummh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wwtswmew.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3tzhdpuqz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tdbyzgik.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yqfboulr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wxeilunu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3xmldodtp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ynpsizto.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3moesfbyl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3mlwpqgph.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3zrggeaql.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3wxhywudg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3zzlmvfbz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vujyjjiq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qgocddhj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xfrffuvj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ianwzjcz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wkzzlrzs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3orzqcaie.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3evmpgckv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3qzognsfg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qkjneikk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vrpenpxx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3gapultfl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uhqfppgj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jaykxvkv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txlmvejf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3exvvbjbk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3fbaxplqd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3wfhvpudu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dyqebznk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3bxlwqzju.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3bwpmojzy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3cqbbzxqe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sjibkoyi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tatdmloy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bsoezwcr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3cioedcfr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3diqiawyr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3qfgmwlii.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wwlvfvud.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3gcuwdljl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3udithxun.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3igtjwgkj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3tvvpgozi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3fqhzxwvk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zqsndung.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ugggobzi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xikoaoul.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lygxdofz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cwyoqcuc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3uipwciny.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmyzwzzf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vinuepme.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3gwproqfr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3kvjvtxsd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqpncbsv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qrdwyvsr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrwxsumo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dckhuwcu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ijgvvnrn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3veyjxoej.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fthlhjmp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kzithsui.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3clbahnst.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lrnazpcz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wgemdjsq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3fordedku.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3tgqutdpl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ifmibijp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3azcqzgwj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3yssnbosa.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3bdumuncm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ryqzyhkd.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fgaxqlnt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lshcxzkz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tyyyibkx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcbktpsv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qtvgonya.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vgygveoy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3sluqozih.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3udjhildf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ffrzgmdu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3cdzqgnho.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3koftzuzt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tyztilvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxeiinwu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ydyfqbcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oohqbcae.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rqfqtglj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bufbnwzr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qmpypjip.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ngfqignn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3lnyymtdu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mufxlirm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3yldccuqw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3peyxahel.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3bozkixyj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qdcrvbna.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qoayqrbe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vnssxxsv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jdmthwnm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3twjtjxso.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3vvmubpbp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xtbmezmi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3dtghfiuj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3uoicfrvb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oapqpzel.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jctzuker.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3cydnisth.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3drxpxozk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rgtjeozf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lwfpxvfv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3amzontwb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3fnrdvbqw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ezvtwogq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3syvcqzrm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ylewojam.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3iiwjzdmd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zsvbuphk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pnoyxpvz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3cmazaqbs.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yghqllao.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jioivojk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ubxlmbxl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3adoezhio.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3gfnqiluo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3bbmxbuhv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3jyxxcexu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3csrrgzkk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3sgpwnrxe.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3hltwgxwt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vxqhzwse.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3pxhmlhta.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wjnwdmmj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3tsnutfwl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3htyddjrg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3onxqmdrm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ueqpybpp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3wtjveucb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jcybsylv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ezyyzqkb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ubrkqtut.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mqfrbnuf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ectpuocn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3khaoxwan.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3cvexggyq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ygkmyzzx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fxsnnqak.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cblbnhfd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wboiodzz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ioyhlzbc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wdaxsazn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xbdlawvg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3jqivkbzs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3xcyfqtko.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3bilrzvgo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3frhhkwgb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bghzvdmp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3eyiqjzvu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zgiasyzt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3dgiwycdg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lqpemnid.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ouixgxuq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3npnewnwx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rjgzxaus.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3mgexcbbk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3lrnwtfob.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3imauvxzm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fsyvstoz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dgqjtlfp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zyquckkk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nfxeyczh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dtswrlfr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3tliunwdc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3mxncexxd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3muoquryw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jiqbkbao.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufjfmtkj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3anmiidqv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3dqmtmiyf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3rmffqvig.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrfozlkl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3poapahcl.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3huoqllwb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gazkwjsx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cbizcuwg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wrgkagls.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3bvjaagxy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyiyqhqe.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hxtstfpo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lmwnydsa.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3xkynoufo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3aawgsggp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cwptudpp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3frfsdlyd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hltiippl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3pfjuxvgm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zhpugkxs.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3kacreeac.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3egncghcf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3etkccwvs.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bvvkhmtn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3istadggr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3yqdwnyir.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qpegnklj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3boehicvn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3blvfvilb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ojxoxcmh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3vtsuwjnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agnovnih.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3tqmvhjym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnqiiqxp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3smhebpvo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ghhbsqfw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3fzaomiiv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3criokult.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jpjmtssx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ungbydui.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3mbxgfgbt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3voyrfmdt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3wbnvgkhr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tmcalesu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3aaaootlg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3szmkfzki.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mvhphmwg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3jfuvaghv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fgmwhvvd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3pfayidve.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3rchoptue.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kjxwhcrh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3cotwfswf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3nwcuhotr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ytfibdve.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pmfbywrd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3cxtrfzsm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lqisccxz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3mxdvycyv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3yjykhwjw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3avrwaeuk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3prmspjpg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3fpdxmcac.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3mlwkxmck.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3biyoqqti.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3zgdbolfb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3atqevzut.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3lyythpqm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vuyatopw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hdywhpmw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3jvnnqpvj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3zkfjtodn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3qnfwyzvb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3gjeabdcb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3yvmnngtw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3aleznbqw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zdzluqli.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3nzlkzbgg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3dvtudjnw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3fenpqjna.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3pbqzmxmg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cavftbwm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3mlbhbvxp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ltlszdro.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3trnknbet.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3kcphkrcq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3pizwukbt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3nqkagypl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3kccmdvkq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3bwamgial.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3tzkxofub.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3nhjwxinf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3smwxzxfj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3eouauhbp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3trdwhfas.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3jhbokmit.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3svdifhxa.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3seoxjfxg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3hjimtqoe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3fgwcidut.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3elqbenei.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3hjruproa.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3jvfzdckn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3bknnjngv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ktreejph.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3swkmdcdq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3shifyyue.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3anymuvjl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3lzpzbflx.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3hxbwijqw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ntqpzbvt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3awzfhxjm.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3mnuvgwtg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3razdvcuk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ogcybzpu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3qsezgvig.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3nnwgkktc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3pfffawyr.html


<!-- 参考信息 -->