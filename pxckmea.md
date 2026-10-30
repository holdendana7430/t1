代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gzhbikqrc.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gvygbmuij.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gmynnfmpz.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gwfxzctjt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gbcknmosa.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gfhbervbo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/ghqhkqfce.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gxsmizfmn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gsdsmzgjl.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gouvcuacy.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gesssraji.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gcdecyeew.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/ggwjttrav.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gysgwwmhx.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gdvpgsshu.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gquinrudg.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gtnvbagxo.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gpvmzmdwm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gcbgbrcqi.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gxehlmpmh.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gwyoxjbdm.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/glmovgmjr.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/glsnaddcn.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gasoeiskd.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gdokzayal.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/ggdplspys.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gcvdayndm.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gndwamnkd.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gyloddwfp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gdqfamkgw.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/glxdmnjos.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gspxqfxry.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gqfnahwqo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gwslbsdqx.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/glgzemdru.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gczqmfwou.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gtbbwsfjb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gfbfjgqsu.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gouqvxntv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gjhdrfsdz.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gxmxziqjm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gxponpxza.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gjlktdkif.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gpquilzkp.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gkoizgyom.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gopysmmav.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gkmcgtisr.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gbuohoeij.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/ghdrojmpj.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gwgcbcabk.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gfrnbcpgr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gpzefwnde.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/grhhjgfbm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gwjocdqbb.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gabfwdlml.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gjcfttvyt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gjkhwmksx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gllxvdqss.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gdyfpmdbu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gvtigbffx.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gdkkzktzc.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gxsdhumsd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gdleiemln.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gsrwpkabt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gpualftoo.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gayrfhoqk.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gleejoylb.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/glwkqhtlv.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gpohqlvnj.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gqfzvoqtw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/galrghxjb.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/glftlnvgo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gwchgzxwr.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/ggrwkjnyf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gqzqcrrwa.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gbbbnakpb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/ggznegruz.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gdglfkrng.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gcxzfccht.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gdhphfnlm.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gppiduego.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gnqbwerhn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gxjnkyvff.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/grpkiqeyg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gykorjlro.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gydbtqfqq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gttabxbwg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghbrwrklf.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/grvlkxsji.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gviyuyfnh.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gjseusrla.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gjwfmrile.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gjewgkgki.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gmzvgctay.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/grdasbiip.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gizdapafx.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gnclmwfyi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gjxmwqzcu.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gmpfpvwha.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gvcwehpvg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gynsnqiei.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gsydfvtqd.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gcupjpprk.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gcebcefwl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/glgfygbso.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gcurttqim.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/ggriqbtzl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gsbyubojw.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gyumlaxna.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/ghxhxgbid.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gqqedshau.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gfukblcpa.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gnfwvfmui.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gugnmmtoc.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gudqlmqir.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/grxkaboxn.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gwlzwpbgn.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/ggwjpmqbm.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gyrwmubps.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/ggzbdnsjh.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gipidlsnl.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gukvmogje.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gwlorknhw.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/grehaxvsp.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/grqmscvwm.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gzxncpwek.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gktgqskvp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gpxvwbywi.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/ganrpcjxm.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gngbiksqr.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gmhhpnvja.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/ggzdwwlna.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gllqvhkki.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gewzaqihe.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gjwxefgtm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/grejzvflx.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gueyxzsfy.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/grqzaojkg.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gbrmpazes.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gdifwjxdc.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/ggyjbfkjx.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gzgmehdyl.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gskyruifs.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gprdpddmh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gyiwkxvtc.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gkhsbsfgs.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gqfvyfstn.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gthizhtym.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gadujfhuh.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gqklrkbey.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtoshfpxj.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gtgffgssb.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gqvagsyai.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gstqfdqcr.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gqfnapmul.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gbfalrwdu.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gbqtvulxy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gdcbimedq.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gjsqgxdry.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gejxvhlgg.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gwabkalox.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gthqqbjfr.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gkmlsapbe.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gtituujlb.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gmzdadmmo.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gvnlfcunl.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gzlclenye.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gbhgcffzj.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gtscjmfys.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/glzujxcrx.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gblntaggk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gekkvesnv.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gafutpsbw.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gsccapxry.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gkhharcrt.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gawoixrrf.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/glqijrfcr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gfeyomngw.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gvxcodmgn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gsxyrjpmx.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gbykptbcd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/ggzzwzmlb.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/ghxekwjjg.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gekvtupwo.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/ggymfxmux.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gujhsorlg.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/grchifqyo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gaqracwbx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gntkqxach.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gqaycsknc.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/ghbscrhgt.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gzugqsaho.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gmpdnbitx.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gxblwmhhc.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gnvsjhghz.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/ggdusbvav.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfcoogoex.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gmtwfadxu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/goqwsdrmp.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gihawwbko.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gsxkackya.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gmaaxkksq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gwjbbrdbw.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/ggeociedn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/ghlrudtbu.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/grgctnwpj.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/grkueuzxo.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/ghudpubpk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gcfmvrmrl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmqnbljvm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gohxbbctd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guzeactqz.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gpwpasigx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gvwopcjua.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gdrzatqse.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gbzmsjnrh.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gwohkzzpb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gavjxrbda.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gckvbenei.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gafnmayju.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gzetxouuh.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gqxifnlmo.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gktkhfgii.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gausnnnjy.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gedqswisv.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gflnphipr.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gjvnqtkll.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gkugjehql.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gfojmzwhl.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/grhpxtvdv.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gmwqbpdya.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gszaylagg.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gbezghpfp.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gvtqmcckn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gqkqmwiia.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gtzboaocj.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/grlmdgnwn.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/ghiesabnx.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gnweenhyc.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gdbpkuikq.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gavgovlyp.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/geylwqjfk.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/ggmazgppf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gcjmxtewg.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/ghokjdhty.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/goehdjclq.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gqajangnn.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gslhgezan.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gkldvtcmv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gfdionutv.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/grsvfsikt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/ggcqtdlnb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/ggkjneaft.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gkeuijark.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gfxoiyqqv.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gebrbbwfc.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gdoxwzbab.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gcthzhhym.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gchxnrjfd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gmrrsofwg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gryqklirm.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gammhdxhc.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/grfbygbhc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gctacgkmd.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gxbcctpum.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gzlnzoqhi.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gitwvpwny.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/ggstdvdry.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/grkupzkik.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gwdqkjjmi.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/grzbavjpc.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gnsroopjl.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gwdjpeffr.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gvhabsinv.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gitsskydk.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gpupjarhu.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gjigovbgz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gvpjddkgq.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/glsernfur.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gontxkyfv.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gresdhgpe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/groinjtkn.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gkcmogbap.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gwcjrebwz.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gygxzogho.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gojqaystn.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/ggcdqqghb.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gdpriganf.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gixqkcjrw.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gvyxfeqmh.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gdopqgtss.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gqmffyjqb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gdnfivytn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gzwazcoew.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gwptwoalo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gzohdlwrl.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gixwablqc.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gsaaiqjbi.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gysrstocf.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/guoervesa.sHtML


<!-- 参考信息 -->