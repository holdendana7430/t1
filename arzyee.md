代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2lsrjbxfx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ptxurbej.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2gzctmgje.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qlyhvvtb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2moxnudrn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2prgzdlvp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xkwnserm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ojhbgicz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2kwvobmwk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2kjzakvko.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2evjlabzv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2cjizvokp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pemlipgr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2omaunshw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vnptipor.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fumusgeq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2cptxvlqu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2opxamaqc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jrdwsrkl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ytrexkdd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2yuwrdmtl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ifgunxda.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2pvzscpzy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jteebkxe.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2yzrvwplb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ebfcmizv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2piiyajjo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dbzoaice.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2tdgmnlyz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2lnhzahoj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2huulvler.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qtdngkia.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ngwwxync.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2gjkvthxq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ezgneqkk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zfsszawo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cgdeqbyz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jagayfkp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2cjudddvs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2uqnbbqwj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xsxtdasy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pqmykphz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2aqmtvvvd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2splamsbg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pcwgrbym.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2cykdjpma.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2fexdbxlq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bviepmce.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wqjhhwyk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiuqyrrr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnplevim.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ytsbopss.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2nunctiae.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ylqbsdnf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2jxolbisv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2rtbiicut.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fsdhjpvd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dzacfpfx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2gurhjrmb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xbinterd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2lebxuieo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2asrvfvvh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tcvubyqb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2mbhpsdqy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mavuzanq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2sviqfjpt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pltdzqmj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2dheltjrz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2uixzubmv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ydqzhfaa.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2yrxitlcp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ijlvnoit.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sowrciwe.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2oxrjzasm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2bnrvixnb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2qxchkktc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2clmvgdvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijqcnkcl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lfbxojou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgmkbdry.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cyjwngrr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2shxaictx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ujtrvmog.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gesavfuk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2hlzamyzz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pfjxcyrw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2okkgopph.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2tlqlggng.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xkcyzaxl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2bukvicfk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cvafmbdt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2azshdhcr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2abrfczjm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2claavozo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2iuxxaewr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ojzlxrzu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ojgxqxzl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2cveoroil.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ufculqlg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2fysnrlel.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2nviyophq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2yqohikmi.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2dgjdszmk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xdsxajob.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zmzkzogd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rujrllds.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ussnahic.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lgjthloi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2kasyfsow.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nnnscfqz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gvhfxnwy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2djzdmspp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rbxjydoy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tuhblkkx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kxwycbyz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2pjltkmkv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nkbglpdt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2nystohkm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2tlzmvwve.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gzejpurt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rdjpdgah.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2wtwpokca.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2lihfkzlm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ibypgvjx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2swalwqrz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2dqpxgwnu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nimvhpwp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vnbuvbji.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2qklrtaze.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2rasyrnge.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ooboakfj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rxzfghpp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2aekzkzys.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mesavsev.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sjgjrmsn.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2mwqhaedx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2njirranh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2juedudvm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2avhywitl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2wdpvujoq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uhhnlaos.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vbuaztag.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xyhxnbsu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vpbeevfs.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hhaiaasd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2nmsmhyxg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ksibiqub.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ztgcnqzr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2dvoqfnit.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2biyerlty.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vrfzgqor.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ghwbkjsm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2penuoeaw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2tacapukq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2brswfcpr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2uxuwuvul.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lipcnlqh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ozripgig.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2sdtaoajr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2wgtoypby.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cdixgjzp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2arntwlic.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2cfuczxgf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cezwgiro.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2phvlygso.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2bmozvrcr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2etocmglt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvmcqsaf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2edgbjaff.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuufqjqc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2rkpcsaft.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2merhghzk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2uhnxdfkp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnapbiph.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ixztknho.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2nwulqder.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbabhdvp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewdmwvyf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fihtjehg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2giommtsl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpuypist.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rtoidrcm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2palrdopj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2yucnghaq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2waxndgzq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2codewmsc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zxifftwx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2avhiifcz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zddkubiz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tbrlarkm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2beghxlmr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ddtkdhex.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qhsniwwo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fajafvao.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qyfnukpm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2whsbctwu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hlaoqgwl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ikvlolcp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ooxiteij.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2dsmddrhe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2eumyyetp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gacmccxb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xwcvhjco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2haoccfxb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hgpjdllj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2nyjfanlt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2uenujwxf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2haxlhocz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2svadtcca.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2zooqozmn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2xbyslwem.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2amunyrmf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2rmleaasp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2nqvhiwau.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2nrkkicbk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2shbqhnmz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2dzxuwtts.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2dxjwpuhn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2iwqmfwfm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hjwvubvn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2xtiaamds.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2obmgmbgf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2uzeebxzs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ksfcgqde.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wwojbvbh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xtneswla.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2bjnmqaic.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dmjjzxty.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2fsxgthxg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ezxvnemv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2tssnwdga.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2gmvelcna.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2elyonvyy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2uluqtwoh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2worwuswg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2cnxfcvpk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2pzkrxert.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2kqwthhxu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2wvbkjybt.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2thugjzkv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2jqwlycrv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2mkggthmu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2faxhttiu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2iwyjkgmh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2cbwwervo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2lrvkdhxf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2wphkibjx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2nvrfhdff.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2eughiszb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2yzzkqwtq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2doyjeopq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2eyhmyucm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ypndpzmv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2otxhnuog.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ymvokygo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2enuuyvtz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2uimnybbu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2bpgrdnog.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2qyhrldpq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2tgysilix.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2cnpnmcds.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2tjmhlref.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2clovrvht.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qlyorkmw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2qxxscjbm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2vmoytaqf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nlgjzgcn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ojgjvrpm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2gtouwkaw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ormlgxjl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ezhfnpgn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2gsuffgoh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2mzijahza.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2vwbzkktm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jgpzighk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zanqujwp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2kzxdkrbu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2wtyphjax.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2stccuvlw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2olliayyd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2wcsinhxd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2anekcrmj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2gsmvvqmp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xwlysmsu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2impmroor.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2fljyzsnb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2viaksnlk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2brqwenft.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2qxihrsnr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2irdfnene.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ixrjmpqs.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2tnxftppo.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2lslfnmlt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fmignzaj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2otujepna.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2tkpyzpzl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2nbhkhdan.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2iiqhfxza.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wbdfpaom.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zyamtaaq.html


<!-- 参考信息 -->