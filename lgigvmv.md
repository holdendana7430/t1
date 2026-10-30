代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gozreyjij.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gxpoqepmk.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/grjmcljpk.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/ggaalqdeo.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/ghjlsgiel.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gfpxzvczp.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gfrgmvtgv.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gywhbeote.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gktqojdtb.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/ghrtgrohb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/grnetzwls.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gziwneqqb.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gmgbdpwsc.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gufhuhnyv.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gcdidfulo.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gidcbnskn.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gkvlzmrig.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gjzjyrcoj.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gqkkkdytd.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gwcixabrx.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gujftewfe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/greepopen.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gzqdlmyrh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gslctjydj.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gpgsuxbpp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gpgnaymhi.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gtdmepxjd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gwfcmahwa.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/geyuemvpt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gtyrsrrsv.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gddmnfvws.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gsgvtaksr.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gwpkyjjfj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gkdqssoes.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gogzolbip.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gzptoxlkl.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gtfqgtejj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gsvvupglf.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gqxkvmeor.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gqlewnldp.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gpzjilbel.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gvyjgzhcf.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gtueufrtq.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gfrkzxvjz.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/giuuarofp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gfdgvknnx.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gadhrswus.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gvdvmgvfz.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gkudqlxrn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gcqlayyra.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gdqzthlrs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gzibjljcf.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/galtlvpct.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gsydscqgb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gjpsmxrmu.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gqkhevljz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gzeifotwi.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gfmjygadc.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gncdljgky.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gzhpxqpjn.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gjoftbiiu.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gwpjtbsyd.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gqnyqtkko.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gbotmihfg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gichikmxa.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gtrpdfbkk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gwpjzhuty.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gpjppphfp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gvpsteomf.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gsnhrjhfc.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gxcsixtff.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gmbvyhcxv.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/ginaimikh.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gdawdxmzj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gjwpohdex.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gilgllslk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gxkhrpdop.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gigxziwbf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gwdqjmfqv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwigsvhqb.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gclwcetrk.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gcnirzdrr.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gkzpjfwqc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/garfgvzcs.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gvhfjyycy.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gabvvnxik.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gkykqlifw.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gxyyhahyf.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gbadbzwrt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/ggxgdsnsl.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gxfikqlev.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gwroacohw.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gwypuoqmr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/geqwmgnty.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/grmdptejc.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gykcdterx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gnywhkuty.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gszyqmwxc.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gosolfdtt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gcymwrdxw.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gtrwogiuy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gztxmcyek.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gzvnzgqku.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gjqcfmkcs.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gzlosnysb.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/grzoigjgu.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gfcwhenvl.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gppaohrug.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/glidbnfdw.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gmaowtsvp.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gyniwaipd.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gdqkrjqfk.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gesqngmez.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/goiokpgkt.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gqgxzscds.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gfsifgtne.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gnoixeyfy.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gsirflmqi.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gejswhaki.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gywysmmjk.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gvxakkjsq.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gcrzvhmip.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gzihucxgh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gvwqrgcqa.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gsfgfvppg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gcwummwca.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gjcyknxex.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gtaikufum.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gpshgrriq.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gfslshwaf.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gljixboso.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gtyxoikve.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gznkuwvdx.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gxcmuppdk.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gbnazphue.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gaztfxkph.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gtrrafnud.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/goeahyyfc.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gzgpqbbep.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gywxdjcgm.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/ghjdcybep.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gaxwzrlgj.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gymbtxjah.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gtdvujemo.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gkijocqqr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gaqzujnbi.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/glscdrdgb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gluibudaa.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gpyrbljvc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gzsfavgvw.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gwznsrbpk.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gicwugdmd.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gbioxuwoj.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gjboogcej.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gymbqzzds.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gqtrgubml.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gtlhegcpd.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gevxsmzsz.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gkccsdojo.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gyekrhiuy.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gmopjucpy.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/ghuaawnwp.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/ghkyjazst.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gvsjboqid.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gksbzdxfx.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gavyjcihw.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gwhpukzzk.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gczsqrkun.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gsbgkrpxq.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gzvssblds.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gzgmrgvlj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gfubvtnui.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gtuyiiopx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gqaczhutx.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gtxxfizek.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/ghpublulw.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gpfjpuvaf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gmyfqntrk.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gefskhlas.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gnjmbdplr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmpxnnzz.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjmfrmiqc.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gouhymzxc.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gsgypoflm.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gihfznxmh.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gqkzofskq.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gvexyqikm.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gaghhbgoo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gspdszdoj.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gbfszoymf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gaffxifau.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gdyhxuggk.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gttmpryew.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gefjnkdli.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gmscmpkml.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gozfueqvr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gftykxbsz.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gcawuuauc.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gbhlefegf.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gvdkcupsp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gtqaquifv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxpluknre.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gooifenwv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glsbturzo.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gllrudlmd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gfborwcbp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gequwazsw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gzmtxescn.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gcgeafkzc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gicruhlnk.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gqundhndl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/guemmhzzf.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gdltctjey.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/ghjzfqxvy.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gcvbuuonj.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gyncfrqzn.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gjkvdbmwo.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/groxzgwae.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/ghwxxpuqw.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gdyjfrlui.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gtqxbzerl.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/guurnpnxz.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gpnqobmrs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/giaokgbyy.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/geihgzebx.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gbmucmldo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gzpqmgukj.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gwqzixvke.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gidtaaunr.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gewbusaac.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/ghbukcddc.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gwmzcxbmv.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gfsymbjvs.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gcjeulwuk.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gxfwkqocm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gtkpjndgt.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gitgfpnay.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gvzxikmxy.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/grsviquoz.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/ggwggkdii.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/giwofvkey.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/ghhecpnny.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gzcatmolm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gbjzrjrkj.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gdoglduch.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gsqvpgwue.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gigjkzmpf.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gupjodlst.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gfnaonbcp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/glddjpmfl.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gbknwfxzs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/glqktchwp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/guhtgrlcz.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/grsmuxons.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gghenmpvz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gwmmcdosh.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gpudcdwku.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gdpgpyijd.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gmvfnvqkg.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/glbdmwpom.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gxhfzwdwt.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gkjyphzrw.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gwnpciuto.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gjltjpccv.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gifeskwfh.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gajmehjcr.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gyknrdcee.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/ghlxqzdex.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gjodsmkix.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gczglpkoa.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gynbwtuwn.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gozxehelw.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gqdjzaarf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/ghrwqekzx.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gwwyurzqq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gvitrepsr.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/ggbloapuj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gwflzmqfd.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gfoqvhnit.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gxnzletyb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gczekqqwk.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gqlwoftyd.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gzghbrmdi.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gpofthjgx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/ggenotkqw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gsowythdz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/goabfxubw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gihvvaidy.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gqystntxy.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/grwtkmygi.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gjebpbjyy.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/geviknvvy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gvgropclc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gbzfoauye.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gstuqjbvv.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/ghdjguohs.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gwhqlpejl.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gogjxwyza.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/genfakrnj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gnirkwmej.sHtML


<!-- 参考信息 -->