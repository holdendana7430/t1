代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobtqfzxq.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfdqvpch.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gryvoogbr.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gnankufyr.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gtlycwxkj.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmyafaxm.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdwqooma.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gyxclkhnf.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gsqpzgief.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gsmpmsljx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrgimqkz.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gilqobebx.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gttkmypek.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnenkufg.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gguophuzc.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gddkaowzb.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/ggroxkwra.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvovubjrt.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghodfyzdo.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gxahxmtws.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gbthcysjk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmihilmqr.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqivsxre.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubpnujvk.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkuasatr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/goeutogtk.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrgiwaov.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtfpcgmi.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/guaydatke.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gcbjxxqcg.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpqnerer.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrstoujt.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbvwjyma.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsplfstl.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gimwrabiv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefdmfyxc.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxxqwaqt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsxnxobl.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzhkaodbt.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gwstcyerd.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmluuwwp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpkvgbuk.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gzphioxpy.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbxjpaqir.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgzmpeml.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/ghehkzpwj.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasmruydn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/glegowkfm.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gqixeksty.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpyatrmpc.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisnkvvxz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkwtshxd.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgytjkjb.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxxhdokm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gqncjubor.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnymqnzp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/ggetcrmbm.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gtwvywwct.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gmtibdvkv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsagucaeb.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiioxvcq.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyddcaktm.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gzlteccls.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxcdfuhi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gchgvrhgs.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gpfqrzyla.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdivmlrrs.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiatmirx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/griwcpozq.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/ghuwlibut.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrdlzbjv.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/grifyeijr.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gddktlmca.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshyqwptq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gftdarimx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/ghshuwyax.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjyvjfah.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqklctbmp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/giaxbqzym.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gaamtdbjr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfabbsqtr.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gmcswrcaa.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gryddkgwx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gntxowflj.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gsvhchrpp.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gmifsimam.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbtxrwsl.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gqvxawdng.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gumrcbtph.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwtllobx.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gbaywreww.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjherjdlq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxtpsqtn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gccdmhrvp.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgtuoutq.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzraupvcu.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/girhyitzo.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gbjozuqxx.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhkdreru.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthggjmre.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfatqjig.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/ghpqmfwod.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gfznptzey.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gregrmztm.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/guezeatla.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzxtvfvd.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gfespiwte.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwcpwrrw.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gxnsayhpb.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtmjzycs.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxihixfo.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcukxiqn.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gfgrmuqie.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gryxrbxhg.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gpxvluedm.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbvitkwp.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gdancuzkr.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqbvuczj.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/guoanoopy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gowhlkpej.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gzlpjzjaq.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcgethln.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gserlshbl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmfvolej.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogmscuow.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gahyvmspl.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gdjsqbzti.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafvbnetv.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gcscxrqin.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gskaahism.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gbepxeojz.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghewuevzv.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxtobrcw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gmillrgeo.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gsevvgqim.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/grhbqpyao.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnbkkhek.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopjnlwqv.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrmyimyn.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gohihfczy.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhzvuipp.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gqbuwktdv.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gfxdvrqdr.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/glyjcovwg.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnsnazrc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gqepucfnt.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/guufzmsmh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gkojqffhe.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gingqtotp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwlxvvgy.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqfarvfvz.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpifigxv.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gbqgdydnu.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gltbhbcxv.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/grdzfpxxp.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gtkuldorr.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkhvuylk.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gtrtfmrlr.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhwqlewk.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohtylxsx.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkyylcah.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gwsyhwlzd.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gdhaobhrx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsxnrsvg.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gfxmlkfpo.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gxxyajkng.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuansqbh.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goqxedipl.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdbqxgcm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhdyvyyt.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gbvppdyly.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbkbfrrq.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gortjrdhh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbkfidke.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmynicje.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhnvudtr.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/grpkopqxv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfrjdjakl.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/giwsqxamw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gciudmvdx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvgtuqmqy.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlvbesza.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gitjormou.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwmtdivl.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gounmioiv.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphngqazt.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/ghdnbafkw.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuiovfil.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrestmny.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gvgggvxuy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwutmlwxp.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gobrvpqgi.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvphfupa.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gdpchcjce.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gzpixqwhr.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gdobkfhva.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gpacwgbmm.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gabsjfxdx.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gxdsqjceb.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbxlxmcr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gdeuobhfm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqkrockwe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmpcxcty.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grojeziux.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxmfdlvd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehedngvx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gkweorrtp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzftiuwql.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gyvcsayot.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gqqycgzdb.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gdsxuhbzk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gotjsjgfi.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gvhweyhxl.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gjmowvupz.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gcnfkgssp.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpawlgoct.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhifcjrh.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gcysngnzf.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejeqlpml.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gtsvqvkkx.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/guuxqhdxi.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimkwirvs.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gbqagagdj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxgstxbh.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtwrsgen.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gmphljtsl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gcovvtihh.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcesulyte.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gepswrvlt.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/ganwwwbhy.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gyrgsbstj.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvscmywb.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gazvonzht.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gtprsvspq.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamjmmxag.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gerzhcugc.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuwjzlhe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/glrsjqlxq.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gbahsmech.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuyhqeyu.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxmukvmx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gbldwwssh.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfdhdsvf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtsmbnpg.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gnfdjjxea.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/ghdgpccjt.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtdmxdqe.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gipzxwqwd.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblawrayh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoflykyp.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gfzybvmbg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gfhlyfxmu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjtylvoa.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyiypbyj.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjbwawwp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gxugtzgpd.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcxyvxyz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcxpqnyz.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiutktrh.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/geovrfdjb.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gzhbtytlb.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gqdohcelc.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gugkvpjlr.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gnsmqwcny.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtsqydhv.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgaxbtoh.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gjocdwjhw.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyafdjccn.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqvfbckw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjctzmmid.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gftpkhfoh.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gllfuoqsn.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gyatvwixk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gmeupucxs.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/grtamfocf.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gzxokmakg.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvojdpjpa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gztlctcyt.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmpazqai.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/gqftuqvje.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/getjxinhx.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gixgnneys.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnisxewe.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkqwyvjd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqlowptf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqocifav.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gzobrvslg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlrdessk.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/ggqyeisli.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/ghowrnzly.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gyjtubfcy.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfglikxmo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcyzhjnz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssoafeoj.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrcsteau.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gubszkefx.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfqcgccz.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gzokgzboq.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxvbameq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhgdbjwq.sHtML


<!-- 参考信息 -->