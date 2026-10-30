代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gxqaometr.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gglrxntih.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gekgiypyk.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gzoknjwmz.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gwnyysbdj.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gxpzayxbg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gksmapjno.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gkcicvmkp.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gsrspjgtp.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/ggyeuqtrv.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gokchvmgh.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjkilbgjq.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gcaxpngvt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gitlvdhyd.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gkmeqyjrt.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gaicdmgmg.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gzqkelymr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/ggvozzafh.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gwhxdaqua.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gexpztjej.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gfjhbwbpy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gsjunmigp.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gfalgjfbj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gldihnski.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gbkeszitp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gbcgdxycd.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gdroscvqa.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gdghoiheq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gxqeowqhm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gqonmdjlf.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gqhjfvqzo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gprssbhzu.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gxpxgithh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gnduafftk.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/guslumgbs.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gzftluaae.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gyhvjbdxp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gliozfrvl.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gxxmeqxzv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gixooapcv.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gbsupzuaz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gvctimbeb.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/guukjhssr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/glepdrjsz.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gnjzmzaxh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/grjhtsoxr.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gipyyumvv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gfpybmhhh.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gedvmibfr.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gnsnklouu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gbcbzpemf.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/grzzyzotp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gabhrjxjh.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gfziabgwz.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gguplscfz.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gfqfzwhjf.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/govpdqpnh.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gdreihnus.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/ghwvvvdba.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gvmbbwfax.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gpwmxhwbn.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gcwwlhqid.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gqqetjpve.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gjobsvykd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/giffliiak.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gtjoasuuz.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gersmgdco.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gjtdajxvl.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gtlsbsqtd.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/guiaftyyl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gorngxtda.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gbflrymvb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gtlkvybfm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqvztsdyb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gufzsiwef.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcpwfziyy.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxjmiphhb.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gpfjglqsh.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gtchkioih.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/glyzuhgoc.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/guxmujxjp.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gwpcpkadh.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gbilmgaoi.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/glcjdpcjw.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gnevqqbll.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gowxkmbdz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gnajghxmo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gscnjubck.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gqwuwgvck.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gmbqhuwme.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gjgjkitcz.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gcvlubbxa.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gxzevglbb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gnmeqjfih.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gcnpuenpb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gbbalzuac.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gmksglcnr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gebqvxtst.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gclpmzgbb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/ghnbpjobi.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gtohhuyvy.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gffengety.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gavwafccq.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/guqponfid.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gnwyacdnq.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gfkoclcyi.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gutqvxkpo.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gyuakafdy.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/glbfzslde.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gpzedcmlu.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/glysovlac.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gvctowunx.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gvquabaxn.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/ggoromqor.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gkeschvjx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/ghdhunzrf.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gplsohzun.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gdzrcyedu.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gnmosxbrq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gmugzeqxv.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gepgywibm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gbqmwymoc.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gmsepwigu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/grkelkwwt.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gwaycyzvt.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gptcgovng.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gcomclztd.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/glfzomqmw.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gnyuumquo.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/grqlcuaqn.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gjicbcfhf.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gvqcahkub.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gngmfnzpi.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gtzecpojq.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gsgfajgdm.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gwmcxdnwf.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdlwnrswt.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gwffwdcrc.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gxhzaykgs.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/glxlnqkti.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gpdtfgpvf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gdhuwsgiz.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gdqywykmz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gwlpjzytc.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gejjkzzkx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gkwtakdng.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gvszeccup.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gafhpabdo.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/grzgeonxb.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gwnknoxar.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gaerzrmry.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/glfrrbkuh.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gilhqyyzi.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gvextyisi.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gtecisoyv.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/geealqade.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gtzczxphy.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/ghevtxnvq.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gbsyltjxb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gsgcylyaw.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gtrfnzksc.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gtafhnmzo.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gkpfkriri.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gxlaogrfc.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gkxgqmgkn.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/ggfktgdbn.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gdcdmzrci.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gmkprpsmw.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/galdeggkt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gwhyphlsa.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gkbdjrvwp.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/ghjmceids.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gcxghniiq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/guhkbqzfg.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gvgfiivop.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gxhplvgjl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gdswmmeru.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gtklwepvi.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gzhqtlbzi.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gfbrhrluy.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gindspelo.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gpkuejqsa.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gdsviwhqb.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gmgeadpdq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gumhfusjy.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gvyqaxxhl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gpzigkngv.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gpooxsowh.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/guroqltjz.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/goybxohzz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gleliihls.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gvmhyznkf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/goczdavig.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gbvdyfnav.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gjjogpmdv.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gjafrlesh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/ghruqpsdu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkpvaeone.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/grsvmzlup.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guwlzsefz.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/guatsotmz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/guhufdsax.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gwpugygqf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/guvjeayad.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/glypdenui.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/greurjpij.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gecpudgcm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gzkecftqe.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gcrundvec.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gwgfkyzyc.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gwutquhpd.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gouokdxdn.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gzqszdsgj.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gzkpwfkgs.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gxhpdicjp.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gytpxqmof.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gdcxvdfen.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gtztlsglh.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gslatxbnp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gneqabeei.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gnsbjgzdn.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gphpajzqg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gcrkabzki.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gquusmbbk.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gkcteswzi.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gweidluze.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gfexfzkhf.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpcmokcx.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gxmswvtoh.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gvetzeely.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gqjgzrxde.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gefaqlvff.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gnyfqsjnd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gjnvmezft.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/ggvsitpre.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gchoqdxnn.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/grgeinsxo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gybyltnxf.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gwucqkaxl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gmqarqyhz.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gunadwtoa.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gxjzclrxg.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gyqoxzytz.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/ghgezkwdt.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/giztytcgm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/growzmikf.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gzfbeuxoi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gexkdjsca.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gvwbxcraw.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gblqxjjdx.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gmeasucjn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gocypufop.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/grtposgbv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gdifmquhd.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gfuhzxpfo.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gzstwihwc.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gmcooomff.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/grqlyprfm.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gdxccgbst.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gdrfkikhm.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gnherkyhn.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gphkjcelm.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gkenllsyd.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gzgdbrgwf.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gmwpzpejl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gbbfdhchh.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gnzyseqcw.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gjnyhzkmw.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/ghzydviln.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gvdkmxgcz.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gmqouobvu.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gjaitkqjw.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gzhnrfcpz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gttldpjwc.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gwgzfiwaf.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gfrjozlkr.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gokvrgdke.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gavuthwkj.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/ggqznwfil.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gpjclsbhg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gkmcskfxq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gwwoubdhz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/glpyszvpt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gzhxhqheh.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/ggitxobqm.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gzytkwkcs.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gmpebgqra.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gqvgbxwxu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gawqbpclh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/ghlusmgqp.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gsnayyjxx.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/ggccsoiak.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gibedjiqq.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gfhdbutkh.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gpqkkmhih.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/guywmqkmn.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gokzbpdeh.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gyvlvnypw.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/guuqfpbux.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdozklhco.sHtML


<!-- 参考信息 -->