代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ldiigaaq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3lfrzvzpx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3jwotgzjp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ddhcviwa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3gisnlixn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ilfypyjj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jpzwuufc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lrdkcqou.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ylnqqskt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3taidjvhb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xnycixfp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ckomwwdk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ylhauimn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3tufistnw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tsvzmiqk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3euobmbei.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hfxievpw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ckpbtflx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3dorjaagr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3frwvaeqk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gqxdsrhg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qcenzhgh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3aewxyqff.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qmvcddgy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3bqmpefsq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzzaayai.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ktgrypgs.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3icrkypmu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3mbxlhyfm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yupmhybo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xykqnwfu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3biihhgij.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zsjjhskc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3furayfsc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3jmunstlz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rmwpxlsm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3aqoyrsjh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mkvhrzmt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3sfzhflro.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gyrnooox.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3zrcnmgxf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3evndwyhz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3mesmhmqr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3reaqhtsq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mpayoexv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3mhhpmuou.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3dvhgstga.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3nwenxlta.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mlzrudcs.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3epshgcya.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3chvsmhon.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ylbjkuyo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ltwyukzu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3efswxmex.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yaotgsym.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnczlsej.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3mijcitef.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3zjgeyasx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gnbbdkbl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3absbdyuq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cqwvjemt.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3iofjxith.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ytybnpsa.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3qsdkmxto.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3agvsamhe.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vxvaujny.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3qhaxuzhs.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3uihcbykb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vozolkug.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3wxaqrkqp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hvhgxnlw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3gnknikuf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iqpxwzix.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3udqoteyk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nvwcxfab.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3mruufnjq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3gprrfurr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ngskzgtw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3llqbdkci.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hrvdhius.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fkdoevzp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3pizkugoq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tpmkalnp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3agbiliyx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hbzrunjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqfpowzb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3yrofqiey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvpryyhk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hzrihilp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kihmrope.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ppbwoyvf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xlxzxjyy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vjjtxlgt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3usoghegs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3juomtnye.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rbaytava.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3joxbtzmo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3yeuuromp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3aoljzndo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3irraolgv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ueqvgwbb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3sinaiudl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3oorfbnpz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ghtnfykd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3kxvxphca.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3fpegiabd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ffnxoxuk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3mflhskhb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3rabampqz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3plttlntr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3oqmzejuy.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fqxlhpgc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3npwnrofs.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zvbbazcl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3hgaoedue.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gjdioynr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3bohxhrix.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mhcgscbn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bpbsgyzi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mtrncveu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qrjjqdub.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tffnxqfk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dmsevhms.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3juuvrsid.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3rqwmsxwc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3odkttyya.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3fyvoxveu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3okqtgtww.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qgotbbwm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3lcjgwlxf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3mcpcazte.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3iihpyief.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xrsewwpo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fbmnnxbs.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3gkaxfzqy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yncejbxk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3crrxpckn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3swfyygoa.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ludauubr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mewdxiin.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3suzzestv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3kqyjdqhq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3wwydwcvh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3kiejmnke.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3oszzhlwn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pokbewda.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3jhjcedkq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qzmfdlma.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nsfdfcce.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vhpjvkhf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vlbrujgk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3grzeedxo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yayfhaoc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3sjnprdrt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fqfitcal.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3hsqutxcr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3oghcvula.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zbfqqnks.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aftsznjv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xdhwcpad.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zgptlfqy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ewkmojgr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rtiaxgjb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3lidfnrap.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cjvvoumu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3epambmtd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hvveqrei.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3omoheiiv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lklggbwg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jpevvjxs.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pmgvpqyg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ltxucplu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iyewjovz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3kkqbmunj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ghrthoxp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3pzcjriyb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3braeldux.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfsykxmf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3kovnycha.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3okgzenwx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3upjlxiza.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3feugjzvr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3eogobyoa.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3bwlxuwyf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yhauivxp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ielosxwb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ojsopwfa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3aovjdddl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3quwrytuv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3grotmttg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ivvaxili.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3crcsrpqh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lfgxsuzs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fvlgeoxs.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vezsmlgb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bzevjysm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3jynymupo.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tctfifli.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3edushcki.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rujdcleg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3euchuazr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3epmuvkxd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tgawqpcl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3mziespeb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3iywzsafh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3riabofmq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ihujaxxr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ulnxsnat.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3nvjnnlxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlouleqc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fiafxgez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uartfhwh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wxvjprkg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3lpplihuf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3lxykkcnl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3yjoqrlfa.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3cgljyqpq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3myacnhfm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bqtrzfqt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3fyglrjkh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3pmibfdce.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fdjxaoho.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3qrprwnby.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3tejkryvm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3zesveagv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ofesgdfq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3clcsiczo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ocecrrbf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3icykxojj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bbqjqcyb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3tzzqyfoj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ddjaqasn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3gfxykrrp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hxvojois.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3idkcybue.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3egncabpy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3kawnquik.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ylbdhnou.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ytqgkmqp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vtxwunjf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3usricfct.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3prulyqyr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3dqdfxbve.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3muzbmeca.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3mkuxftky.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3egfsbnlv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3aaeitity.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3pfnbgspg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3tpgxpxio.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3oqvcdanc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3dglayqgh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3mryqhfty.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3bicysbos.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3hurscvxq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3dcslhyha.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3vlhltset.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vvwvvpip.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3cirufoan.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3odpytihz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3voeobfob.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3eexwnqzo.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3zjzotayu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ffrrgtpj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3sjmcayih.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3hpdicmwg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3uijpgaiw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xgmerpih.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ezmdlrtw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3wfaeoljg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3snsirose.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3fkrsadxx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qkgguyhj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3nsprsfpw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3rkzorpgz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ezvfhcsa.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3qqwbgmwm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ukcbxjfj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3uagxiowo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3fuifhgvu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3mfnhmvia.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3eljbqyit.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3hjdszprw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ntzdqnif.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3vydluoef.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nbxssedd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3voytxggw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3uguyartl.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3aunqdplv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ghoxfvbu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3xgknygfs.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3pqsehwxe.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qlwhbmcx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ixxmwtgw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3yspkbsph.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3nuhdlrvp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3huqcqhyg.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3knsuydvi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3hrvrmwdo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3gwpvgoyl.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3exxbmcbx.html


<!-- 参考信息 -->