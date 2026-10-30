代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gyffxlxps.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gmqgierzw.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gxaivwrto.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gcnybgmif.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gdejhvowg.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/ghdqdnsxg.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/godnurojc.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/guftbcypp.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gpobligvn.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gvkicjpxn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gxazhowpi.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gullzuufk.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gjoqbghgh.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/goywhleaq.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/ghyfdbfgx.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gxstdvoaz.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/ggzporfyr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gaqzkxzvn.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/grijaglcb.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gfpifpkmb.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gbmrszmpq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gcwvwhlgq.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gveydzcbj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gcvizogst.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gzbzrltky.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gdxnqbtxi.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gzxwqfkou.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/ggqajebdu.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gkpgmufvz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gtfodvabl.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/goiqzawwy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gubcvuqbu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gnuuojago.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gioqlnakp.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gcyrdllpp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gwoumskfi.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gchjyxvvr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gwlfwnxnt.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gomwrawof.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gnyuieowx.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/goezjowkv.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gmxaxinyy.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gxhunzsor.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gegykwidi.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/grpwelxzc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gqmcjjlrj.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gwzmzvkut.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqivqvquz.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gldrhiddb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/grbrbjipg.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gqfxetvzt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gqwnpvnkh.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/geaejkxtu.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmzpliozx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gnfdamlgf.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gcxreolgr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/grmnehkql.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/glilqesxl.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/giwbeemcz.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gmlnqcyvy.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/guswjtvat.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/ghtztcqrq.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gpjgkzznn.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gdsymdmha.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gpnrbwubh.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gdcsujxed.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gzrbvemib.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gzbwsbico.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gvwgmvdce.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gdnilufxp.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gwvohwfoi.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gimyuhdts.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gbboubsea.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/grlckaxyn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gvxqvcqzq.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gosbdqzuq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gvdfjefom.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gruoizwih.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gqmpytotp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gutbhcumu.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gibanwpni.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gdnzurocm.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gobjuezxa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gkmeurhsi.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gbqsahxhm.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gmtttmftq.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gdqykgauz.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gyuvkgfox.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ghueynwmu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gsbgqgiud.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gharychar.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gsjsjsbfr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gytziwgns.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gckmppsjb.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gdbrjetwk.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gffbgwoap.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gtpgztupv.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/ghnrcbcep.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gfbduqdll.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/glsxfzdwt.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gjhroujnf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/grgrpnlgu.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gzrdymrbb.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/glpydsxhe.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gbroxgnqv.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gohyhfypt.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gkwqwydqq.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gfsulgpkc.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gzqbfkcli.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gqfaeabqz.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gmtnlyebx.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gclxkndga.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gbatbumbw.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gssimdsrr.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gokieskzk.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gzohfwvfd.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gvojtoubr.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjhnnksyk.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/ghjgsqglw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/ghchfdnjt.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gthykktvd.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/ghgdfhfgo.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gzskloqld.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gkkcndene.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gxcfllioo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gzzdgfgir.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gybyelghi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gjuatogkt.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gfrurmgpm.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gwqjkzxor.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gbdukodvc.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/govwmhkfs.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gfsygopls.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/guzykqewy.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gngdftyjh.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gylvnpnyv.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/ghknlrntd.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gaalfptft.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/glbrcffag.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/ghrcqnmbv.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gyfyqscuo.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gpepmwprk.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gjahofyoh.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gwshhhjrx.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/giyxvmdal.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gwppmires.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gktwpvkgn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gshthmapw.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gxdqnlzaa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/goauwojfc.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gccsfstln.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gyjdgtmrw.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gdgytfrcz.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gvajmixos.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gpfdlrhje.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gsypzfpgn.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gwwvujcec.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/glabnupjw.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gdbtjdzuu.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gpqueqxhu.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gzdwtzuzp.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gattrxway.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/goldoodad.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/grcmmvzza.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gpvxjmtjs.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gkbcdhvwx.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gwpotafwz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gipunedvf.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gfulytidl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gnlgbzapv.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gjcgctfhh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gdjwywsdd.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gjtkewnbi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gvvwbbabu.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gdawnfhey.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gnypqucvk.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gmwvjylwf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gfohphqff.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gazhelnqf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gwzawzzrt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gwxapvpeb.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghergpwro.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/guxruphxh.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gbvouunbc.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gorpfkxbe.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gdzpijwzu.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/grzxihzno.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gzlfqlccj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtscidpfi.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gkguwitka.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gprdaegzr.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/grbqkurml.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gqjcmyfzk.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/goolyjqwu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gjhxcbebb.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gbtbyysey.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gpnxttnsj.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gijqslcwh.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gtpgrjajo.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gvsaqpoyy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gshnmqefc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsihomfjn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gjuevryqo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtnseeztq.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gofitrxdx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gifqynupr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gbmovdvoz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gpuckjjzz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/giinquqau.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gypznhmdq.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gaekxjqmp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gepxippvg.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gwkkxmgls.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gdxbatjcd.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gcmylpgnp.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/ggcwzoddb.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/guppvglmv.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/greppirhq.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gexmodjjp.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gdrqbnntg.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/genysubjy.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gdzboumln.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gdrvzgcqo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gfajowsdt.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gcdsfxpza.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gfukuvfgv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gnnmfmcrv.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/graohlolo.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gjbmzcjll.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gqeerrwob.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gjpmwjraq.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gujhhgqws.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/ggtlujwsm.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gimlfndrj.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gvukziaqn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gipjpquol.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gqnpvddwm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gbviwtabm.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gbefkcsaz.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gyvjmfiqq.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gqtdzmdcc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gypsbegjc.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gjfxlzcaa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gqnbylfym.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gygfxfryg.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gwyxjovhs.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gaipprkhp.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gktvmrysw.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gnilvgrlf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gosnxduah.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/goenpkmhu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gjesrvzme.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/ghfppnucf.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gdsospnyi.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gemvbmdcz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/georxohiz.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gswwfkedf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gulxrgvnt.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gwzurocau.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gtmxvarmx.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/guggwwiuj.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gjxfmawsc.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/ggunsovbe.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gwnofaibz.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gpfvxqabj.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gwfmwzolo.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gkafcxhti.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gtpcyxzjc.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gaicrxeza.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/glqzgxexv.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gwbkvasbh.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/guakpebhg.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/grghyvujn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gnslvyyky.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gxdrjiqhw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gvcjwtfhb.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gkeiptltw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gydmonpkc.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/ggkbdwgsa.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gcbpltmda.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gdxmofhzr.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gqqnhgfwn.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gttpslbvv.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gyvnyhurp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gtmratwvo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gwytzmpju.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gwkuztuik.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gtkoqechr.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gstkednoj.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gzegyfxmb.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gdozkgvgp.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/glnvrklce.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/ggjopetul.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gidmtsnxt.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gangvrobv.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gxyjagees.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gsmpirita.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gugrtgyez.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/grgdziljv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/ghkgrfvkq.sHtML


<!-- 参考信息 -->