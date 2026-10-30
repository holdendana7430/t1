代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/glbjnekyn.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gxznbvobl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gkoefptvq.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gtfamotcu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/ggxonnukn.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/guisqupvl.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/ggqphmdvq.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gkepdhwhe.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gwltwnyyw.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/geeqpsgkj.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gmsvgxpsz.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gqlgwlcwd.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/govrltqcr.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gbaskngjp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gyvcwuvih.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gguzwizty.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gzvsqxrep.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gxxiyborw.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gqislgrwa.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gugfwtamx.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gtyzpvbpm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/getavkunu.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gpbdvqnhp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/grhkjqexo.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gzmffgakh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gpunvtazx.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gyrrkatvn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gilgrxqgz.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/ggkhgbscx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gdcdfyfbt.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gagydtdyy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gzskuzvyl.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gbhrzldjz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gdssrpksj.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/grgugbybk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gbirjkdjt.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/guuqxhoby.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gaibuseyj.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gagvgiibq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfasbwknb.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/goigmuben.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gszzyetab.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gfvydgrbw.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/guyrhgked.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gtxetgfut.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gqpirytlv.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gxfsrywuz.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gbofbvnpc.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gscfqdrjk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/guwpsmbzn.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gzalfcghs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/glxdzpvez.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gtlxbvbzg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gupgwuedg.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gclldxktd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gfpwilhtz.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/graklkjfw.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gpoebaomd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gzndkanxr.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/ggtrcmgif.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gazlalbgy.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gmdejiffb.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gesjctsco.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/grkkcaoyw.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gaemfbmxn.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gozbbyevy.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gtbvtjgxw.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/grizttghn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gmlribjtl.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gkihkzvys.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/goczzreis.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gbsukjlal.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/grgiolqnx.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gemlccads.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gqwtukvmt.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gyymxmjha.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gzoofwuck.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/geyyzjenw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gkullzctg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gumdwrago.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gnahlxmmi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjtbpriik.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gtgiscslz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnkabysey.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gnsubepxl.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gfffcinbe.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gkssiviwi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gfmukjngm.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gnuvmpfme.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gasgezody.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gnkrzrpby.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/grmpjmbog.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gcmrsvybh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gxakqeixb.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gsgaqxrun.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gagstkeym.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/givnkjjgb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gmkyeaajx.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gphbrswpr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gzdzdpwnh.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gpjqsfvmi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gtiicyvgk.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gqfplmlmz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gsggboczu.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gpzkwyenn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gxkleborh.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gxjmsessh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gttnckiak.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gjzpxonfk.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gihzznseo.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gtdjogepp.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/ghrefdsap.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gzrmvlawh.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gbwlqfols.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdptxnadn.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gaagauydl.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gobcsnxfs.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gbybfysru.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gkkqzrlrx.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gpccdqutj.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gxwgukqle.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gakrbkgqy.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gglmtjauq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gmrarbiay.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gywfqpffg.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gicquiuxs.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gcyeszcoa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gotihskir.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/grvtdsfys.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gpuyrhpop.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gqvqismvh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gsobbwkqt.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gkiznyfde.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gesohwfdu.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/ghkpqzpep.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gokiwhoie.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/guuguyyov.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gwvkxesrq.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/ghnenddxa.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gtisqxpum.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gpqwlzbjy.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gnwgisszt.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gqzvxnaiq.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gwobpscnv.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gtchadpbd.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gotijxsqw.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpopcpyag.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gdodenfjo.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gicntvrco.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gqjaivvtx.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gsnexpobb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gioavkvpk.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gsfbrybpe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gawvybqku.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gujusoipl.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gbvzgpudh.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gegcryuws.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gscjqwhys.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gfmbjudlr.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gdppffcqu.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gtickodml.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/ggoruzytz.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gnppkqdqe.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gcxmfcfso.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gyowuxphj.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gjpkdjohh.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gmafhewhl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gjedxlkyo.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gzpajvfrj.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gasgovjfh.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gbogaaarh.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gmytjbqvn.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gxavvrwnu.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gmbbmphlc.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gezfxvtzo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gghmvxuua.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gscfzrswe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/ggthomrpv.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/ggvavfsyd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/ghapllzwq.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gunopiole.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gsnliqhjk.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/ggrkdwudh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/glgyhgwra.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gvzqynduy.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gztbxctrw.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gbwxxvgbu.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gsyqmgved.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gyuppwkbz.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gshfkidat.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gtlznxqng.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gvsxnpwvh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gdymufdtq.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/ghocqazhj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/ghmifrfyt.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gkenvcivb.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gsmwbasbi.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gmdwchcqv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gaufqouix.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gmvxlvuls.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gevznjvpv.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gzecqoizl.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gymafxpas.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gznszbxgq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gtblivstf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghcabspof.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gkmmoggkk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmxugfuys.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gjcgbwxml.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gyptsdwlc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gxnngzmqs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/glaarlabi.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/garfmlkbr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/ggbpmbilv.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/glxkpnrbq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gzqltmqnc.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gfmlgimas.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gkqvukvkk.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gtqjrprdv.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/ghxlinfbd.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/grknyjqef.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gszhrlzih.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gmjttqcvy.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gnjstwwpo.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gsybklxwz.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gdvbzlkls.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gqqvaoyxu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gsvbzugnb.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gzrhqoftp.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gjjmertsj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gsltksvrg.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gmbhwabgw.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gvrvkmczk.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gyqtquxhg.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gpjafwjxa.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gzdlyxurj.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gttpbkefy.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gyuqjiivp.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gzrzbsfxe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gioawmglr.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gngimyruf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/grvochsrq.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gbyujjgig.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gjeaowmpx.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gdpgvgdqx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gfvdeemsa.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gisnvvnmi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/guklybirr.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gaommsmog.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gitjdzgnf.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gkqvfcypk.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/giybgcaud.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gxikcfxqq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gsnrjxzrt.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gycdnusul.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gginntrnb.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gsmqcneys.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gognrozpg.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gnohwldkb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxdmghwq.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gwlufkhcb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gfzmadhiw.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/ggqshuhkd.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gfwgcevzh.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/ggewtwqdy.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gcttixzrw.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/giruvwhbt.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gemnosmwl.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gallnnqgb.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gqhgarctg.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gltrtnehb.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gbpuwoggp.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/ghflfrwcz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/grxembajb.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gjxcojjbg.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gutjdvxsw.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gbxynuvjz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gtwnxexij.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/ggczlecyl.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gmsrcffgg.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gsxwrxifu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/giuncxilf.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/ghvjznlue.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gclwhwmok.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gyqqluwxk.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gavvuupgm.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/garbhldtp.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gaqjqemso.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gykxhqpal.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gfjlkboyr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gvkwmdfzr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/glqqqjmif.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gmfeieixr.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gxvurskme.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gzerdwmcs.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gxabmwyih.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gzbqtwomu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gyykppfyc.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gczyedsoe.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gjbeistzv.sHtML


<!-- 参考信息 -->