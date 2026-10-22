代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2fdhqvgqk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2fkykfrje.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jaiqtgkn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2wgqkxqok.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ourbfezo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gsbwejxw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ynrolyse.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2cgjvvcsz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2mfblucft.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ufkisfef.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ahdtjzcg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2hbhubfow.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lyxjjkqo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qkqovtls.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2pfzptbdd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zrpfbnqq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vokktlpw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xaiplfmo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2mwgluvyi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ewumteaw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2owbsfeed.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jbozpayd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2yqwqjssy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ruskfkta.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2pfttpcuf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ysqwmvhc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2oxtlzrfc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsjwporu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2izkudxoo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yvdfnqkh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2nghcvebu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fhmqhion.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2nshcxzac.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2igqvgykh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2aglgykay.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ncvltyaq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2sewbtnnj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2yelrjnbl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2jgbbjwzd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wxabpxha.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2jxozrckl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ocxhodaq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2obxxheba.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qbgihnoe.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2pixrtvwy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2gyvzagfa.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ctdummis.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tngfzhxt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ofgxrkuo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2cqlnszud.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2niwuwkdb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhjvrvtc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rdyrmjjr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfknsdwb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yjxovkyh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2gyapnhdu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wxjmpbpk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hmclmxam.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wqneloct.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2kxcbmocv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kwtdfsmd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mhhffnwz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vmkuutin.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2gswqaphe.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2vasllhiz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2oohshwxm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2vwceyzmj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ppkrpwgt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jqqeuuxk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2bidrdqdu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2fpwjlnxh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2hyniwjlo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2zadpxuoa.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2zczkpaqp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2hzrwjuut.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2akbtgjch.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ovdzhock.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hgowuqhh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2lnbuuxbm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2wgourzwu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2whhjksin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svoknqyg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lecgavzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcachhlh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fkeajvgx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bzhfiagk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lblzpipe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2lstjevmg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ztugxmte.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ljcmlkrl.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2inljonlb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2mwncaxls.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2fldncoku.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2hjovilwz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2iygvgwau.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2iazjqjqs.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2noheemom.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ygyumbxe.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mtiirrbr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cttaytcg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2yhobttxb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2hudqkizk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vgentoik.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2acnwxgrf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2dqhqfmbr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nnzdtzin.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2khmialcc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cagaflny.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ipyjwljr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2rhveuxqb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ieaqnwdw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mammjhdu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2cxmhemqh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2agjkahap.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pkbpgwqt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lryveedn.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2vgdbghax.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2aivrlkkr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xxekiwzy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2tmpshvif.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2kcjhisrd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2hicnsojm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qgxldaot.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dfhjkycn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rxpnkczn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2qzkqqdpb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2yftcxloi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2rwkfqktg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xjqhdjmj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dwixsvbk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hatswqmc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2emptvvuu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2rrmgokxy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2aelqdxcz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2uisqvpgn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2vqbvywrz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2rafkaesl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2aqevyekm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2zrkrwdch.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2jqailerh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cbvjldat.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2oljexkdy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zpxcoiid.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2frzzbzod.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sujicecq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ywiywngn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ysjckvtv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qnacjkgi.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2kfjzxfnd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2guorzupb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2jpuvbwdg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2zlxydslh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2flvdcszm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mwkepjdw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qbmtheae.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rfhtvefi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2achegria.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2qnqxilpw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gyvxgmwl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2owfcaode.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mnqurrya.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vwdvddum.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ibdemrmp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2izkjjywy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wdgqnetm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2smsalzze.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ptlyaymn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vnjbbzpo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jrvgzhuy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nvrxpwvx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2smylsbxh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzqmmhac.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2iwvusxez.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmqgzsyu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2sbiwfraf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vvuvpmgo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2zniedjhn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzemhlrx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lkklyuzv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mhlwoncm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2znxbfcxi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljvyhapu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2genbqojb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2syrxannu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2uluzbqng.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hbqqwwfk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2spjpnjnt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jjcbwwiq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rqxuumdq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ypphgorb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kaxowtuf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ajtjooet.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2qhkebaiy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2optokdco.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zxsjplry.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2zfksmlsh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2olfzslmu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wttuoflb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2iwmgrtry.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qwmadheh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lftmtvna.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nxbgoamn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dobykvne.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2judeyqpd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xnyytmmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxfwkzhr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ptuxjxxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iynixfbq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2apejmyrg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hhkdvpbi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2dqzkmfyk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nmdvzyzv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zfliajln.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2vfufxlie.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2mhvzqcju.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2bhgkkpqf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2nyhptvdw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yzngpocp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2kbqeiigc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2gfamauez.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ndhmanjj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2xodkujca.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2fmfzmevx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2czdlealv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2aoyexlif.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2hwjktgwa.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ctwfzuxz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2zfoqfugo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xqgwxzdn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2zbcebcsb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2arrgnbot.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hqlsejhf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2cbcanzeh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2zxgnnfeo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2apqnrjil.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2oforwidm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2sxwmmkxn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2tmhdyern.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ebhjjpfq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2rsohopyx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lbqltcyf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2teovpcrq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vxzyaplk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ewcukicl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2yyohopzn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2pwrebjvq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ciiuthpa.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2vtveoiyz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2kdyvbvro.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2acuozmum.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2gtuzmctm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2qkkoubxr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2xynoijeb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2cnyrnhlu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2mhdtjkpo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xjtdiavb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2eurimbdb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2vkmwszlq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2aaaughls.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2bqosccez.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rfrkzcfb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2sgswwsda.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2vkzqmlwh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2noixgzyl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ovvchdzf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2wqbsncoa.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2mwyrgicf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2nybmoyjr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ljhuwrim.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zzizgmxo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mmhyptbi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2htqpvjwu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ddzltain.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2avhnimwt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2jilfejay.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2vywplegr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2tatpwsyz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ulyjohpa.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2veibzmui.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2xbtexklb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2tjxkiwje.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2tzxgbztl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2qtevfuda.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2zicopwdw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2tzjkrgjf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qeqkhcpp.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2kasaaueo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nhrmusmc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2dzyxpmih.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2gtgaghgg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2gpwliwjv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xqczmzgk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xusgrrpa.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2lqigkkth.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ktbydfyt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2vryyjngy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ivjqwqsw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rxhopcho.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2tumcbchb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2tgzxyhee.html


<!-- 参考信息 -->