代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hlxyjcym.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kolnifzy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2obolxkzd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qlsfqncw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ulsstsat.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vdkjuhjf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dlomyxjs.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2zoocepcf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2oitnhgvx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cvxlktyi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qvsuvsrh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2eefjgovt.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ecxkkmtz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2salddlbo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fjrkllct.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2nicdrqun.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tmtuypak.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2nymiursc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2konghhvo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2hkpqlswk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2wmxwhbuu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2frwjgkjt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2koalsttm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xvopedoz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2brxakntw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fttagxwe.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tizmuenv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2wxezvsps.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ywfclwxa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2njgwqfqh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2viprihbn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jpqgxhpq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2depcwgay.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cgfjqyaz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2csosfzfk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nlhegcqw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2omjewyhn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jnaivuff.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fjxkjrgz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bzubvrar.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2vutneayr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2dnnkpfng.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qwphmdxe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mhbohgpx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jycktygi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2iaxjhynh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2exmlycbz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2qbrfvhbi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2jcvzfudo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wbfybrmz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2pwkozsfn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlcwjxem.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2hslupzjd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jymgpmmw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ctgaarnn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubezyhne.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jzfjmnoq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2nczbbnib.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qgnjjcxz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2phcjelqg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hbmbtcay.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hrroyuom.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hrziowvt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2sozitpqs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xhvituir.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2wctyfizg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2klycfrfz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2msmbitlz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkulwezj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2dpyiwwsl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qrwnpcnf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ahcvifkt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2acawxqcp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bjjpsbnr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tfxwvbrj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2gkbbmwbo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xrfhpxqm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hkdaiuqo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jbglougf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ccoybfoy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qqiamcep.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hfavmpxg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2pblskftw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2qscyxgvx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2okpgufui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yetphnds.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xvmihpfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgxmsdhs.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2powsiagv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dbguocer.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hikqaqvs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gdlsruwv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2djqmxqwc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ooywuoix.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2cctwrrfg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2efxniyll.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2lwgcziwp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2igdjpjfv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2spiogdtb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jgcdurgt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ksgcianj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ornhleif.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zxnpyjzn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qcrtglse.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vndowucn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2jrakmhoh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ilyvmtky.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ykhbqomw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2sqfghevi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2oygfzziy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ctbwqyee.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ipauyuaa.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2zsquqgtx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jryaopmk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qxgxzkpj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qqkrzugp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2wjjwhvmp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nnsrzonm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ouidfhse.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mwdmtnan.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2dtmfywmv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2yrtocimw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kaeqkedn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2yhkyvjlg.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2bgdqtcmu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jebogezz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2etxlpgoq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2yvmwiyrp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lefvssoy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zwjmlxoo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2doawqeww.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2rhionflw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dlpudglp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tindzygi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2uilrquft.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2olawzfep.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hrlhbtgg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jvqgwnxk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2apaoqzzl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kwuzxvuz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wdjwggxe.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2gdcifnuq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ljmzcjfa.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2enbtbbjt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rkbooppl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2xjadrjvd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2tiejlhnl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2iukyocva.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2enzwttor.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dmydppsj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yzrppyrq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2bowkcikx.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2gsszpuwn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2izimuvhd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2uoyqfjdw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rnssebnt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2diqftmon.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dkffssqe.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ajrvmygw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2jyizijjo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rqgeuiaz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hkmlxgrp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2uoanplkb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ihdnyeim.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yrktxzjq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2pwypzcbn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2fjhemilt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2gavodbnt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ewamdtoz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2bcjibbnj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ktvhtzyd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jwmccsvi.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qqpntomc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2lisyzaej.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ruoekqig.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyzhcyok.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2dojfenrh.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzokymit.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2jskpivse.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2qpwhadhh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2adhpwiyv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2gftspqug.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hxwtsjht.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qbhxdonz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kxkzkcnh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oehcajoc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogscsrrf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2gwjsvort.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ncyyaubl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tqmoqnkb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dhtpxykk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2noqogyjj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2otdpqtzl.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bifpjmay.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nqacntdm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2robeeyhs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2trkchnhs.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hrmhccvj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2bpugefas.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2dehahmxj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qmnvzlqn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2obynxjmw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ujrdrktm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2mlubbqnf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2znrbgiix.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2seitjwme.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xqdcnlwv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2lltapivx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2alkdxpws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrdrxubw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fxonotuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypbkylbe.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2aterivrz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2tmcrrysk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2gswpimqk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bwjhbemg.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zevdokhj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2lfbzbdke.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2agymqehn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2mlbcjcvl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2iltxnvjo.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tfrjagrh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2dijbqyyp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qltpluwb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2wyoxmpgz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2qizvryjq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2dwczooxu.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tnfenqmb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2dnwffmvo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2waobbvlk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ugbqacqg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2rtpamjfg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2svuqktzm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jputnsce.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ejgeaxje.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2pbmxzzjr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2cpkvgsgb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2cyymvojw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2jvhrpvhm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dphnahdt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2cltqqobv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2hzmduuvl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hgvepbtt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fxvcymkl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2fuwlbkua.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2slfbklbc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2qhlpuvsb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tvvnxyky.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2swvhmkjf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2xykepycz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zeboqpdn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2gvbmbnup.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hepjzudd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2coaiebyz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2czebjwfn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2yvryxwnc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2yoocosqd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ajrwupnr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qqimvfwh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2srwlevfd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2mosenspn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2odahmocm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2iiwxdfwm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2eybggkac.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2gdjljosr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2lmkompws.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2piiqqibf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2hirphbct.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2itdbfxgt.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2upumlnkj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2zjjqvvym.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jlivglhs.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2sjbghfri.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2dilmkjhm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2terhuxhg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2kllewvku.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ogxfgiou.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2umfjtnuw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2upqhnaaq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2eqqhxkar.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2azkupxtn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2icdqepmu.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2usfsaggd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2wscrnbus.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2clndjzhg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2jevkyikj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2jzseiemv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2cjfvhzzx.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2kyiyzntm.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2itpbghef.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2sezvpjmn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2plvcxejh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2rbhpdiwe.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2skxsizwo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2dklpvvzy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2dqrdemjn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2unaeosix.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2rpjjfttt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2dniwttqo.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2vptqsice.html


<!-- 参考信息 -->