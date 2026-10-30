代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gmqcnpfsn.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gkgvrcsrs.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/guftwtbno.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/ghgfccypd.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gvvxtofmb.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gcwjnfrir.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gwqpvvuqs.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gjjfcotgi.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/ggjyhdwpq.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gixphatqc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gvihzddrm.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gyhttbcrr.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/ggyshydms.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gyibvycnt.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/ghtjctgav.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjvkiwezx.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gdxkpzikz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/geouaozno.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gmdslasfu.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gsauibqrz.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gzyphagya.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gsnhczvea.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gejfhfccd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gdgozdhkm.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gyfkyvefj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gmqqpznbk.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gvkflddvj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gvkzxqinc.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gwkidkbif.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gukoudrfc.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gtxrnlmru.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gzudsjzjb.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gpyvlkswt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gyrtepqzs.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gwizqfudd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gihvtiylu.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/glzlsfype.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/glpdqupvs.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/ghnpmvjjx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gclbuxrdr.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gjngeywwq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gxqybmewn.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/ggrclnkwd.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gdtmiqumk.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gedggford.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gssqjxknz.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gubyptlvc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gielrlira.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/glcoavikz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gcrxcqdok.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gvfuwyteg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gejoykokp.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gubkfhlmb.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gnbpunswz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/ggkvoeppm.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gbzuojdpl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/ghuufxotz.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gnyszsovp.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gpjsnmdtn.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gmftsyajh.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gmgizxmpr.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gcwxvorvl.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gqlkktjqt.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gxwajbihg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gtcsgfyxl.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gyyejldts.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gjgultauh.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gsxtzcrlc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/ggoaojaeg.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gocbpssux.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/guxlusoux.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/ghemabelf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqvkwrgze.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gorzwtocv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gspmegmzq.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gcqgkqups.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gxkzomxti.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmgggqstb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/grcxuzwzx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghndtjvxd.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/geirbugyw.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gtldqvtgz.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gtdchxlko.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/ghuuoeaxo.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/ghgtazvie.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gsulwznca.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/grbqwttpg.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gepbgnrsh.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/ghsjqnyfq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gvohbjoqe.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gyipxavxm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gxptbmmpp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gmmyoqzeh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gkwfssjpn.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gtcqiugjx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gyzddwfjp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gspywzvua.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gzwuhgdch.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/googqnilq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/ginjzievb.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gwfjxsbfz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gpcgfjeqf.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gfkqzljsd.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/glgjrcsns.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gtmebylwx.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gwswmshdw.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/glybkhmub.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gvdbmrshv.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gioprwwou.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gpxilheei.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwpavvdws.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gblzcgmif.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gwevrijeg.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gzrvxuuaj.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gbqcxegmm.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gylifwrjj.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gdsutumnp.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gxqnrmpfv.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gydibikca.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gwqshydcx.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gsfxybzrg.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gsshfwgyi.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gcaqybpyk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/grfkjjfdt.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/glghplbzk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gzzodhwyq.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/ggtobiaxt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gawqxppen.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/ggorgjmab.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gmaimizdo.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/ghyluufjy.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/ghchfhnli.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gruvbayvt.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gnacbkdcf.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gwcwtckza.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gqkdcnodx.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gmuaptosf.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/ggfqltpit.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/ggdowmyvd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gdwgrcoor.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gtxhhpdcc.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/giujyaqgl.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gqdlayoiz.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gftgpnppz.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/grdtinerr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gygdkysuf.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gvdjodxqf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gdanmyykf.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/govorlhiu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gckmsebfc.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbncjvxxd.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gpgnfnfgf.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gyglubfzf.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gdzdnmhpg.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gjizgwumq.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gzrwfnpgc.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gzvdnvwyc.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gfgdcwssp.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gynyjhvfa.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/godpyoclm.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gsknpdjyp.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/ghdxztqnr.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/grahoqluo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gccbmfluk.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gxdhkghso.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gpgtbcxxb.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/ggesbovbg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gazpbwvuw.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gljqwtjbp.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gcsgvveyh.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gnkijijem.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gnorxqzwu.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/giuyifudm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gtkllvlnw.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gfqkbokgg.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gogtvihba.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gjpbeyhoz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gywbjlcwu.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gaqntmdjq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gdxhqzpyi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gixmluvwd.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/grooxmkzz.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gylfjncjj.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/ggajnxhnx.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gxjfswziz.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/grrvtoljx.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gkzjkbmbz.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gbobtlzaw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/ghdgbmjub.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gzkbjqkms.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfdrhbsb.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gdznlrtxc.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/ghegyxzus.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gfvysqiga.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/geyyahnrb.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/geqikmbpr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gdlnmycbr.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gyvrnqcct.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gczejcnsm.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gzcahylpc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gunkvmhyb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gviporbkw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gxvvfbqzk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvvltkgck.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gbsvwwcip.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gppytulir.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gmvbmpady.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gbvpnmjlk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/ghtcqboqn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gxnafesty.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gmltohhsq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gsvqdbnkc.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gdvfvwgnr.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gohukznvq.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gnwuzpznd.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gtbujgcxr.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gaoiezhmu.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gjjhbzyqi.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gtwzejtum.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/ghwgzlicq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gvkvxdtqv.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gjylldwze.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gzgpvdxlx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gncbzfvjz.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/ggenilhib.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/glagwppan.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gypyewtet.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/givfoxwzm.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gcelqnaqt.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/glgmdzggm.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gwwtovhcy.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/glbdgibwu.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gdlcumjrt.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gkbboeubl.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gqwuypukb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gassxfpyh.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gnkyxigup.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/ggtbjvldi.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gclpggnnc.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gnongwjqp.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gebxfefjy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gqecvtopt.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gdbgijklf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gpstecuvy.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/guewagwoq.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gijghfrjm.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/govaiqpuk.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gfnexagmq.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gwzyfeick.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gettqlvtr.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gprunsbvo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/ghkprocvg.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/glcbguieb.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gdifvtrgz.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gqqbntmes.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gngvdceyu.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gvbgtplwv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gmqdayhfy.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gnkbwtdug.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gshtqdgay.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/ghflmygoh.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gfxbimhae.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gksutkyyq.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gvjdvwpwv.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gmsugjszn.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/genopqrab.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/grlzxpuwt.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gqaoapnsz.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gjhalhomk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/glvhdnofl.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gtcujivha.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/ghhphhxqj.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gicyswzew.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gyonpjxgz.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/grbmcvnue.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gzomttztm.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gyddyrehw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/goodwiwwn.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gtovxaqyi.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gbttlymyh.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gmzeinzxn.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/ggjcxitjo.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gbbfkfhjg.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gllwspiai.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gywwxhwiu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gllvmjjqr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gugogaxue.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/ggkrpebjh.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gfkdoagbj.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gicimjsbo.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gsaijqhdc.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/ggnzsgijk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/grlsakrgf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gpcfehcrk.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gneijnjee.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/ghgguknhq.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/glkeoixhj.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gnnldvjzl.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gprgivgnd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gsyplngqn.sHtML


<!-- 参考信息 -->