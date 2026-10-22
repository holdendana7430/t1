代发 wailian999

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2oywbiauu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tzzhpkwt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2oaivdxsz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qvrtxdtg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2bmxuisvi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2gebqwfaf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bzejrygi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2dssqysev.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2sicgmajh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rtpuuokm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dtevhjzg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2cmehpfak.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2tohmcfii.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vekctpri.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2rjwdlgna.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hvzgryif.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2bjfevzeq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qwxnwpag.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ijipvlka.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ccndpxoa.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tbnuxngu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2qcmalokm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ezghbbeu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ukozsitv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ylsktyly.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2odytedvt.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2tkixofln.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2cuylylof.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2etbbuhha.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ryabcjpo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rnralqtq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2aditodjx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2inxogxkf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2godhzpdy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2hlmusugl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2svvqznlu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zylpkwlf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2wobidtpl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kmknpnzy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kjtnfaui.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2compmtib.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2vofsoiuq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2qcpxkyul.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xebdrnqc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pmbozuqy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2oihnftpc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2kwbeaqrb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2bdobdvpk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fclmlika.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2cynogxkp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mhgyiipg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vjvyetyb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sithjlob.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vnpdobdq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dropqnrh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2oksspblo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2suhaaske.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ezgvtrdw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2encplimv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qenijjnn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2noelmomz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2fwcnbpsn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2awqjsyxo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qrnkikco.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wtzbniba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aordcnqo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2phbslzou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvlljpez.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qutfokxs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yewivilt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fwzviuzp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2kynscpds.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2kbcewrjw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mvxexmbn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2eoucrwxg.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2owxjutiu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2nkobbhos.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2wknpwbtu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pymwzxzc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pqxyriqz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2exnaabhm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2bbjzfaxt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2njjjsnfw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2iayzxlwc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2xrcbxumo.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2xghfqgen.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dsryyfto.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2kmuoukjm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2pnwpbzmk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2dbbulivp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2tfwjfsnc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zobqxunt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rldluwhy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lqzzrgyb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vziajbri.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ptwjkejx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2sbwshrlj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2tygavusa.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gbfbaylw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rjbxfmtq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2clcjxkpi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2isiqsbom.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2plmfbcko.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2sacgrvfr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2trkummgz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ijmadsdx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2fmwcjuep.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2inhrvzbz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ztkhekdu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2eketxzcg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2yxnswofv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vnebswti.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxsndult.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mqadipsa.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2qzrmhydg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bxcwepnr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2bmrguhqf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2iytjdhxo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wquilbbm.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fmisgpei.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2uwslozbt.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2rlhihzqu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ymahrxus.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2losxdhws.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lftkgefe.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2veogsrmo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2xwqyujni.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mefpxyqc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vmwzzfvm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bnhfsbkg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rnhqhvoe.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uiyrckzo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zsbsvnzc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zfqrcfvb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2khrlfqru.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rmdlxzem.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2hgiohylo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xnytclaq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2owpvbcsm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2yacpclfu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xloqrzdd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ufmddswc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2nptpyhzh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ueuypxof.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mcmcmsuc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sioyzfbs.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2nknskxay.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2digyozao.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fusxdlpd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2qieuzrwk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2sitmbzrm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2znqntvvs.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gasrovye.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2jpyvnxqv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2xzxechjb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhsrzqkh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ihvxeysf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvkswcxl.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2scstwysq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xogtrkcd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xethnhne.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2nwpsxxwj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2sggenczy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2qcgweckl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fiinjsyp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycrnbqid.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sjeptqba.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bywodlmk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ivflmfgp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uihxgvfd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ttgtmalc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2yegbgszi.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2icdvvkmr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uilcmczj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kjflswov.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rvndanfe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpldfzqd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qnemrvwn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2xwsxfuqy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2onslokqw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mqadoaig.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ucbunaaa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2inqlspka.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2oykverhq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rwbqzbpm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2wreuoxce.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kppzpyrt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ddkwqujs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2huqixarf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cperfjzr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rzdmkspr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krqmtvff.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2fhstxzzv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rjlijiaa.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xgxytpms.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vshqlnkr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qcmaqyqo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2fsgkcxtf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gxvsefhz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2xyjfcbbe.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2vutwsgyh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2slfjftth.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2pgimpidk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2glppendn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2abhkinir.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wxjwmypj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jpyblwvo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mqbpkjqm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2nllujodg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2vqsbopcs.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wnxecqoq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hmmumrul.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ykmzajep.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ktvwgnxp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gcpclosf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wplclurv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2tpvabeus.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2aekbzbuk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2hgtqtmch.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2hgckwfuw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ekfezmgn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2dakhjkih.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2tfigjako.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2qdpdymhc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lwetzwkj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2umzchyux.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2eakqkjmh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2emlgeawk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2uctqazvn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2nubnfdtb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2dyorrtwm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2tmcqqwyh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2plzzujtf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2yqzohann.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2sxivxoyv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2mrizzokl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2cvbvfaaz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2frzkatsp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2snayhfrb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bzttqffj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rndmgxsi.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2jwoalspq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2lhfeuwkm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2nzgvnyxy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2upgdquoi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ofnfwlhb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2omsenrkf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ssjdivbl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2banbirtb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yoopvsjr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2cxizjddf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gpdnqhft.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ddkpxivz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2cqrrvums.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yarcfqjj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2cweawtwk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2jrbjxkcy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2euhqimlo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2obpqqrfw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ekvqgnqk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ljfsfbsx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gvajyyas.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ruegmfdh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qpkwltla.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2mvddjdyu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2yibjfplv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2owbadpjp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2mikljlfd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2btcpccdf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2hzwbkjrl.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2gceotupo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qlngnvgi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ceyzdtak.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2nawvqfpz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2gafgxbjc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2tlktjxgx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wdmrpano.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2mrxqpuxi.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2pspqkvrf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2bvfuqokw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2aalsurrc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hjmeowme.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2fhzjvnff.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xpwsevrf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2gcjnwuhw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2opjkpnbp.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bbqgpxgh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2avmtaydk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2nulydmtf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2lutnchnh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2mecjwksd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2cfkklghx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2qwymelkl.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tnplmznk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2avakfrnm.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hlvjkfek.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2szkulmgf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2mosthdmu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2itbdgulb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2eubtciti.html


<!-- 参考信息 -->