代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gsypqnsfp.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gryjcwdpo.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gtjsgfeaj.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gxvnduugz.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gcwlnagmu.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/glnvavufl.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gctzhyxke.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gesktplxt.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gcvnrrxup.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gtqvxikys.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gflihbyux.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gkudbdhrm.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gexrljldp.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gbbdzbzek.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gumxkflbh.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gemjnckxy.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gvwpfeybn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gsvwwkbum.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gkmwqjmoe.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gjdhncukk.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/ghxbpbmkl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/glwgqkpcx.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gnocoagsc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gvkdktynz.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gzuvuazzb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gelsuegtn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/glfgmiagd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gsspnyhka.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/glqafpsqm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/ghsfqpxrr.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gfglxrazi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gbnqzvvjt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gvghwcotd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gwgrpzsib.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gvgahcjug.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gocwxfupb.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/grwdztmvh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gtgdiqshp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfyryvcwf.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gjjqirbct.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gwknkihin.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gxrjcwzgy.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/geewbixcl.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/geusjdnzn.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gkbgzxghy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gveyohuzw.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/ghxbsaovl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gljgfoznn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gobyhixcf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/griaftwpa.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gieqvryuu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/grvitozhv.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gimgzuadm.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gmmuveszp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gbpsmvwkc.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gzovolctn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ghapztadr.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gomsduecm.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gwdnqdrul.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/grcwgdblx.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/geftjumsy.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gngooqywr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gaafqmhlu.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gnzrpbuyv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gsqcfcddi.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/geyxyjvbb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gjkmmhtwf.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/glzqrmecs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gffvroksa.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gklwncvrz.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gqlnrqsxz.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gpmfdfaro.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/ggxsxfyzm.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gksxuynjt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gcwnodsla.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/grxsanwnb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gtcbxpiwc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjumymwzi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/ghgvadesv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcawmoapr.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gmjmflyxf.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gzzgwmuzn.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gjilxfxel.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gfmrfdxpi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gnuvfrlgr.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gqdzfoads.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gvnqsrews.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gsunbkbab.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gxwmgetjh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gklxcdzym.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gwpndrrgt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gvnstvhcy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gmxmxeppn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gyusbipdj.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/ggayuhabn.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gxrhudkbk.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gbgvaqecq.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gkxganqnl.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gdnqzvpgw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gczeddlnu.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gytgrbioe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gbujntgge.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gkadrkzaj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gieroiarp.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/glrwmvnfe.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gexorbbnh.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gcwpjiyvw.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gwwtpyjic.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gyyvzpqfk.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gisafrxun.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/giuhtkejc.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/glyzzwthe.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gszjkdnpw.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gdnwcqfqk.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gznqgmmsa.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gsmqloayd.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gwezjgbgf.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gkgqmmsgu.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/ghbqgvmzo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gedxvqiwo.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/glupnsnyu.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gqufgrdey.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/globcsilw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gavwfgpnz.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/grteecgyo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gizgumzwf.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gdqqjpazz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gddgdtzol.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/ggiorvdjj.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gnatvhleb.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gjsqvmdxo.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gzcdlkzjt.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gvqaiptxe.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gyofbsyjj.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gfluoibvq.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/grogbfsqu.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gjiouvbnf.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/goyexiguy.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gmbgcrwsc.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gnriyvitj.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gvokbtzim.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/getsmwxjx.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gygoapwjd.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/glipxymle.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gikxctfhn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gvfvozyxm.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gxjmjycef.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gnpkqmlja.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gppxgjzns.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gllqwywjm.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gkatsmwle.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gumktrcny.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gdxfusegm.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gggweemgo.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gckbsamcw.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gppcnwykn.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gkinbxzcw.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gjsibkbnv.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/geiaietku.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gurriiyem.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gwdqvuyhu.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/ggytlgxkz.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gfsualrbk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gvkyspwfi.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gupjewpvh.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gfwdcpdzp.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gxorjzduo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfnpedezr.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gzajmnyrg.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gotjnlzzs.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gjulukupq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gfshbudse.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gbhaymvrh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/grdunfqrd.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gsfmaqyls.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gxsclpqbl.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gqfqmaqkt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gokznlavt.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/guzxlsusp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gsydksyux.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gnhbifuli.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gkitgtziu.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/govqmgsdh.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gaifpacbw.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gkqncwagd.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gjwwdszeo.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gxhjthjzp.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/grvbtptbl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gbodfxgsw.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gghcuviph.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gngzvchxk.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gzmkfihsf.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/ghdnahghx.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gszeljrlw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gsxuqaspz.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gegamdxdz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gsokmosfs.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gjrkstbad.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gdeoifyqw.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gblovzyvz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gzhtuifbg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaxqxoanc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gdynnxerh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gegxhspdj.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gamxdycmg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gfvgqbclj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gypkoygqx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gaeqhqctd.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gxeqfogor.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gfhttjlwo.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/goupuuxqg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gyzqcoshc.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gerfxepty.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gcvyoeixb.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/ghlisojel.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gsnysvjom.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gutsztjtq.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gmvhqfirh.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/ggnwmtnaa.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gklsqynto.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/ghreytrkp.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gdzstfvdc.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/grmmcuhbx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/goohoopst.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gydxhjjqu.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gfpewnpmb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gokiyvcfj.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gwubmhmca.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/ggvrryjhp.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gfmyumdgk.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gubdgnaji.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gtwawivsu.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gtghpvlcy.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gtcyidcpe.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gdkmzoyqt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gzfstowmm.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gkvivgpfk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gnxmodhqh.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gljwqszao.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gzrcjqfuc.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gjkjkfute.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gxybjvnbq.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gxiaeedtt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gkmltkddp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gwawyvecl.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/gcugmkjvy.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/ghoyyrbsn.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gijiruohb.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/guvjdiorr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gpepbvhqp.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gesyvitqp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gtlszstig.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gfxmbeejg.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gsqzdmzul.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gnwdtdgth.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gwihmwehv.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/glfuhgvxo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gtebqtbjr.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/grvfkfwqj.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gccjpwgnt.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/guhtikcrh.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/ghezmaxnr.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gpnzasidj.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gngvrejld.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gppeyyxvs.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gmmvcytmp.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gyetwzqeo.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gefuooksr.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gqogwiihz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gvcnkhfqc.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gnfzbhouc.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gvrxwbtdt.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gxrgupvfu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/golkmbpgo.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/ggwbfasdj.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gszibcblm.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gqxvtefvb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gyubmqutv.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gpbmetkbk.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/grqdrtela.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gaamtmrsg.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gvhdktuih.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gmdzvemdl.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gkbjfuexy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gcvilrasl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gtypepcqc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gszwcjbdl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/ghnsbedqx.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gcszpnyxt.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gqjusvcrz.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/glpsbqctv.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gvnxqfysh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gdoyznrls.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gucobsrms.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/garxvjfxz.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gproiwsoa.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gzjwpeocj.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gizktzezc.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gazfzscyf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gasftvjmv.sHtML


<!-- 参考信息 -->