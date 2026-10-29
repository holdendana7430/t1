代发 wailian999

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gpbjcpwnt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gipskpnuu.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gpqdpdqes.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gbsojktwz.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gxbkkwyga.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gidctlocx.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gfryvyrzv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gsfrtbwuo.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gvqybubaw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gddhznznj.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gujqpqhql.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gietzqimo.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/ghpziscyj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gfheblhlo.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/ggzeqcovd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gaoeahvvy.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gppbjphqf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gmvskhyhz.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gdyprgkfp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gxonwhxfk.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gwwbbiwuo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gczbwrcik.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/geviuawhi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/grskkcpnl.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/ghfbvlaqa.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/guhqpcjcq.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gikuukzzf.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gkpikjaoc.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/ghznveplh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gonfmugvg.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gqfsgfsbd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/ggyezbbqj.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gbdivptkf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gbcfohfvj.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gqxaxhkfn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gmzafkdbe.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/goybfgfhn.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gsamxpqtv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/giucbyxne.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gyzobleea.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gkexuglml.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/giybeqhqq.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gmvzxcqwn.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gfbrfhech.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gwxldqcay.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gehmnylgu.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gdtmlyusg.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gevnzgywo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gmfmhxknk.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gzxzipoco.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gflzhtdvt.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gwwixkwlf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gyymyktxt.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/ghnuogirg.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gplwtmohl.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gccsiwnvm.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gngskhloh.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/glqqctqkz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gnvwbngnp.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/glwkxuapu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gcepdzcoe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbrosxgwp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gaavsvcuy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/geqkpjivp.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gyxsudgdr.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gdyzukavc.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gjvynfytl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gkluejdhf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gydqtgbjk.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gggccmpsd.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gxcfpmtze.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gmmdbfeiz.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/glezetoqn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gsuzwzpoe.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gtgigjrts.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gsnkxbdqy.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gtcxdjcsi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gvpjjaazk.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gjuknihpd.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gtjxicvmr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gjhqzareu.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/ganrgnbbv.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gpankubww.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gbqubbtbk.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gmmbpqpiw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gkylxccqh.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gvtrwejgy.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/glpkkamrs.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gylvezgsw.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gaqfovvxl.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/guakpiicp.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/ggiunxgws.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gwblrcirg.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzcvqpgb.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gyfhubjhm.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gzmoebhxn.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gywbjlznu.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gsvbsqrqh.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gjvayycdf.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gryqbvtny.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gvhvdksma.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gvcjbwgmb.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/ggtlzpryp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/garyipjui.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gnybmkybx.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gggrtggco.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/ggddgegze.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gwckzyktf.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gqmdodvkw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gtrzefopk.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gmipxnmed.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gosugyqne.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gmqwmnpjv.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gxvscpqio.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/goxyxjvwy.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gtymgtetn.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gtjnzeiwn.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gpyavucqg.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gndawrwos.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gdfstbgbm.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gtnxasltw.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/glentmjxu.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gsxaubksb.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gtqbwtduy.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gehaknfil.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gkaefulxj.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gfxjowwcn.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gbqyuiukx.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gbcwbufof.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gyptxuoxc.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/grfpusbxy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gwvwodsik.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gbnqxskff.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gdvhivynb.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gclgfofra.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gpgdiqgsd.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gigtniyar.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gfihnhaxs.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/greahgreu.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gehyjptaz.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/ghvhwrbat.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gtvmfanin.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/ggtukjbki.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gfkndxhsl.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcvqjwsew.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gmuwxhzsi.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/grjdvxfkf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gpacvyxja.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/glsvbheqj.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gwkbkaoch.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gdqakoluz.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gjgghdxrq.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/ghxgfaizl.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gzvkboyij.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gpbtykyxm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gdfotncwd.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gzznygoqt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gzfozmmnl.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gijgqmrcy.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gteyidlqy.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gdldwwuzs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gchmyloav.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gcwandgqx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gnbrsqlnn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gjhxpcrcr.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/guyhttman.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gxnupnijb.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gjefvakea.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/geyurdstg.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ggdffngfc.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/ghwtonrim.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/ggfmjlzkl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/grusdotda.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gowmyzydp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gyryczoll.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gsozdwmwi.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gidslpbta.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gkhepdhmo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/glaaphclh.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gqtfvlfjv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gfgquonde.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gbixqvexh.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gprugpbmk.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gghycguxh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gzkipwatg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gubioiofd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gihdefciz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnrrrfmgb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gmmjizwvr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gdnyjtixx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gdocqxofi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/golggomvh.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gwjsfviiq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gjfbxxzya.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gmjmefhjy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gizlogfml.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gmcuduqmn.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/grwtxeojp.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gngxoniuc.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/grnaovrih.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gdwuzfxoq.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gbbemaktb.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gxufmiqpr.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gambqpojp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gwvwkkefz.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gymzaghvf.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gugooqrko.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gbapbomhq.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gyhjdgqbu.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/ggsmuoyng.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gbtyaaymt.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/ghlewclgd.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/guqqdsqtn.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/glnaioqdi.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gioqbcayq.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gnoqfkqys.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gztfgprhe.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gwtsmtipl.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/giawosujk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gkeksbvwj.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gktzekusw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/grugasaps.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gbzofvdze.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gtavpcddl.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/ggsntzwpd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/glljfwxya.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gzrczjket.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gobabckrb.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gfazvbavy.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/ghptpjlie.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/ggxurbhjc.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/goewptxsm.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gajrwbqsq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gonnuzkys.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gmolailem.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gdhughgov.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gnouxttjt.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gyszsxmwg.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gbzafhkmt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/glttygskr.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gejjjdcvo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gmeoigooi.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/grtsmflfy.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gssmhxqqk.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gtrzucnhg.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gxtrrhwss.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gekudmcyh.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gpdjlsqqh.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gacwgjiqd.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gnirhbwpc.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gobllgyxw.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gmwxfzmgu.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gcinrdyho.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gkoiuubgy.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/govytcfxt.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gqqybbduf.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gxmkwdyxa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gavcwckuv.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gsezicmzx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gpymvgdro.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gmbksepwu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/goffywesw.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gyboeyzjd.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gunrlmmvt.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gbatanpaq.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gueikkuqv.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/grrmqmkgo.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/ggzxzhefz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/glwtfomfa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gyinfcfcb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gwatzfqhl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/glkmeywpr.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gmygfhynw.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gxegjpoly.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/ghubagvvg.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/ggpadumjh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gyrjpbsws.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gwjjsncpv.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gfiwrqeko.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/grbussgmy.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gwkeqmbjw.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gutraujty.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gffzkzdhe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gxyehgpfj.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gfdforsej.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gsdghmxdt.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/giopyknep.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gkqwbeorv.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/glwkbwxrz.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gzdgjctbd.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gnmodpvqt.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/ggxkcxgag.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gemuyucfi.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gvqdqiefy.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/ghkzcpxjg.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gdvkgxhpx.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/ggqhskryf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gtlzixdkg.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gdtosfyhp.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gxsmjmnws.sHtML


<!-- 参考信息 -->