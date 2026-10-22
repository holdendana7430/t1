代发 wailian999

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2unbpjlay.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dhrmsggq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ysjdyjfi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zcoosfwb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2erhartjp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tizzmtny.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2iytleaix.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pewgljtp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2neguamhg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfveggwg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sgapoyht.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jwpgilgi.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2tlaicwsb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2leyumbzs.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xelroktp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zviyevem.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2iewdeavo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ctnupbmj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wgkasbuc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cerdfxau.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ydvkycnn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2jjrzekcp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2yvorxszy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jfrnnrko.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2udjoqsgz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2tocksujj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2litlnsmi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2sskjhygm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gubaklil.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hpbhmkld.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2kuapdlio.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2chjivvgo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2iwvajwmx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2esiyepzf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ufhusezi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mghsfnyw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bihlxnqv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ibycpsuo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2lnexgcvg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vatdknoq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dbprqjob.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2gncmuafx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iaissuvv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2skkclokg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2cvwmyvtd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2rtsjtsde.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vgpkmnvz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2byrwyijb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pxqjovji.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2yjylwwrp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ljbdguws.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zybsltpr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2hgcystrv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ahhvvspo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2kaszigrg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2bwtrntss.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hyjzmgbh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2leklrpyi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2pzmsmjji.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2pjjpcbvx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2jeoitbcx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2njresrug.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2serbvngl.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2szrggqhr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ujeiwuve.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2nsmilfpk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2poeamrxh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uugxbjqq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bvtzoaod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wncglgbw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qgjyyfvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acahxybo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yvcghmbd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kskdiyqh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2epvaskmb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pinpshrq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2owyrfsrv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xuiacdhh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2deflvmuv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ssnwrrpp.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2cdwtrvqc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2obgxvmgp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gfhnbsrc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ureczozi.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vyeuwyrz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2qqqqrjcw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tfkcuqcw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2clokhmhm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2qgcfumcs.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zfcutlrv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ypaznnhu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2wrjudafr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2wemshbnh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2dmbslfsf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2jplvrfyu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2unpymube.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2krswynok.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2tpjvympk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zmyczqti.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ieaqmbqn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2xfbogloy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ouegtiil.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pukdzrdw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lvhztbmf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ridboxdd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ebtcqrip.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zijbvlns.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2dylkcsyt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hgtnepww.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ncowgwef.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2taonvuyl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2zyfedjlj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hjhundlt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2cywtsyba.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2lbrhbcqi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2rigrepmt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2gaoblphc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2uannehzw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2frmmwtsu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bhzljyjg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ueffmmli.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2wuxqqlol.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2sevjpjjl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2unthyhcb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qwuiyfdo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2uapdbcwa.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cuwgvjpo.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2frtxlmgq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2xgsmcjbh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2vkghoegz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2vfejjcyn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2yiyuiipr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2adxctpux.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hxltpoys.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2vqywyakt.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zijmnxzh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xytgfqha.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2yoremjcr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2wbkjmuzk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2yecugxpr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2pfmiyhrp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ozvuicch.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hqeapyya.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2yoiltqei.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rbykvazg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2jzdbhogv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2awfueawv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2yrdcjfrk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wqaikehn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bqyxjakf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2qjzyjuyw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2wkepurlt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2udsfoumg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2reilxgwz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kqunrude.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2tbuxssyz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lmaekicw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ozvqgvpn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2zfnhtxkz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2cdnquyzd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vqtbeidf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qktjxgle.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2evpiktua.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2xtnitwkl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2holgcfdb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2myuujvnx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2anekprpe.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mflwepnw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2stihevvy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdsrnchz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kfdvnbcm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2zehrewjr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dunhuhmn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ljishebz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2buuwgvms.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2mymogmkw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2unmpoepl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uiqigyno.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2odahhner.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wnoksyvg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2gbebelba.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pptewngd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2mypjgqsj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2gdzxqobo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rpphurwh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2uoqhdipg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wspvofkf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2seugawgq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2twlzvzwn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wylddqzm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fmtpxtki.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xyreixzm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ptolsyvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovnnntfl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jmbcdnyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbhuqtkl.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2bspmfilx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2gyqpwtnd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2aniqdzso.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xtojnhpm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2pfrosanh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2otncugat.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2nrpuosqt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ocnnuyxj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ibqxfmho.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xtwbzdou.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2zxqmbxzp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2oantpaba.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2wqsykwnw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zkecblcz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2eknhoxii.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2dntelxuw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kwaypnad.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dklvhfle.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2bqyspljs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2brswrpfy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ujzhmhwo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jqhbryfa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2qmmspcrc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nwseufis.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2yspknjxp.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jjznqzak.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2nebnaimu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xukyavwv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2btfuquyz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2emurmjbk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2aurvssjp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2qlummaqt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2kqxfaqww.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2uqavkoic.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2wuouscpa.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wpfmdiny.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2tpzooawg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2yrcukwhb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2iqgyaonj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2grcceggp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2jsdhzuln.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2cboccucn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xzpavpwx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2falibehy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2xqakvinx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2mqufgota.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2boybdzmx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jejojtoa.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2myrujilo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2nsfqyype.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2leqbcvjs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2syiyyjuo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2nlarhhvk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2typpwgil.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2nkiclbcf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2xtiklrqt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2exdsnoqn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2npdhelbw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2iuirwbku.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vmlrvykk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ipvayuto.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2xbgodeem.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2zqzcngih.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2khosjtbp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xwetmyhs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2sxaibmsi.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ottjrxvw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2rmyomuhi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2kqurpujy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2owsvvcxi.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xhvuitdn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2mwxwlshm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2gvfbgnpw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2wlcgfjjq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2wfxzubfq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2brnpbpwc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2lhtytmml.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2jplriams.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2nwgijepp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qwekscwr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2shumtcnh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2nlxkmrif.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2iknkknyt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2mdkcerfe.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jlttwurk.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2tbsxipdn.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2myesiuhq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2shjlnvve.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2janltgkz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rgmongrw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2gekyigkf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2kmhscpqo.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2dknzdzzu.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2vesmvmwz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2abpxiguq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqvaupjr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2omjfnnzw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2wjkamptp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2hmztbsux.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzdjvsvn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2vmauehgq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ewwbudhn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gyeqqedx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hnbntqkh.html


<!-- 参考信息 -->