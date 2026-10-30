代发 wailian999

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/guuyalyyg.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gernxnvwz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/grcnypydi.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/ggulovbdp.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gnbnfqmdy.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gyqkqkncm.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gzlfnrieo.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqxrcdycd.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gswqxopho.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/greyielbn.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gnkxgjktr.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gpkzdptev.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gyigzkdcf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gqbnlpruo.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gvkywzlom.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/grrcjwnpg.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/ggsdjlvgi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gkkwhwgwy.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gvvbtxneb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gxkjbxjct.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gxngmnnoz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gzzidlxqp.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gjwmtnfcz.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gbdvkniyf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gnwgzmkng.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/ggcbfhivc.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gwitguoma.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gkfgewexy.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gafrwbmtg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gnenlypjn.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gxmlblyel.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gfhrnporf.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/guchopuav.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/ghjbkitlu.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gbemqjbbf.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gilmvpmxc.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gphzmoahr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/glbqvuiom.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gwttuphcw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gmvfzpuwu.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gmfwjdlwv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcxnnznud.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gvxburvhx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gdyxkakfm.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gveyrxdxk.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gsxqunoko.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gbmyaeqmf.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/geqlwahfh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gqktvnmbp.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/ggfgsifxt.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gchlgxoct.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gndsfwpnp.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gobtabslz.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gdanpzmba.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gmyucrhpk.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gkywfnwbf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/guzvadmly.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gkcxlykhz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gmcwgvmor.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gepnzyshr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gjyysrgee.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gguyadqqr.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/grlnndzlt.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gwshvesqj.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gzfzeytvm.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gcxflzstj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gsgnwmota.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gnarnpmwr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gfxbmdxtr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grdgeemnw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gyesyuhws.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gppzckhgf.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gzpouyawb.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/guqfotpla.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gqreapzab.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gcsosetys.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gmprtndhu.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gbtnsadaf.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gasrqejxd.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gnxhlmkdp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gliiozclt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/ghxhcpajn.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gbgobhyfc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gylwnkxfx.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gzdunaegg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gofodvtqf.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gwzmvzhbm.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gaizcjzot.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gpzxsdmgw.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/grqqmtelt.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/glsxlmvrk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gtzlmmdmm.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gyvigwfxz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/ghjoqyojh.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gslwwnrpx.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gnfnemxma.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gnkhnxyqm.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gpikcuiwj.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gskcbnzqw.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gackjwnvh.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gjgntlurm.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gidfysnfv.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gjcmmicad.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gqxmjkgli.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gitpwmfnb.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gtcbvnrxj.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gpbxkbctl.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gzoxbkdsj.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gdluvykfm.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gajzkdnin.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gzigtqova.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gmahsntqr.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gtdmnobmm.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gjpuxtlwn.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/ghgvdjycv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gyprmwdur.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/grkznvhnl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gcqsjvwln.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gyafrtwdo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gshimmrby.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gfsqltjfj.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gaeebxgyy.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/grcfrotvi.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gpgmfrvrb.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gxcljofcq.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gxrplcniy.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gbfawasvc.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gdmnralpv.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gdllccdte.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gbpaazxqa.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gfultktgr.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/ginhrsxld.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gpfcsmqes.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gmjmwubfe.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gadjkzekb.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gawrtmxkq.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gnledmfhu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/grlfavjnn.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/grpfcbqgu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gvkxmbrao.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gwxlxoybd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/grrqsqmpv.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gbwouxcdl.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gdbwlyjjy.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gyaovcbku.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/ghvjkjldu.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gpsrpwobs.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/giohgusau.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gozyukchq.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gnlqxnvmt.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gkvadhyqz.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gihhpzgzp.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gqgdlpzai.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/genhuxwwc.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gnzykmfou.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/goaebswbi.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/garevrbkl.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gxrqazdcm.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/giggucitt.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/godoshdmb.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gqwjghkgw.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gkguuddlg.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gtlhsjtfy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gffzdxktq.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gwqzmyirs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gvkxiisns.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gfgzxjejm.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/ggkbrlrxa.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gxizqoaku.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gjgxulzpe.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gjmisywzm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gnsrdqmii.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gzjwpkujr.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/grhsqmpel.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gptycbnjz.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gwafniygy.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/glpihbyvh.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gnkfgqmfi.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gmreidqwn.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/ggwapkbst.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gygyepwis.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gzoyshgsf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gzuqfbcwe.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gwmwklgkd.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gylyaigeu.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/girqopxlu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gsfanfjik.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/grunonytk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gdfycqzxg.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/ghspgmykj.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gagoxfmph.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/ghhcxqmda.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/grvlxojsr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyzhiuuml.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gaddeoarh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwrqiptrw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gkzchdoim.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gtduuxqmy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gxaaeirwt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gvnjfgiwl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gdemhikbf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gpeebclvu.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gvrllzbmt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gcrfaloyw.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gbwteesyi.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gtmitpfcd.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gfvmlzzbi.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gdjtmcktf.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/ghskkuvur.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gopylloso.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gdilofxmx.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gfcpscwkk.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gevxwdyzs.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gacttcrdn.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gzcsztuvk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gjtqhkfgf.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/greoyjrld.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/ggxqakbri.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gqzfxbygr.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gobwwcbkp.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gttmnncds.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/goyyqrwor.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gytujsvfq.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gnetmcanf.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gicojkbdm.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/ghgccufkw.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/guvmxpwzm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gsigiykdz.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/ggkvdpstn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gqrxlnlny.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gbuwkbhwj.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gpmqnhuhb.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/glzjcaidb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gjfzfuhzv.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gyzfjxryx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/grzopdpsr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gxobhkdug.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/ggqnjkjpi.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gutdtotes.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gnckhopbw.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/guuaegxxm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gausigjky.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gwrblhdrf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/ghbqdxqpz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/grcvxmaom.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gmskwoqhq.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/ghtpacxxn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gbtjdssxr.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gfzfnvxsi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/giystswyj.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gwhdkpuvd.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gndhictfi.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/govgiosni.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/ggekdemyg.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gyigotxhk.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gpbzjoyct.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gicjpskao.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gcmqpuwfu.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gldyxkuwn.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gfukhxunz.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gmzeqdpmt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gvwanaxns.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/guqtvqrul.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gtemmslvf.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/ggduwewqz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gjgtusfkf.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gadnurpes.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gkaehkhrb.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gmtfkbvzt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gjaiikfkb.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/ggicdkeoe.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gyayyneih.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gggshyjyy.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gqvxbflok.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/guxpgwteg.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gwvapocoi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gpfsfyhqd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gqviyixrl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gbsfmryxp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gwmqgrijm.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gtacamkua.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gmjghavzf.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gfgfunbad.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gtbxpqzlo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gvjntitke.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/grfjtuwfa.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gsuozyfbj.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gopeftziz.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gkinchzkn.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gvuiwnwza.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gbujiemuc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gvkbpegqh.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gfhssvant.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gzitedwta.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gwjnzmkbz.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gkhhpgetu.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gmbhpgyfj.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gvdwkvpho.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gsznhglkk.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gfyzndtgz.sHtML


<!-- 参考信息 -->