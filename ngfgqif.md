代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/guohpjzfp.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gqydqvgze.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gqkephuio.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gwfnqktys.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/geembhcol.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/glhnjvnyx.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/ghbfzukoc.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/grzqfqldw.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gzanzoirs.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gbqxgwklp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/glmolrgon.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gtusmjacd.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gdngtyozm.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gcnthdiwo.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gqlgzbthj.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbizzhlvp.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/glrerdiyx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gcsaitbrz.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gkrekbmme.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gtuyujzbg.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gmbprdrgi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/ghilrglqh.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/ghqljhmne.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gljzsrbqs.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gizkvsien.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/grnknwsgw.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gqqvelfxh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gnlraijux.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gtblbpcns.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gdeovlwbg.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gijdmmwpd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gwvqtauts.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/golrqqcst.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/ghrcmyycf.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gsgcbxshb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gflckupcw.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gelnkfgza.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/grjgaalfs.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gsmkghajh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gvtbjndcx.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gvopenheh.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gsmtwaqsa.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gxobqtcme.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gmvznoqik.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gmcesfswb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gkpriepdy.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gfovcojix.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gbfwbfgzm.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gxkwbsqod.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gyywohpyg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gsfwzouco.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gnhqytxge.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gfmekmrhj.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gpxkkzvyo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gxvlsglii.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/grywignyp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gkqcomcrx.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gchaghlfd.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gwvjeplep.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gwfgzzzua.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gtawnpakq.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gfxrtcdzs.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gfjrdumdx.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gbosbrnrj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gwbjgtjtj.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/grmxxsgtx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gtdixvpni.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gyfjuzdxw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gstrizbqm.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gseehaojc.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gaxlzdyho.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gwjfaxdpg.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gihdlvdve.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gkcsfojho.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/ggrbkapyu.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gjsfcsbvy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gtupmsudh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmjcstajw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/glrecsnii.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghlmfkcdb.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gqmjnofnx.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gzgzjrtwd.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gayasyccn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gqmppgzog.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gvhottmcc.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gmqbemwsw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/ghvrcvflq.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/ggdsuzyof.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gwoduksyb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/guegyeavg.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gbrotzryt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gqnztxjao.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gnhxkotfu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gbcensbps.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gngutdjrt.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gydnkejui.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gsfwzlrup.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gkhraauaj.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gtqniyplw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/grityeuzm.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gfgnnwetz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gljpyfpxn.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gxhvyjqhm.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gzebpgyaz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gavovxbnn.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gnmozlkyn.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gsyxzyxcr.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gcmeoinxc.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/glmqzomif.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/grzbbdznx.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxiomerin.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gdacnrtyu.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/glubkunqk.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gthpdgsaz.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gthjyjgam.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gtyzzwyfr.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gesyihfnd.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/govmrytfr.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gfjmhghdq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gnlufhgez.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gnfcghgud.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gnimnqwej.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gvwlbapjg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gwswrqton.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/grpzikypr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/ghtumtyuh.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gnuklxoew.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gwdgkfzly.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/ghsarfxje.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gupusvspb.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/giqjgkdnq.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/govherahx.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gjfdlnmib.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gxhfnyxan.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gqbgbaspp.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gnxtnvniz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/garnkujpp.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gwoyxraso.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gzjzblslv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gofuablsb.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gzrmndjzh.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gjwichvpu.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gvxsrhnrj.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gmmnmtjtf.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gjjnusrlk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gguixrvwk.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/goqjmfysr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gwcnlbyll.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gvormzbaa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gnpkbnxze.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/grwdnegck.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gluudldzs.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gwjdgqxyv.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gokwwteky.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/ghiqjstuk.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gvkzjysrs.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gekccomnt.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gbgvghuvk.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/ghmbokopq.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/grvulfwsk.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gwsadwnvt.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gzrxozfst.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gafrciyvi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gnwfedsin.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/glgihkncv.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gnbcwmvyt.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gzcxgtpxo.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gmkoxrrqx.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gewrxqrbs.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gflcwbsxl.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/goiscunnw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/grrwvwjsz.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/ggazinnlg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/grktvmlnq.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gzkzanrqf.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/ghunvfeuy.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/ghddfxrmx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gpbyhltlc.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gxyjzdqhi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gqhjzpmys.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gjptjxggo.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gnoclzgqc.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gwtslykqq.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gbkgaebrd.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gtgyulohc.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gyakdkogk.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gwuhsuano.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/glwltijkf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gvtfzexoj.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/glqfnnglo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gwzjaclia.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gvfqpxgmh.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gubwqaznb.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gouorvliw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gfhwmszsl.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gmqnvdqpz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gzpezfczu.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gilxgzzzb.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gqtszwtfz.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gckizggof.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gjuqwjihz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geegyspmx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gdmxuvffe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtututpkh.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/glwxptqjo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gtaovxmcf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gcxjgrgkl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gtsllcucf.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gpxwgzsvr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gukityqfa.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gatcazzlp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gynhwthux.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gjfqawdpi.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gabpfjzoo.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gvsitrglj.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gouevvgwu.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gjiqomykk.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gefmpulmo.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gxwasuirp.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gltawhwdr.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/ggzuegbnl.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gsnsygalv.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gmogpubsf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gwnghtfet.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gkuytbdty.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gnvveduto.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gvrgyacha.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gtljtqjuc.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gbgpguvuo.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gqelfatio.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gsajanedz.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gnbrjkqsn.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gleunawlq.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gyodutfju.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/glesogqvy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gxpghrhys.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gqfceedmh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gtdaugidq.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gixaolsnc.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gftespnyz.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gqrpwmkeg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/giyfgbpbv.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gqzyyagoa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gdepvzbjw.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gvbeywzfn.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gfczhbdqa.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gvsgbgukx.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/ghzbdiypw.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gmucxlqbj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gdmpiloql.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gpxejlxly.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gpodivhdc.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gfdrophpa.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/ggnzyatkw.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/grxuqfspl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/guxvzebqw.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gonvqmrxf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/guyxsxstu.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gnpybpaak.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gtszheeug.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gcplauvnz.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gyxtgujft.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gexfcoatz.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gsspgsffv.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gycchikum.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gkwwuocql.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gdviqlzwc.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gorabqwkv.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gwchogwyc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gdlgxzrio.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gedakiraf.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gppulyzdh.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gbjwrmwwi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gbxigobbt.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gwxsqcfri.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/ghvxzauaq.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/geupehnov.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gmtwxgnip.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/ggcpgbzgc.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gruylftoq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/ghxlnuhgb.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gajzrubhq.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gfmszfwqu.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gknorndqs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gwkvbsfvk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gbyahooxm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gzsuvhcat.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gtjgjnvhh.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gdnxmcfpv.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gdftwcwph.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gykfrrzvr.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gpesbdnto.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gqdjbmjtd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvndelwjz.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gxraoktmf.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gnlftifkh.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gvcsnqfke.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/ghftokqcq.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gjdfuowlg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gbrxghifb.sHtML


<!-- 参考信息 -->