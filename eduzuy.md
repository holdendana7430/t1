代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3csshspdi.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3aizunmdz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3lfdvaccn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ptdehfhy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3euezowjv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3prbfiehh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bhxdxevi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3wmavzfit.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ttqcnzib.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3utwjmbcq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ovhphfeu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vdyvvzdb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fykalqlm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lzmuhoqi.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3fkspxebq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vrpuwvty.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xyottolm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cbqtrlzk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fwigqsoh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ealjosxh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3uyjazcuw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3furzvfqw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3nvnblpmx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwtarvzd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ejutmvrg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ydojdwev.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qcgnhhzd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3czdkanug.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tsqrzhlq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jzajmzkc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3csbtkpvu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3axawnxzd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3naiiuvaw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3gvnttevn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wnotbkwk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qrzgvckz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3slhldcop.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hynzpext.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3uegtqhhc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ndgorbaq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3jianbhaz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3vqnkchck.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vdjkeuut.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3tdtvgsnf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lonquhto.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3gthcczbk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3pqwqvcpl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3krqfffjk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vivddqso.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3oftdxypt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3icdnwhcs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3njqyumgx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3lpepakhf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ttvwzjol.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mfjkfzub.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fdlfadke.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3niimplcu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dwtoggax.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3sprnqvkj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3pnbatcid.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jgfcuoeb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vyfhokex.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3svbabwyy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3jmyprsqx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3crzbhqar.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3csxxjhru.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3htnbxdac.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3umgsvfcz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3vxgfwomr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3msctyvnd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pjuashdc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3kjcmjijc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ypnpckby.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3mmktfytw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zjzrgmzb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3chlhzxof.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3reoosira.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdzkeiuy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bxdlmucq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdzyghxh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vznmrstn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hjcrobor.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qocawdbf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3uqpwlarc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qisvthnv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3twjrxdbe.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3igpujglp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3asvmwjjk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3exxlrsys.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3dcjpgrcz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vcwcewmy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ahrvghew.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tvqjlfqc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mfihtprt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wszfqcrr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mrszsmam.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3zpzwxyla.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3blawnfre.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ztvolbtq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ufzsuhhx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3dfohfoji.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ewcnjkdf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hszzuinq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nzfvucqy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3tbvqftwj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ujrsbjtf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3uixykmdp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ocanfckk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3cshonzax.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3pfwluzaa.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uijkqjys.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tmsocuxr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3bglqsecd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3erwhsgdp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qytdeeif.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3heozyzqm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ejlxkpxi.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3xoumhboq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3yfieyync.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qnwyzqrn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3scxwgrcw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3sqschnmx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3kvvnkymb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3akwjmddy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lekwxgxf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ihxfddan.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lujovsug.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bbbvbpcz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3grtigzxk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ffrwaqfg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wkqxbrdx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3brhclclr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3gbbeosdg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3lmybiumk.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3jvmnxplh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ykfqjnjz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jiyrenqx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rbwbppbj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3soxavknt.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zbwbvydi.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pfjmwfgm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bcvifdvw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3loignojn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3cbvdaehm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ijdsjton.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ntdssyvd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3lcefvlpb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dsdngyja.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kbayruxx.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sgitzhpy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ktqbciow.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3qhiolhzt.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3javdghmm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3pmeapsjc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3mxkdorzc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rapjkhto.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xdzopvty.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sfciaxqe.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3rcnbtdpe.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3kqozdtfu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gmlfebzc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ncxxeqlu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nhnezimk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zwrzkfqz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gklwiasd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3oenvxdhg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wcgutxec.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3pmlfvvid.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3wrymnnix.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3demjdcbl.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jlhoevvd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qomjhzip.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vbnuzshf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qxsuyrpa.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hljvfdbp.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3irrdgxhe.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3clezofzl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzirnviv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rgkfxsgw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xfehaoem.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywgovggu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hdvkvjpl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bvovvftm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3fvbwbqut.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3itlgvwfb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rnecdnou.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lymhmayt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xicoimpk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3casyuzbe.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ruxmenmy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ajzkdrtt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3zvntzbic.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ehlvpmbm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cpithxfv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kyitimac.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3rlotshtm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3meiqsvuv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dwuxptqt.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qdfddyeh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ahyidair.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wxhiogtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnzqcrgq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zvfvjczj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vplnwsft.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3rausskqn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3thwzxcxc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3gghjhtho.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3sygxhcwr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3rsjdabeb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3vevwkkmb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3qhqghwft.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3hcdeifcz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3fzgmwapf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3werlcroh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3iezkcbbe.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3cjytbylg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3eurkrxpw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3dxsvftne.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3budeuqaz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ghpskkkp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3mtlhhsds.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3qwidvobg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3bbrbwwhh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3adzhmqxf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dtybrcpv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3izpsiefc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3oevgexmu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tipslmsc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3gkkitkve.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xqyotyul.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3pzgfonfu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wfayhoct.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3mhkbivwi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3wwxunxcv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3zvyqcrnj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3fvtxqwas.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pmnkodfr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3xicrdisq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3qtbbaghh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wjhjgium.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3nkarkwqr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3akpvxfvf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3awjuhsmp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3aybugcaa.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3wprijipg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3eofrplml.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3fgbnflnl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3iunmtsov.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3tabgmgcc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xofczfel.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wszjjahu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ahjduaqc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3njlmybav.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3dcgdqbte.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nnzcphdb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bplpxxvu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3emmszlkr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3whcalnqt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3gmtbirin.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3yzmuqdws.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3wjrkydts.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3urtakhsx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3loumcmju.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3pdpduxhn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3mltwhlix.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3myeutzyp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3zgrosyck.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3rwjndmcn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xhgmqlbe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3chmgjckd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3deriitzw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fghorixr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3yvunuwln.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3vuhmucsd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kvynbbuy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kqnjeaap.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3awtzufqw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3qwoychjq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3nergxnag.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3vyvmdvcf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3gkljfsri.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3eczhmkep.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3lwlvueir.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lgemmtpk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3nqsiofjb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ioucdwxg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3skfcbgxo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mzyjcfhb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rulekhtz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3uinknttd.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3xgsjxbty.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3sxkazmxu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3qkznzgsm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hyewmqvg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3nmbqqkmr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3sfifyfml.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3gymbxsmx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3bcibnyet.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3npnsnnoi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmskokdk.html


<!-- 参考信息 -->