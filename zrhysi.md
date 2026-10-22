代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2cjzbiqrc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qjdydeby.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ofpkqfxx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2csccdfab.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2pjgapqwe.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2btqrhwah.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2bxamujbd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nyrggivm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2fayhtbrp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2imsarhar.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2sfmzadfa.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jwwzhzru.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2lwuxlnxh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jnyilbbc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nofdyiov.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2onxssebx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2pppihnwa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gcwmtxxg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2fwywvzoq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2alxwzvxa.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ktexvzdo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ahkrgcqt.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2uccalvyj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tjqxnolx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qrgzhnia.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2dykwwkzl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ubahuwlx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2aapbpdlt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2aooqmmca.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2qakuhued.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2sdykqelo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2sajqjbul.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2okvbftbn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xooqarpn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jylxuupz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xcxxgngv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2brxlygde.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2pxpgaezo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2umyxowob.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2eavojsvo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bzvxjkbp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2vzsertbe.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2homimcmj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2cvthvdqf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hblpezpl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2xegjoqww.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mybxmyfb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rwgadude.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2irndoxhc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2elfmoesk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ndbwbnlk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dpkaxrha.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wvbpzqrd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2euqgcuuu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hzhtbltp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xhdysscu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wjffitwl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2mdegncws.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2vvdinemq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2powcjpga.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qtmkvlpe.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2uudgrodm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zzisucbv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2dputgmca.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2txhtgree.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2bouxxjrd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2exjtytha.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mwbxtylj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2nnpqttum.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wkrcwctg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2gkcwoabk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kslmsupp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qgmvupty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eydzqsko.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2porjoxme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnsndiuc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2etdclqaw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kebfkofe.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vhjvcbna.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2uyzkgngl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pvahjfbo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2przaedac.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xuxvouuh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2asropivh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pbywrgzv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gjdqaceo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dlhzfkwl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fzramysh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gvicsijs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uwdqblxe.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2btxywyne.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rxbdlpbk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2kudphsiq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ddoeoley.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rxkrvhlr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2nyubyhki.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2fmnpbkbg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ihfludaz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2fznrmsnr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2chsvibdk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qtswqrzb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2udpokgge.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zjzczrql.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2sjgpsdgb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ffhaxuhm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xtrvvtxs.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jxyxrndf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wvmppreu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2aonoxrcm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2wbqskehp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dskgtdjn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2uzjvtksq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2oswzowjs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2iazijpmy.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jqoxmtpd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gftysshk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mcmvmbsd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2qnwxdycz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2zkgprtgw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2jwtlnbnf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sisuzkfg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pywsgwvv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qwbbdroq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2trqwtpyq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2sgsisfxx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vvgaldqx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2cbikvcbo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mgjbbeqa.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2mgjcozns.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fkefmfur.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kckuakiz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2hddelkqi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2aawkjxwf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2gyeqbapw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2eknlaivu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2vwtayafs.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xsalqaqx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2neshzmow.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wbpwcgkn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2meffljgo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2qzqemhsi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2qfduuyvk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2matzxhum.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2poxbknzs.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2wufqcggr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2amgqqbco.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2stnhhvog.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qfmtzpre.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cpguenhs.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2yqlqtkxy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jgljdpmq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mbliejhj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2leujoomb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jqplorje.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ppadrpjc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2kzrylguh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jzbbtpjs.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2cpfgttcd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ljmlvwdn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2qqcnsrln.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bzaugspj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2bsjzfhhn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2guhywvjp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2yjjcutnw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2acmxotgx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgtnglan.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2hkzwsltl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlhtwpqh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2krerhwcg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fkthxycx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2swxmibzn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2idazhxck.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tdqhnoll.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ichuhxit.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rrajztpn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2poabbvor.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjzenxgx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2crgxvbwl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lgiggaav.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ajgdjwje.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hfuqjiro.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2swaiejrk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kcmmsrzq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2auobfjmf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbaruhkp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uriisyps.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ghhftgdu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2iguedfcm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ulfpnzsc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qxwksijx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mnbhwpsk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2qaicuyhk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2yiipmvng.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2rgyfqhxp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2caeutyvc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2wvbvgtwe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2tvvjaiqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ralxoskr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2syyitahp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efhbrsfo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2gaimsohm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2kzaqtnjv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2nsoyugma.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2oeekywjn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2gjrwlbpz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2zcivaqtc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ltiqecgq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2fhirxxgt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2bnzoulnm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wodyglob.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2peqfdhcd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2plcefema.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2nigacarc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2imihhwvi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xbtmluka.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2zaouybxr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2cbyyksie.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dhzhtdbx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2uocsoahv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2lopntebm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rygsffnj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gwbllbkh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2cujcvpot.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vlihtmdh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2qiincgxz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2risghevk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ruwdxzss.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2etipfnng.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2yseqkikl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2vgygexkl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2xsohcdya.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2hrcaljee.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2hofevumj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2pptsipqo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2oktkdmtt.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qgxghvcx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2wwvgkgin.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ecfcsqag.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2oeycresd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2nkshejyx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2lggeqfsw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2yuuirlod.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2hpyiqbqt.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ascovjqp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2leagkcxf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2pgwtuxab.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2wutopsta.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tytlqngu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dsymhvwn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ozwwwgiy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2mymxxqua.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2hpggxaft.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2kfvxqqbk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2lovacyus.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2yufhaxem.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2klpkknrz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2vepetklp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2outwgtqd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rsfzgtln.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2imjanxjx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2brrovdsq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2gunhgptu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2laxhihgt.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2yxkfodob.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2zfjveupd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2kcxsyopy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2tiawahld.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2rchihaqi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2sxmmxljd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2hbggildc.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ogvrralq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2blviagxa.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2esjtcksg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ouhjtbor.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2algwxayu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2wxktwtvu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qlxuagrc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ihrlizuf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2wsneofzi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ibhvfitf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2rvieatdq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2yziyrrcz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vpqyqufc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vzduasrc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mmqpzpzq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xqvnqbhf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2dilvbmjp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ssqasasn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2kqoxicfq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fatdugub.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2idncsbpa.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2xovlzccq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2enjtkipv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2fegaixtc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2cakbganu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2typaryxu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2fyqftjvl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2fhyevxsy.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2rctdutnh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2psjyncqm.html


<!-- 参考信息 -->