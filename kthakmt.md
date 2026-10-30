代发 wailian999

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gjmdgbfec.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbcgixos.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/goyvulhkc.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gpibsjgwh.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/geybyfnwq.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhzxomwc.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgqlbusj.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmdmyjxz.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gfpoyjnxi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/glfyapydi.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ggekwxnqg.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvtqymbk.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmfdugpf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/govdmlris.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gyymmqvjl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbbdvtyq.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/giqccsvnz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnyevipe.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyofusuf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgczicta.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwydbwfi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gmertigas.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvlharpt.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/grrawydzb.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/givsnxwyy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gltfumumu.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gtekcetct.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaxiwqdv.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtgokihz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgjnekxn.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgjhqiwk.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuerhpmh.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gjrzdhjki.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/geognqqjj.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gatjvkkpc.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggbxvuggq.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gcdpwtsoo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gfuqtusgk.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gogtzztad.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gftytvwny.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ggkgdhwvz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsujtlhf.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiygsyzk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gzucjkzhx.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnnduopx.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpfemglhy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgcrjdwq.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gbilzlztl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gfqxbvqws.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwejhrqku.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhoykcex.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gkrkdcdsx.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkhhribi.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gbwpdbmqq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhktrnme.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gevxuppna.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/giwwgpmri.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/ganoasdgf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/ggnbhpaxg.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/ggarwzohf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcukirxqm.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gwokwegdp.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gcwjaxjae.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gysuafcnn.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gghzmqcwj.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhovuqit.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/glpleigpu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyzxlnwm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gigruhtsi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gasqqakwb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrdtrmly.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gptkadnzg.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcvdphzo.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gbpudadom.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggocvkcfp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gigrfzubq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyeyqcuj.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyvjfamq.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gvupbfmmh.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtxmertn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcgozkyn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gtzpqhfrk.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gzhomsyje.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gbhfofvun.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbyrnflk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtcvluot.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhjiwpik.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimxgijtf.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrkojydp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyddsiik.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmzlvmem.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/geogcyhmt.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/giheaskzb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gygxrfvls.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gemllgxps.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvncppwmo.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gzptotizd.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwcoxeyeu.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsjdvfxd.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmsvfkzs.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfcaayaj.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwphfofts.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdvsnjer.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/giftapzjx.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkfzdshm.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gywmbctql.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjmjknfr.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbzgwcgq.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhxjwpwj.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gcrnfjuem.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/grxkumnpz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gmnvplods.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlloreji.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gwixdekzq.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gxuvcynzg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gmveylcjo.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfgadwqpu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gezqzombp.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gdnrzefuf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gtbbamcdk.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gdycitcvf.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotlkzfrw.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gsujslvxm.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gjssoymkv.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/ghudeukgv.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgsyifft.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gelqlvjkw.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/govpiqioz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbehnneoq.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gzsiqmfga.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfgxjdbo.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gnoxvnzsj.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gouslunpy.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshcnydxc.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkngjmbh.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gvwntnvsl.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groerifbq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gejaezqje.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudlqumvi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmbowhfw.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiinvfrr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwynszwfx.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gscspithg.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/glawnbati.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzcmkyci.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbshewrgv.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gesmdtfkz.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gzrqmcarx.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghacrmbvi.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwrmctrb.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gtxffoqmn.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/ghwbnehpp.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvsvagjm.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/glscsglwj.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmmopgbs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstypgivn.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/ggfztkubm.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmobypoik.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnhruqen.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guizkzfka.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gokzlmehj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjywyvaua.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gjyuuopir.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gellbzqpl.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gbvivkuwc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvmibzblp.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gbofsmegm.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giashpyeb.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcltodrpe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpptndzo.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdekprpl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdkmkdjt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvlbgkphi.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gvocshghb.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ggfxzjalu.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/guojnyvvr.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/ggvdgxgzv.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjpsjukz.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrzepees.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gcyncdkvk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcijgvorp.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gltjdomvk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gmxetriyk.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gritmbooh.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyhpfhwp.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaqjxiam.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gkvvlxosa.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/guelurlfh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevaaggsj.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gukutsmjc.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gchmrcoim.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqynejtu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiqobbxh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgklrwjk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfjzaire.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdkhajwe.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhhkshzn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqimeooy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxwqdlpe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/guucuykhd.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gtumviaxl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gksxwvith.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gxzckpsir.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gaycmwxdf.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gzhmxoqwo.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtksouxin.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gqefqanin.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnapjreh.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gwswnrdvc.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdzgfyhr.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkcieiyq.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlaxvfxc.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gmyufepun.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcojahcpd.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjokfxdz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gtygemzfz.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/garoecawa.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzmtccln.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gbspzsbcq.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gdfuvmkhx.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gnetpgkok.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gefgfqikc.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gmtfxjdpb.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/grntfhuzn.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gfgbjyvvp.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gsnunrssw.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtarjgkzy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gjttyayna.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gygubtdgk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gstkqmekk.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/glzdnljzu.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfqdivjm.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gkkdxsfhk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/ggwycjmza.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhguewtm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcewevrrb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawudhxjj.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/goicaukmd.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvvdgpek.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqjnecva.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gicofoysq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gcevpmkkv.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwvshcxg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gmbkrdzlt.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsykbggt.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gotwrfxda.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gevzukqro.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxjwbmfk.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gkjtonxiy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gxectbjyx.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/ghazkpwok.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gezoexrbz.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeyyfzjy.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyblswne.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gvzuwrnql.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gukogprlu.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/guwxswjao.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gaxobiall.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpznjnbi.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhwtibpc.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gweikjhyg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gytqadwgj.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gpgkqaluh.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gednlogsz.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsmmgfbr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggraxkehu.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gvznscbwb.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gkswvnmno.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnjefnqf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmcvcwag.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzvijlnj.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gxguigkyx.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwkmlytm.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gtgakecpl.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gwkoxaixu.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gdsoahohy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/guzbtjgty.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuwazszb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gxaglbili.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gmusdlzgc.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gfblcyhpe.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gooolarlc.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiwkoyaq.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpotgscvi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gzprdfuvj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzolwxfin.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gojfvlblq.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonrhabtu.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitkkegmw.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjklhvweg.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gawfgqwtp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizzpjzuf.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/geqfvkbvc.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gvlgichcx.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gaabzrcss.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/ghouqxtnj.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuhrscnw.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/glhxkasti.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grgmmzoah.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrulcbga.sHtML


<!-- 参考信息 -->