代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxraafwu.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gjoudhtwh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqyudyxb.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gijvncdag.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/ggsvryenh.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgdlucur.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gwlnefvju.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/genwiczkv.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvekdmrr.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfcrauck.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gszlyhnlp.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gferitkyz.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gufjrqcvl.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gafmdmcze.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocqgidmy.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/guqrcueme.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/glpqmxcyy.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/grquspxmn.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gffzixzec.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/geqvxfgwj.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwiklpwd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gammptxri.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gezsdsaef.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopipaqbs.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gzeezjjin.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gxkkwohxi.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gqikfergi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcqfgqqzc.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gigacfuzz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gscwuhtan.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzoudivj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpfyyrzf.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezdfconj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gkmidrbhp.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/glmocujsl.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gmqncygxv.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxcjraiq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrcqeept.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/glyktayeg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gwvtcieqn.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdqewmow.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrvvjgzu.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzmrtqxji.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsmczanb.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoypurvg.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfuyrdzk.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gvsmcevvx.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqoidhta.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/geyecumta.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gyinvhmay.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloxazftd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmooiqff.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/golktckqr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghyyswqbj.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/geudixuhf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkufeaeg.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypshgmgj.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggamcveyy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsijjzxl.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzdbauww.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbachpetx.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpusdcoy.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbyiunbg.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjwjpxjm.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtlbsdxe.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnetfeucy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpfqqole.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/glxqxlfvl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gueykslbb.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjmpjihv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gacxknwew.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzhdcozg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/grgnmagpu.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gopyglpke.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gotfvngfk.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkgjlqdy.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gfjgjanmh.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/ghznstseb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/guxrdfyee.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gdynetera.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gmimyrkoh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsmmuuuon.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggubyesld.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgsxnywj.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmammlbcc.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gasqvdmlo.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpasluas.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gymzphwsm.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gquawcjmh.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoarkwjg.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpvvkoay.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gfmxyigur.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/goeyxqwcf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gpjacehgd.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gyxwcpreq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrjjfpuc.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gygabhpbj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwljcbdx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gzopxeubw.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeipnctz.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gurknatof.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/ggtlumyiz.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gadwvkmom.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gphszozzp.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuhiruow.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gbqyzgjjm.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gnfozfxpf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdhlaizj.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gtqccykuu.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjupwyzhw.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/grlwyonll.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gwbeezmxt.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfbrkdwi.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gcopgdktv.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcbktbtd.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjswoolj.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwglazki.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklrzyjwl.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gnavduakg.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakwytmtk.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgkqncwp.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzclzbfza.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gncgxnjka.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gfzvcunal.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaowjmev.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqjhqvew.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgpneusu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gbfuoshap.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/goeircakr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gznpnxnwv.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizlxdjtk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzlyfplq.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/ghazhpdbd.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyspljsc.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkvaankr.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gltfzdpbo.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gqslolmsa.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gyuqfwcqk.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gxdrejkwv.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgctdkqb.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gfcwejknn.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghxvqkhh.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gmlmdljhc.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gebpiyotn.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/glccnrksj.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyjhwfje.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzuarbpx.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjclpjus.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfrzglgs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbkqpbfs.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/ghepwjjcm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gvitjxcth.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjwwrtoo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gdhvnclrx.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmclzecmr.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlhvdjcr.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gxygfnrlw.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnjgsctm.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/grzwevvnu.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gqwcpchco.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/ghzxaadxt.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gsrxddiwc.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwizqkcka.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gnhvungxo.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glwmqntdz.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadswjmha.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gcbmymhxt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/geezfdgcm.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/galnrocgm.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gjenrhlkc.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqszulvut.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcoyssksz.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gasfwzxtu.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gblihwuwb.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gluezpntk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gipouneed.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gikhkfgig.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gspqfcrou.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpvvqvle.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guotbpjqb.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxwoprjf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsczhishm.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjlufjdj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gztermyps.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozzqrozi.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gltohqdir.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gojjbcwyy.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/glozpvhwm.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gopxwnljx.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtstzmwrs.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdjxukat.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gnusxucky.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/glilgskpp.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/glwhfvcnv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gwzfvqbhm.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrxvkmmx.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gybxibgzt.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gvyizulkj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmrfnyas.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gwjupyeoo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/geihcmsug.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcbrhuzz.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gkrrzcxyv.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/glstkvvlo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpsqszvj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnkoecikt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gbwquaius.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuxgmjvg.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gtffcxqjx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjhyqbqs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/glwahqvmd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtdokznst.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkfwyesc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gughbjtgp.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnkrvsag.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/grrutivas.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrkhbohc.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gmybwdare.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjjpavhd.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgwwipfz.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdjuencz.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkoryfek.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwbsukaf.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/giywlomws.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gupnsgzop.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gdirgbqzk.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbgbodrq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksjtxmmy.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gjvfpfucl.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpczizegh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gsfbbames.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdvkoixt.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/ghdltsoky.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gymvivsos.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/guqvwderq.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjhdtrxl.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gdmwkwkqk.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gtpihcjcp.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gimgzanie.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzumcxult.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gjmwescaz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnvupuaz.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjzrdesx.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/ghygrwnhc.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/ghvndsqca.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gqdqulnwz.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/goubrqgxa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/ggettkntk.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyucianiy.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gstklzrhw.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/garpowkzf.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyopvjeuc.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfsxzhyt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gbhjfyedu.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijkazoex.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gklldojoh.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/giharxoui.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gookhsvki.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/grntiexvx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/giwliucre.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwojisxw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiqswtys.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/grtuusbxn.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gpoiaoars.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqyevtfo.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gwanqrrxn.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsszhngk.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknpalbuy.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipxzkelx.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqcdwkqv.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/glrsmqhxe.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gsdaxlecx.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gwkhlfona.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/giiurgwmh.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfujvsps.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gmqfplkxm.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gockntibm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gulqzpelo.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrnclbvl.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gadtqyrei.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkhocprz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/grhkvwtzn.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfddcglw.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtstaaxpq.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gbbytpaew.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjawoykn.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gynqmepra.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzwjmbjd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gafcnjlhn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gcgswnbsf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gppngdocq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyalodst.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gejuggrkm.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfxtpzeu.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grurwsetb.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/ggalvkkir.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gieztpubx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpimxgyrl.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnuoqiqd.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuufaimt.sHtML


<!-- 参考信息 -->