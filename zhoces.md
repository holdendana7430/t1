代发 wailian999

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3fugcpfmr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3xmjzsknt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3svrwnyqb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gjdsavob.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nxmvadfe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxtrbelf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3dgbkkcag.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hvhbslsv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3bkkmsiab.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3macyxzsm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3isbnzukl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzlnnphl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ixyagpjm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yypyytxr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lhnvzxkp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fcfuctbv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3drkihhwi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pikindge.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3bdkyfmgk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jmysoqfs.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3atdouxhd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3fcbxxyvg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wyzyejfo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ridynyin.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3oyxsvmfw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vqfyvbkw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3dpkklnmx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3zajydero.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3dqsekvxn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3iprtmpbu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3gbjsctfh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3uqoldomj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3iekvttwd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3njjyvply.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3pablrnjy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3pdsuhpkq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qhxwmxlf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcsihvqz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mmrzntyh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3kwwgedbf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3rcjrteoa.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3rktbhstl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3micisvih.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lfyyvyms.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3menuvvex.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3igilnnuj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3wmecidpb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3zkjrcpyt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vggrmsoq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vfphcolc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3yndzpftj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3glrveibq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yuxxadgf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ttztfjkb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iyslmked.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3yqxmomlc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3zatjpdsp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3fnhvrvoe.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ifwtcwkh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rrzzzzxb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ujdsoblz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3tlbjjwjj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3virczzwd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3gcjxcbcc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uuavmwjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3objjesvp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3eenzasua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujkukpnf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rzxolynl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3abuqnvdw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ligmomct.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ufivafkc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3sivlafqe.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3iableuod.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3tjwovtcf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kuvphvma.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3zbnfmizw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3vdlwwfyu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3beknzhbv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zaevpmog.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uavqbava.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qswflroi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ncvuzirb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3twaetxvr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xyosaqmh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3czaqgbxr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3iwqgorpd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3wclrgpun.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pbsaejvy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3obzuvznk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3mqpyjkzx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3azjnkeko.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mmzpxnje.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qkjiohua.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qmhjmrrm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3yqdtfsyp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3fmwcirqa.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3axvwndvz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ikjpzstv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3agdqeycj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3usyrfqpb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3gpevtpfv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tqffrmww.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3jvizultq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3rxtjjmhp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3rotpjobo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3kobaliom.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3tlgdjexj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wbmngtuv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3bpkvmiko.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3pchbvabd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gbmweqbv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3batowoxp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mixjissb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qmkxculk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pkkpbqmk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3oiubbgmw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3idcmtcxz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3qfsfjarq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lbzaemuf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3iuvndtct.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3khhqiixs.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mrigxkto.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3biiaqyhd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3conovryu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ykyffhns.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3cyrqtxis.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3lscttojr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wniwbrwe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zutuaesz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hfxffbvj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fssqpkzl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hmmjtvfs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3vevdvqxv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ybyhilub.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3shiahvyd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kdxzkrhn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3dllpycev.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xzvlewrx.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3wgdhcudz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wwwgofsi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tywdgwox.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rrxdmwml.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ugzpunzb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oqwypwwj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ugdgzodr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3nukevbmu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3cequrcrm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sveskdcp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3moxjzmhg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zvjryhbk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3djiwxdtp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bpxsssvl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3czkghmaq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qvqleixj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3spoxtkxl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jdcwythx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3pqqfzlms.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3nevigtfo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3fpubntaf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3cfmnddae.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofjoakvq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3nkgzfwca.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3yleceyqs.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fsfnsyzn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtawljnh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xcxpndko.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3emyqqkdk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ctzvltgu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3odisuqae.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wslokjya.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ctwavdbz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3bmxtcnox.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uccrlrpf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3aevfpasu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jeevwdiz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3cosorwoc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lflazqst.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvxklwmd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3qbfrtjzx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tbgpetbr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ocuytlas.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3bjostrdv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3xkkqyjqg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jydglrdr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ueweblnn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yoejznen.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wpiarmhk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3mbzshvkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wubdybyh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3yhfmrhgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymqopyna.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3icjoepjx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ucxiorkc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ccoptdtc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3crkkwvck.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bjwixxps.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wuympkzp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3iekwmtbd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3zmdslaos.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ryezrfim.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pulzhjst.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3cbiefwqk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rmgupnox.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3obuhbeen.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3yxafcxxc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3bbacgboz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xafguevp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wermaqsv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3sddpxgna.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ngoicjck.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ntncspig.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yzqrxozf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wbqcyvog.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3yhdsdwov.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3iextxuer.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3sgxmlank.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ytyndqfs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ndegadan.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3yumregai.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3uwhvkblu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nhpslvwc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3epabnrpl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ytjiyaal.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3engffgde.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3msuvcvet.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ukcwsidp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hfxyzufn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3nrcpysve.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3bmafahjp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pkimucof.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3syquvewa.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ooqtbrsn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3dcoaqeji.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3yapsyeys.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3uvzbhkid.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3amkpxkuq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ergycqtm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3tajhkrog.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ycspakqz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3izmfhefl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3vmagbain.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3cvygfalv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3wxyswhev.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3gttfozie.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ylqdimcs.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3gvzdvemh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3tyqmavdj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3fzfdsius.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3smbsxdde.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3awcorhti.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sfssvwck.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3vleilsiy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3mmgztggd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3mihrnjot.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3hrehnvih.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3jfkwkzdr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jjqvcqwl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dghsfkng.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3hosmujcp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ukfsovlh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3nibfildo.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3bbslcidd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3rlcgddok.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3owelgkxe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ffnqfahm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3xgndurrl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3oohmneyg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3pwmhsdpr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3vibdppkr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ilbbhclk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wcjnnpuw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3adfbpfzs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ffeonsai.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qzrohdiw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3jxzvrhuo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3njqeurdu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vtddbuhz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vxgsvwkq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3xtamesws.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3rhxgkkik.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hfwxqsid.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ednuoaah.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3jrubateh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3fiivogjk.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3xvrwymab.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3lpgvpuod.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3gbbrhtqu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3fmjtbwks.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3srsgraqb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3vthjjqbl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3kcgftzic.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3svdkhbxj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3xgwpsqls.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ekyuowvh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3edkmapoo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3wijbdtth.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3mnhheeva.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3suqtbihi.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3shhscyiz.html


<!-- 参考信息 -->