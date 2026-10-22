代发 wailian999

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2intohtet.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2kafuiuob.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2gbndmpoy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2zzdxexmb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2abiesooy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xtakgjem.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2npjpeqld.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fanosbud.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2andifour.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kofzmmsz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ytyuzpcu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ikbvzyzp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2emqzppud.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mcekqxok.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2phhldtjw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xrtyybwf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2auopbhdn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ptjodxeq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ymahmenb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rrtnzmtd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rnzpxbkn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ymcnvfcu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ywjrktis.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2tgfwlrky.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2zcoszbqw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2hksgukbe.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jbqdiwnd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2nhvdtpyx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ufkspjyi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2qfmmdvrw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gkxejdat.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmskhidg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2fazjjqly.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2aboesmor.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wgtqzghn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vfofpwkj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2odyrmgsf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hspgtjtd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ciscckxc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2jfoplnzv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2neinptkq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uhzobvec.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2etntasvy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2kbkkhpdf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2krgfasix.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2jffzdeum.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2duadhytn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2gnifetrw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2buucccuk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zvuhwqvt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2fglbgvej.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2yywcmkjq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjgzpizz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2hffxqlzc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bdlcrlzo.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ndmvryag.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2atzimtmc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zvzrwlkh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ycolofgl.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2xnlidhti.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2uwaicslx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afateupi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lqrrticw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iodigfwg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dawgnxlt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2judbpnrr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2trksulhv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2qfvxtndw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2nhhguztr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2flfszpso.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2slahbgfx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2yvqinwaq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2vzvdujvt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2nentyvul.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rtwkgxmf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lrhkmpsj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hjfwmiew.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fxkqdnhh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tlqucnsm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jneyemoi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2qoyyrkrb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2odmjuvvw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2sffxqdxp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2mjsyjbdl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2bhrkscim.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2tsskptqm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2rwzhnfbk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdjtbymi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hyygisre.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2acutyfqz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2obecxxky.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ddnedrcg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yymlewcn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vjdkgsak.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tuxfauic.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2irfkljmr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ezftjkrk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qkprfauw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lgvqphab.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2vdxmjngu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2pxibbtbi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2cmpwccwh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qjqlzdwx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jytmjjhj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2bfnmkxbk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tflfmbll.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2azzteoxp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fdcjptsf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2bilraeim.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2sqhfcrtk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yibwekiq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wbdvihid.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qgbmpxvo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2tzertmco.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2dtttgyxv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2hrbbkmnp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jfaeseht.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2cqnteemh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2swvcdkig.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2rqcdbthn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2oswxjuzw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2mtxuikka.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2gtqaxite.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2flghibkk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ectkanvv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vpjdrapg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2orlpaulw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ykwtwtpz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pgvkvzfw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2fnckuiei.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tdohovrv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2lmsuqofw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2vzeoxqhu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2khuqqyoi.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2vmsbaacj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2apquooce.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zugznrak.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hkrvwspq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jgwpdscm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2yklgwdmc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jzkozqor.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nulgeqsl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2blheccna.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2piwzzuhj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dfejqygf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xwugzpng.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2yechtiti.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ybwcrkhl.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rtdemaup.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2gizrahes.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2oadiweke.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ndawgmct.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ufuwganc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2eolunkuj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2whpmmzmv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2npcgdmcn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2laudlngs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vltsljnu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2kydfacrr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2bokfcxyd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2pxznqiur.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2chpjegac.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2onmjfese.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2didppisy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpgkdeee.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hwpbkdfs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2quioilqi.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fmovlefm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yfcwcrxn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vmsmukhu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uqdcnqon.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lxmhgvsc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2zlourddd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kburomup.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2diwgxbel.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2iiwlqyyd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yoekkfxe.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ovhkpjel.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2spsifzab.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2zcqcupyj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2pzozswxy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ownsxrsl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cvplimdy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2weufgkbz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ihfpesbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ocuxzkhz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qbasealk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khqwnfmg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2opymsmfl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2dxujiflx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2judxioll.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2dxodgzyi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2opnqellk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2yveztdut.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2sikudcpr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ylzcescr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2oqyxdtex.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zobratmv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xgnzinye.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2bdoevgla.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2yrgdctfc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2uzcdwtbn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2hvnsjjcd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2wfqlrrxx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2mtatzydk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2kfnjckqc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fjhibxmd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2rygmpeaw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2jqzsllnc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cpzavjof.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rgrdamqu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2nkalgihj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2seqnqcuq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ujqfbgkk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2kftsanjk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2zabrtmqe.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2dzgyauko.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ovipsscn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2sggoxrpn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2iqnpnhvx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2czidksxi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2rbdvdryx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mfiujqpx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2gvmtxmvt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2wtcfttsq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2fpzfidwr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2orwkctjb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2gyduajrm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2zxqsquww.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2pcgbmjtx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2nfhgstga.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2wofqnofg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rygtmeay.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2prmtzloa.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2fhusqkip.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2exzbdlbz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2srvtjkxq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2mrqqparq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2viucvpqc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2mcsmgomo.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2oahogwmi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cqaxqnhz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2xrclkjfn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2yurlrjid.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2zsxpqjae.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2pmzohlmg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dxbqzakv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vsosigkc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2iazbegrx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2hncqgzlc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zyyoigkm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2javgvehq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rmzppoyd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ivnmpjyq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2rbonjyyt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ivlnkcez.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2kuysszdo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2vuvpront.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2tbqcxdjx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2afzsxmql.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2nscjqsac.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2qspiwewu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2rtedrozw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2jprhxwyc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2rohpkull.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2cwpicyke.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2keyljqzm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qywgzrsh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2grifhapk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2rixhziiu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vwyryexi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2tpnomsvy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2cieicrwt.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ixkywxsu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2zylydnqa.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2zwuhyapo.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2audyxslo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2arenydal.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2fusiyghl.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2qqagcjmv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2lcrwhrau.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2hmsrdmag.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2miyfwbzf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eejxjvak.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2qanihhkw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2bustylfz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2nrnidsup.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ytoeovkv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2rktdrizm.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2gmzaslqg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jfyvdjkf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mbxngvdw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2gvtbsriq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2gcymjmzm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2motjipkp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2uezphuxw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2thyumefe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2dzbtdopm.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vfgelexv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jnjyttkt.html


<!-- 参考信息 -->