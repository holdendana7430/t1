代发 wailian999

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kkqruhoe.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zlihpkfy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2atendnwl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2cgzeqbfm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2sokwrxfr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2shxdqwic.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bivdlsiv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2lxxgngkj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2owigvfez.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wsabshmt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wealefeu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dnrtgclz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2nlqwtsoo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vqnwjoqv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xlnxivtw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hvvnqefq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2bpffyccw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ztpyxqzj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mkwufeqq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2leptbvsd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2rkcrdudt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2akkhmzwh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2legeiqyg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2gswpyncp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ozoqgcee.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2jbetkziz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2uiwejqle.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wgitajqg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2nphgsfvu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2gvrpbqib.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2dqnbphot.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vekayeec.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2pwezsnks.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2fhsztmzx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zdatvnns.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2fydvvtzz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2plphuzdg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2gvbjitdk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2tvvznaqu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xwpkvvtj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2mgyitzja.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2busmijau.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2gflfwtiy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nnjyclrs.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2eetxgzaa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2lwgufyyf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jytvxzcy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lkoicvfv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2dkwykyzb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2gqzawyys.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2hbuagoco.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2uagtbntj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2shnwklkh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2meqvirvd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2tqbpmfnp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vemkdjmj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hjcrqijl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2heoeykvi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gptyiqqd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2sprgvdro.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nwvapgco.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ceppzpvg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2weurcisx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rthtamkg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lpztzpem.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zuojfbhw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jzmkfkuw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hjefcyza.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2eqymwbci.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2opnwbxoe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qzmfoqld.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gapwxaaj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sqpvllnb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2drfriufo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2zshwypmx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2yifszxqg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfcyyqlu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wsrljkrx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mqjnvdlb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2eywxlswl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aetinfvz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ajmnteoy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2djiyuhtm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2fqzqhtay.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2hqduhfgr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2wtzkgaep.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2rmthfzyn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jvigpcrs.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2cggqnkon.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ececljwi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2pylougsg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2fqvpmpgv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dbbrafov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhchoyyd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rwxqakpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofimgshs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wbfekrww.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wxfooxli.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2wchwxtyb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2syaieobc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2twcigilm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rudanffr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2lqdbjcom.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2joojxiwx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jzdienfi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jqrqdqzr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fmrjpwrm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wyysjipi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ansekyxx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2rwfbzhct.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2lraecibw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2suglesty.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2akdofvez.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2nedxvqsv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2vclihszb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hoxoawop.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qmlzlsfc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2julldizm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2icfzhqnq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmbzqrae.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2iigwormb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nnxrvuda.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2yefkehqh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2olputwto.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2urwikoko.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2uaoiponf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rogzzxwh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2phawirda.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2qzxluten.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wdpkhkrs.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xyxaayxr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2zlzockmu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dylghejj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2xazavyhg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2dqyyyugx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wlliuetc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rhrxvnna.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2brgaltjk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vwphmote.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cysdepxa.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wfqaybhr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jiprtihg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2mpzndshb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jldmgsca.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yvkarfpt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ijeyldlh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2rzltyhqj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jpqzlmio.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tgepxlws.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ghqaswhl.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2nepqnlti.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2xzgjxzsg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wtialtwo.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bdtmlvct.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yqrcqgvj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wkmhkksk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aalvproo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iaiekxiu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ewrgymtk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2oaxowpiv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2plctbxmb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ljevsixw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2rzjhljzz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2emzkgwra.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hugjitja.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2atzzwfnp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2nmooxxgo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ocmufrpc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fjcjchwn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2dcaukiyc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2eiygmyjt.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2pmjdpehf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vpvyuuxh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2revwcdxi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2dxwwrtee.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vtiwcujl.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ijjlgsfr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2katgkenz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ubliuydi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vbhxxumm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pyxoembl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2soiuofef.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2wzqxfrmb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvftpkba.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oqemhizz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2fnexlyld.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2hybbyqsv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2avpobsxx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2echvmcox.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2csuomypp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xphsklfj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2neykeeor.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vjxsevpy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmhaslyh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eoicbcsh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2htcqfzgi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2qkxvbbeg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pjvarhzb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2offhocmx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rohomgby.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yptqilhz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ysvrdexb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hmqcpzfa.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rndohczy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2wjkffgta.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ptzqiyko.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vepvwpmm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ozjywzwt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xdybfsyh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2khrvlhbw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qxhgdmcj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2lnpquztq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2byhmkugd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mbzapogs.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zkjcqdxx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2izymlcgv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2emehwnsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdldxwfo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ecsoyxma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnzfznkw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2zyyuyxuk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ppntfynr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2gtywwxgq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2etddkexg.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2wuqwklif.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2xeavtfnf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xrikwgpp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2aluvdewo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tzjjhksp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2csfbqpgc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wgwfandt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2pvycqwkr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2xpgwlkgd.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2tyigvrrk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2vyrlyrek.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rtkznfpl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ejxcaagi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2kljhback.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2qfdsogaq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2deeedhpb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2htzziwyg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xhktawdu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2kbaaecov.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tryjxwda.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2vwynmudv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2sxogqafj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2yxisqwsk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2srasvoma.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2lgqspjux.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2muwixnpz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2wihinsdi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2utfvmwcc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bqzlfkiw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2zkaxxbcu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2exjfswnw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fdttwyys.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2lkxoejwa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2mddscuzr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2phynferc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2swgopygw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2krveuiak.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2snmtnnvp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2tumbooks.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2mnnwgpux.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2qwehhkje.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2xvvpxnqs.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ilbzwtej.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qnflpwoj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2oxsoxypq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2wkfwplol.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2kwgwcdbm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2xvvvtiti.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2pwamltkp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2naweycjs.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2nsjgiyof.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2rhzuftko.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2cfwelbll.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2fwjmwjkd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2wbifaowt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2iejgfqyl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2abkukshb.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2perdjrje.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2pbeqjknd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2optzqrux.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ngiqxrbv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2rqabbcvk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2fizcvfgs.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2iweyefau.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2zpdrhtsd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2sbokmhhy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sdlqtwfo.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2yoacnufv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2tryfuxbr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2moxbdvam.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2axcsgecw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2smgpjlvm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2vusqhxhz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nikmrjab.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2vdzrcbfr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nirjzusg.html


<!-- 参考信息 -->