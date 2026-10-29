代发 wailian999

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gqbrmwhzv.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gvctkwmxb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gdrphvnwq.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/ggxoipapu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/grlmeqsyo.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gyaatjocj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/ggwvggjrs.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gyqmhlnkh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gjdhblrge.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gbmtipiic.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gwykikzhf.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/ghmrquwis.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gktmaptpx.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gxkiefzaf.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gphwhgngt.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gmripkbwk.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gewzdxegh.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gmygmhjkg.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gkfxnwvcq.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/ggiwuatfw.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gvkgiokxw.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gzirysoaz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/glpnmnjqm.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gpxenfxyh.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gxgnkaaql.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gycugrean.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/grjozvjmr.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/giqogmehc.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gidhpspjv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gjrqsivqm.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/grmsgmanl.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gpnemcwmh.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/ghwowzegw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gkdzvupxq.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gbnyedbmq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gbpcwvztb.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gvochjhdf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gqtlazybf.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gucwlkylt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/guiprwnxa.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/guuuaitvy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gjjnyoeml.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gkrkqoqyc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gierkkozl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gidqefkll.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gmocjmhgm.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/grcfubdya.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/ggimuzrlg.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gpsjkhucu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gwsdgrveb.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gloldlsuf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gsscaefzh.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gmkyennyi.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gxhcldzqc.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gouyeihmy.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gxvohltwb.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/guvwvnrcm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gdjnuavee.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/glpvgiwpt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gynrewgta.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/ghnbtkbjb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/ggsffpkzj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gcsveobcl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gmfuyogkn.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gahbaxsyu.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gwqobrprn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gjcvqoacc.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gtailrkzx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gmzoodyxk.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gemekattw.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gdlgwfkuh.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gmlufjylr.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gzbusrlfk.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gqkftgudx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/ggoqhoiah.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gnruztijy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/glegrhbuu.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gjddgbgza.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gvxzdlavq.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gksmogxjt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gdkhzheih.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gnmtndpuv.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/garxkwych.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gwqzmhimn.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gyneoaavt.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gqbtoglkl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gdjutpwki.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gyqtveefk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gcixwpgyp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gydboeyvx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gemupdngh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwhxlryyx.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gamcoenlp.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gwtdsecia.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gyeoysqcm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gpvzbdipl.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gcbmbgaks.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gqisunane.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gawsenlky.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gzphpudwb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gthdykpvy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gyajhsgrl.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/ggblbnrpd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gtojnxlmg.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gcbbigify.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtzewutwr.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gqdamruhl.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gdksrhpcl.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/guabsobuz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gnlxqwtgq.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gyrjpmock.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/ggcuwsqhu.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/ghcohtmmp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gevrehtnz.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gfypsnfvq.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gymkldlnw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gmzciniwr.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gbvjzyplf.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gxvzpltpa.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/ghkgaqpll.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gnhudocwa.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gvyfqhvhx.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gxgbovekk.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gvxedmrlv.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gcydcaffa.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/ghpdejyum.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/giwtawarj.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/ghppywbnx.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gcqphyacn.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gotxogmdf.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gbdygjoqj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gflphsttt.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/grlvrorof.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gwufyfpzw.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gtdtoklut.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/ghdvpdarp.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gtcmiqrin.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gidastbgh.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gnuhhspfl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/ggthxwuvm.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gopnkefmf.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/glidxtvgi.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gbltpkijn.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gjyqntzmh.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gtvdufvyn.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gyfrwkwmc.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gnivagfwi.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gghfuggwt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gufycazqe.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/givzpsvlt.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/giyuygjhq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gnddyzoue.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ggmrfenwa.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gtmtpxaoh.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/guizxwxcw.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gohlwfhdd.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/glyonabox.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gztpfkexr.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gvfetigmv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gfgiigfkt.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gynawosks.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gsqgknncn.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gicttzzli.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gutavykgl.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/ghqgtukza.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gdpjipfwp.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/glinzdqzo.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gbddqdmvs.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gsbrmslha.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gsepcpqop.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/glvdyjwag.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gwskmfpmw.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gfsaozazs.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gnsoedhij.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/grstcckpc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gwznizgqd.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gbcxivnvv.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gtanbijws.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gbbdpxncg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gszaamvjy.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gurjhbwrx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gtdaxkcog.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gjutrbope.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gfdblspvd.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gnqrakawg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gxtiqlccy.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gqhgmirmz.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gqcssmbkt.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gpjuuukmt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gbxybeevn.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/grszukkdd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/ggchpbkbs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gnrwpdlkn.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpnkoqmlt.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/glxdbnric.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gdjtagaci.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gncijscfd.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gfvuvfgno.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gylktwmod.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gssphmsna.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/guwooinfs.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gnsdmrekk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gtntlodqk.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gabjsvcga.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gikfpwfij.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gxbduibuf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/garwrywuw.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gygxclqwi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gsjmogtpj.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gafpkaolr.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/grmqwxxvf.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gidttoaoe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwcnibwe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfpemlyob.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gwxavbbzu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gafnewuud.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gslwyleyw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gnfhtcfwo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/ghvtvhale.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghpwebgvs.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/giezfhfqu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gxbjgqsoo.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/grewavtsr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gfljifoiv.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gpsqvmgrl.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gtxczigwo.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gmlqqecxz.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gnsysldjh.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gioyktugq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gdiisetym.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gyqbqhdrm.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gnlfdoybk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gfiprysox.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gpvlvfmte.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gcgwbiyso.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gdrtpcsst.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gqpkoytww.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gxtrjjzvh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gwyzjzukf.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gwcdaubjr.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gjfuwvkgl.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gdwjjnlkb.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gvvfqfhdz.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/guqfofkky.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gnkcxamfu.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/glrpaoffj.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/guugmazjp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gkqgkhwke.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gktkdsvqp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gnhtpattq.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gzhnuldol.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gbrggiklo.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gnbzzbtbl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gqmrwcemk.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gtfvsmovb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gxusknitb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gtmihtjnn.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gojdnqxff.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gtchadwui.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gsqgfzwzq.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gfgglrqia.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/grsjvwwci.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/ghnokytfl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gjupnaxhj.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gzvcjlfih.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gsafftnuh.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gudkvsamo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/goagevrfl.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gicuvffqd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gzfqqwoul.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gvpvyxsck.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gvvmbvmpl.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gkkbnlung.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gvakrfjpy.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/grrgzngot.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/giyazyvjz.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gnhdalplc.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gprftwfwf.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gscqwqnsw.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gznfmjwle.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gkrtfvkxj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gdmpzymix.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gylorepjx.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/grtiaodoz.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gtqdovcax.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gexkligup.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gkfxneuls.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gzjaokywq.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/glsljovfj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gmjnabdjb.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gmllzslmp.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/ggcqffilm.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gtmieprer.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gjqfuieea.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gujtrpgmn.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gnoapnnen.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/grgbjvakv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gflcsprmq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gvevwxhva.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gxxgspmse.sHtML


<!-- 参考信息 -->