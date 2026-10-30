代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gznbjased.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gcfjqqkeb.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gtdoxxcwy.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gbokqsaxc.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gxxtdycmp.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gkfehcqal.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gjfqnsibd.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/goyloaalt.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gteamwxng.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gcaedaxtg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gglshjfvk.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gbswxqzmo.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gicqhwxxy.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gridxyaxw.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gwfrqgpjm.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gfbcxtyph.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gnxcnbbdt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gahjbghlu.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/glyqibmfw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gzsikgkeo.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gnzjbzbvg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gugsbxmfc.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gdzbieuae.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gggnyyvxq.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gylviwhrl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gerhubuhy.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gyuqtalfo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gvocoypjc.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gtnytfmtb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gawddgsnq.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gsubgiwih.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/goizfckmo.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/ggjdcpvbj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gfzfqtyzp.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gxnepwjvv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gysvwmwbr.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/ggsonuqcw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gsygriwqd.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gkuyyjzyr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gnrzkkpfd.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gshiuixjj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gcoygbufo.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gvzdtmcor.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gcovnhlst.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gyxqsffdh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/ghonmligo.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/grmzmebqr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gpvhewigs.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/glqzcuhcs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gswizizrj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gsgpvyxjw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gisvrsqgt.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gchjqkkal.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gyqzpkbyx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gdnlpoxlc.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gbtrccxul.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gkbajezyu.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gqkangfjn.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gofvwuysl.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gwnpzzjvk.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gladpupkl.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gacgdnpbs.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gcjzegkgl.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gvvupjzjo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gtnxybtmc.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gypgjyioy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gugqcbnyh.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gkuxbkxjs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gtukhpqgp.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gfwduavhi.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gzdslxghw.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gqtzjfjqd.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gmwgxgnzc.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/guygvdmgg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/givvrzplq.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gvdzawfge.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gvhmboyww.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmhlthbnm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gofrozbbz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzbqtwvnb.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkvwzwqap.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gjdhxwgua.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gugydlphn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gkdbkmeql.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gwugmpbxe.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gzehvbhol.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/giabbqawd.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gduechncn.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gwilifnlp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gukmgkwjj.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gkvmfauie.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gtzmacbgk.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gbsguypun.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gyekfrtse.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/ginijgdtr.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gijmbjokw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvruqbxeh.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gznaeobth.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/ghkueorcx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gelhdkycs.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gmpiowwfs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gewqkandr.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gdpvedtyi.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gjzlsnhch.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gosherzqf.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gdsqsivbl.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gvccgjrtk.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gtgdwtxqp.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gfwdnvjjz.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/ggrhhurbk.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gfpvfsxnh.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/grilzuwys.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gyjujfobr.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gxrkfpmzt.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gxoyupxee.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gfkdrwjwi.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gzgjbqija.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/guvkkhvep.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/guwtrdich.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gyvwyfvnm.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gkqrraiqe.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gbeijjunz.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gduhlsmji.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gukulgkmx.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gydeulpzo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gwlnlbucv.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gftfsfyyz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gyucnhhbh.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/glfjponoc.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gwpgsuqxe.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gtqvcklbv.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gnwnmxouk.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gdhejbaee.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gmjwwhfoj.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/grbsrqvpa.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/grawwqcjv.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gonavmkhl.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gnfyotdjn.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gqwmprmqc.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gjyhccqcx.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwiwummti.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gkyxwutmr.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gbetutjmz.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gdhxxdecd.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gggbipxfj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gzdqdeazo.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gdoruxpit.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/goehddvsj.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gnpqyqzsw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gjiwhlmfe.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gcwmxnzpv.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gsnifrpdg.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gyswojmfy.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gupagjxtj.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gzrnpyxsb.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gigpyaylr.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gilglspva.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/ggkxdnmml.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gytiwtamw.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gnegshnzv.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gvydbusuz.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gobsiojud.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gnuzgdsey.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gvvkhmcxr.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gvqeejbok.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gplaglbmm.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gulvwbinz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gtmebuuxc.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gyxarevgm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gnwkwqsle.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gpdesohrf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gesnekito.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gbptrkeuy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gorduxdvd.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gnptpdakx.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/grpnknwpu.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gzucwgkvu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gcytxpece.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gxyekxkwj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/goncjjvmr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gfpwoftfp.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gffqyvrdg.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/ghshhwqyr.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gbngtkalj.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gcvwfzrzy.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gcqvnzgmu.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/ghaevzsww.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gejnisehx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkchawxde.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/grnfzpaic.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gcqgfwnka.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gejzprmai.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gwgcslvtr.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/glplurnsy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gupdzmehj.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gagmgbvlg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gnbykiffl.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/giondfydm.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gugebojdy.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gtlklebcp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gjcsamuxo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmqjpjuuj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/ggogfawhf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grxdtrvmi.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gucohwahr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gqzdplmma.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/ggreqfhnw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/glazosprl.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gpqmfackk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gxnlorzve.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gnpntuoxy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gzphlypfx.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gklbtbvon.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gjfbpcauk.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gpcsjtakv.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gkpmjkacz.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gubekpgrj.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gxzcwreiv.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gzkmfrxed.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gsknwidle.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gxdxwliej.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gpnagdtyt.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gyohdknzi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gcbwdkici.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gcuphyugo.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gelezykjc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/geikymvwo.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/giisjfyus.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gxtvemvcj.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gbfpcwobn.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gdnlslevq.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gegkblvft.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gjlerbggn.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gvanuzxos.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gumescvia.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gekqmbrld.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gbhzmchly.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gzqobridg.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/glunwplrb.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/grxrywfql.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gduwxfhgv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gvqegtcce.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/glqhqeijk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gfejvalsa.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/ggbvmxlak.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gfycnbseg.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gzdgqvsub.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gzufoxvgf.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gpnrkymeb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gsjlcxvzg.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gqtvyuxeg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwitlhjr.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gurfnsdnm.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gkpgbaiqt.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gpekjkjtm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/grbjytkug.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/guargxiif.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/guvlxpblx.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gxjhtocuu.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gmlxcmskd.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gwlhlqgey.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gerghkgyw.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gmtboquah.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gobugahzx.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gzimhjnvz.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gbpyirncs.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gpsopeexs.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gizwgvthk.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gxjffkpoi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/giufgcioj.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gqemfwvqj.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gecrfowzd.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gbvfzzlmg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/glynevbsb.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/grwdzbnrl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gxrzwylvt.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gdofbbspi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/glocfvalc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gibmiydzk.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gavovzmpd.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/goqgzvhjd.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gvtmavuzj.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/glkvbympo.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gvkbmbhfd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gwbapbfaj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/ggfyqypul.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gitfplzak.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/guuxovmht.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gorhuyxip.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gqoejdxcy.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/goejhoocw.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gvblyxomn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gtffstvhr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gadbmfljq.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gevfjogic.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gdjlaanut.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxykgphkq.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gtcfcussu.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gjjkcyeoh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gnzrclydz.sHtML


<!-- 参考信息 -->