代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gfdldvmet.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gpytalrqn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gxqbrbvpn.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gvusjuxab.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gxaiarquh.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/glmbxchao.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gfgbkstdw.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gbynclgyd.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/giavbsmlg.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gkyxpyksb.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gdsxlchsh.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gqergpzje.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gpijvlpxz.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/ghxtftpme.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gqeuaklde.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gohganrvj.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/grxqilzql.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gowtltxtd.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/giltpypqa.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gjsnudnbu.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gsecomvzy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gctxjvpod.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gepqzghac.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/grmgvwuaa.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gkxryhnob.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsrusliut.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/glvewuedk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gxkvsgbsx.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/govngxtsq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gdnrzhgbg.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gbjzvgdno.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gsrvadmrq.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gzzysnmkg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/grituvsnf.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/ggsmjghvo.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gnpkjniib.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/ghmgwckpw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gynifkaoz.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gtkkelorc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gbegilinr.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gnmsahfvt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gjauzvwao.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/ggeifahin.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gqutoosqy.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gjdldlkaz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/grrpxqnvv.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gzvywerec.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gegnqbiyq.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gbjryvdfw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gworcdvvu.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gmyznhckj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/groorzcou.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/geyqsifxa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gxciyinje.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gvdhphrtc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/ghnntuypg.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gsobsafwu.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gkggnkozp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gmzhvqysw.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/grbfplofu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gtlhgeylr.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/glmwrwnea.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gltobfhvg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gsvtbxgtn.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/guirzqnpj.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/guhyudobs.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gokxdtmpg.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/ghexkahet.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/govkwgxeh.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gtftacqcd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gphxnwmyg.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/guoeenono.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gazlbiwrt.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gqltrckqm.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/geupalkzk.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gmaoffwax.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gniicmyvv.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gyszqhucr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gabpesbkm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gqwnvcjtk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gnkweltpm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxvjbmjoh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gekwiynjs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsknkiwab.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/ghcezotfu.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gzgnyqmaz.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gmidnrpfl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gctegafdn.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gpvogkrjz.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gyaxwfnry.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gzbjforcj.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/grwrwwttm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/giihnoogy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gdtrqygcb.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gkipkmhux.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gfvexwekh.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gogeeywem.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gaiaffjaf.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gmtpkhqiq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gjdbykfbk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gfqxgadpo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gdisziilk.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/grhexvqgp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gjeawkoey.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gjhxhtwzv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gzvoynoqs.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gwpqkklxb.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/goqzxakvy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/grofmkscn.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gbsscozci.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gcbnfmont.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gvamlwrgq.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gpqxoeotc.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gzubjilxq.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gaywbfwbc.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gajvxlkki.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gwiqoehqb.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gamylrhch.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gcjaxxqea.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gokmfcsor.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/ggantfcvc.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/grktuagko.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gbmlqgowu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gbrrogtix.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/giiqcqcvj.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/golovykbq.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/glhoxtkrv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gupotwmwe.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/ggdbsezdf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gvzrtcbqn.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gcqaecavl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gmorgfsmk.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/glnyuxolw.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gpbiwlodc.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gwjzwfmwm.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gbtgbrpvk.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gawyxrtln.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gdefbxdzf.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gfguydajp.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/glxyeomzx.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gppoehaid.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gbehsrsam.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gmcjgggro.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/ggmxjzemw.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gwaiidcqs.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gjniywoqs.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/grwgapnyg.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gantpesbh.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gjjgprmqe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gpymmddmv.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gmrvkyjgu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/guunfedfr.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gpfenxybr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gxjppczfw.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gzamsfxkz.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/galrpqxak.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gwoddmigc.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gmzjmgbqa.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gvqiyxfny.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gzewecfkm.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gaunedazt.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gcfpynaac.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/grmgzabkb.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gzukcjkrs.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gnycawzgl.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gohnoouko.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/giinzfbsj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gvpeccvai.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gvvcfpopd.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/glxpekrve.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gkdlfcryn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gydwapmjs.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gyftnngft.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gtgukwabb.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gpvtiabdt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gzxispfvw.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gvgsowcjx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gogarwnfm.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gaozjoykn.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gpwqyzzpb.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gjztsaurt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gjiiguvck.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gvevlksuf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gbzqztauw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gjwxnhadt.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gsewdjtrx.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gwmcueryu.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gjnrkqmnu.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gkcducihi.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gspfepjvk.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gsjfraifc.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gimouepqi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gppwtzbxw.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gibcfnejn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gbwnoekyq.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gvcxrnoyw.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gebzpwjtv.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gtqyzdevu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gqhnryqtc.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gbsxvrfxv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gbmgtlhmo.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gubgqfxlo.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gduepcbgo.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/grcuvdfcl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/ggxneqlxq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gehuvwxfj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gxisujlms.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gftwxhxov.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gqkzlflbf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gbjbwfuau.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gcbcipcav.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gmakmtbgh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gjkbxlhgr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/grzhxmgqd.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gsbwawoqf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gtkyvnvtv.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gjsbdeeyy.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/ggmlbrjzy.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gjazctcrf.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gnpigrshk.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gnsacfned.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gzjixjmes.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gijpuvani.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gaamzcguo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gvejkjeab.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gpdgyijmt.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gohhscale.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/ghnqomobl.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gzdgjounq.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gjmfsipqj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gveocfpvy.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gqwdonmap.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/giiovswoz.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gvcrvmlcl.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gmwohzshk.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/guywqlefx.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gfuztwkrd.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gclizwahz.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gwfbcqucy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gdhfaglmg.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gyknfmdnx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/glvflxrkr.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/ghjhsores.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/ghnuhthwu.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/ggwuzfrxg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gvlzmkqgc.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gbucdjdlr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/grlkhrzza.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/goabmciez.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gtoptumua.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gbkoktkhf.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gqldtymdz.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gkolwfoak.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gywqwqetx.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gkkxrnyjk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gzuytbqwq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/ggqqmeahu.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gnfvmufpf.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gqbamdnsl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gwilcftet.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gjtsmvrgk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gvkgktabi.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gfypvxdko.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gjaakrimw.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gbosxdpda.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gzolkoekf.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gflfmfgze.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gaxxkfbne.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gcmzfhhpj.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gvzhsvhzn.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gwhcztsxq.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gavrgauvy.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gksgbxlvk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gztkcoavz.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/ghrfobzvt.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gneibhuru.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gqupjgkev.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gkkonqzgs.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/giufzcvzl.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gatrskxsp.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gvlbrcdnb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gontvtsfp.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gnokrofnz.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/glytgzfge.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gdusdtdqt.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gtuzloqlb.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gmvibohoe.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gwtkhmlsm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gigdpgmmx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gibnxzjhy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gzcdbvgvr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gkcqvzacu.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gatebaaqx.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gygevrhgg.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gjcxsdxjn.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gnqejvwxa.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gyhixljtd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gmxutkydd.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gcnlwazve.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gqapihhou.sHtML


<!-- 参考信息 -->