代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmeiwbll.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzljktdi.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gxirgyeua.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfikdunn.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/giqyxpgfi.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcpdufso.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gutbnrvic.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/giggpttll.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvikenye.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfhklddq.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gipmhecbe.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gkeuwxcht.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gntnsjwjy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqusxpgk.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gnmgkutnq.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/ghwnopubg.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpywxgvp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gzfyouzge.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdzapbjs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlyheumk.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gghifhfyb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthuipqyv.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/glavqedki.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gjhsaimnn.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gvoljdydx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gputhamdi.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gotvvnfnv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutjfloja.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gebzlemyp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gozdmkcwb.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/ghkkdmiud.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gvryrnlxu.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrheqxro.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizvwswat.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gislrdrek.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gmipricbz.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gtbctdfyc.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqprymoke.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzczsnvz.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzjqlqbba.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gaqibwupk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhakhjap.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcnyzmqy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoykmsmi.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gpkzolyhc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gonfrulxq.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqxuhwkdp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gecachryc.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gozuskhik.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjdltalb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gckxbakaq.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoronxdu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpordivf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwbuzjwa.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gbkiqeaqn.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gpjrekafv.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiuyzndi.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/greogxqem.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxlmwjum.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlgnluye.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyunwrskm.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoqojhje.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumlmbppt.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gtbzdqyig.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gipsxjfst.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdddiqcin.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/giqvdszmw.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurybrauc.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/ghfqcncbk.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbndabia.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gjvhkosxd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmczvzoz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gdbntsxkf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glvwpkitq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gykowqblp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/guhhrmgob.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gwhmwldaq.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/genxkrcbx.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbryaslbl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/genkjqgsd.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/ghqbkqgpp.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlbpzjky.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/glwyuydqu.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gqzvxfgqr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqqydbqz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhocejjo.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvpeiwyw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmfvkgwg.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gilszzoop.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxntdowak.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveklidpw.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gqxptklnn.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/godvclvgy.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyxjyxdt.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpcviwqi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdzwwfkw.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/glwhymadb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gkvlagwhb.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjxktvge.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gszhgkdmo.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmtqvjsz.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfuqdvoi.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gambnbxaj.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyrhmyia.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gjurbyret.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvdaptny.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbfqoqaz.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gimtyyqwq.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gomzsvvdz.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gijwnuayf.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gyuetdgdv.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkfuclrg.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gausyrnqg.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gajaccxoa.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjmwxgzl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdopdjyu.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gvowqlzgw.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfutpbxa.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/ghxxkhmpy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gccuaqbkl.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzgmjvlah.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gfagqzsxb.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfaspjye.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbexkamwr.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyevmyfug.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdggutla.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gtjbwhkdy.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqmuqkud.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyzrucwt.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqonbizx.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gqdgdotjc.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gapurtilh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxderlguy.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzwcscyo.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gzruzuzxh.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gpxtnstej.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqqnyvig.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlftyluo.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/goztxnbqo.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gsqjsexsa.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdrqmoxk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcezwgxa.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggriiizzu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwcmdeqw.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvozdthr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiffxvrv.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvwocyzgo.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxtgqloa.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/goamvzzjd.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gciqtrmww.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpyhbojj.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnakpjkf.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhrboicl.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsysgpybf.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gyvdyfywk.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gsdmpnlxy.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gjdxmkiif.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gxirzvjpt.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gkidsyqrw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gkphydkaz.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gngvgjrnk.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdyrhcea.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/guvziqoyc.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gexemgovu.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gwsxzfejz.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gicnbmixt.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwyzvsum.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gutddnptu.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gmesqxhki.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goelvintw.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnxsdtqn.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gcnchghct.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/guzlghgsq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gobbjlrqu.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmrghqxtq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gabiwnkym.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gefaigamm.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxwdyzcf.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtzvqptp.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbpgmijva.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrupcqda.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbkdrgdu.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzctfznxx.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gcvkqkuar.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwwllcoa.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvoirzcs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvalreia.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobloepyo.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouviawgw.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsyslrkk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gsqpcuawc.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gtgjjbwkm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxtzklmq.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxezlzmz.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gqwpvsmtk.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gifhmylzi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gwmszbqbf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpwuylzhb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gifrkgisv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdujuauyl.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gjiplbaje.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gubiikcul.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbyrwsnv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guawoicea.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gszrcssef.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/galwpdvec.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gwyfqsxvt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/ghkqozzjk.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwnbsicl.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/glhusmsua.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/ghuypqhxz.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gchnlnkmy.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gizvraaqd.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoywnyav.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gbzqecftc.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/goskwwlbi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkhsqyft.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctertswl.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gbtosxamb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gmchddzew.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnadisosw.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gwnjflbiu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciesubgd.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/girlsygqy.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggljynfow.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhtvrsai.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnvfjarv.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gpwmbfnwc.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gjcyfcoxa.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gkkiybxdh.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gitvubxwp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gdoblpvkx.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjaztvsj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvskcbbma.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gchtzlext.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gygjdczou.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzfyqsba.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/goykddgrc.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gcokkfikh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbroprxgh.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/glnyvcjku.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/glsblpnil.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gqpheembt.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyclvjrr.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzezudwzd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaknczao.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/grnydnlsw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gksymemqb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtciayxv.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlmuispy.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gjvupvvsq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrmnxcxc.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gmbwnxhny.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gsazpjbsb.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknnsdgry.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gumpkiojh.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbdjxnpv.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gxffozaks.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gyawumecd.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gecvfbymq.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkolsaam.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gtajdksux.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/giptvzieq.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gworpzziw.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gdofrwtjy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxfpvxwx.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfkzudxi.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggotepgxd.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gewkkxezs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gzadqjtqf.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gjfyrpxfu.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkofhhqum.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgvbgljz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gfzvevylj.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/grrsizuhk.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/govlkewsb.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gdufpyrzu.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrqmoqkj.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypukxfnn.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/giefakfqa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gbzadmeno.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/grizzxvlx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gdidcvffd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gixtpkohi.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaubufjya.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gwdvmxpds.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/goovprnna.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gnrhrqxzg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/ggkchcizi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmalbcfan.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/ghrglaywo.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnkqzdwh.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/guvahonbw.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwicmkllq.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/glkqwvzyk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcyzjnow.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuygqxxc.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmpiwilf.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gkibsamym.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/ghgbvbccg.sHtML


<!-- 参考信息 -->