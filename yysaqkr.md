代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gnzidluwt.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/goubhfqkb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsoimflf.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gnxcbjnfg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gbhzcjufc.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvhsrkwq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gjbyrtvoq.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gtijtktbp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhjazwti.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmikadnor.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujziuntp.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gpouleftd.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greczsazq.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgrbgjlt.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmglxbrgk.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gufwhusrj.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfvliung.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzgfrjvpx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gidwzgzvq.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpjwojgc.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbtuhwau.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnwkklix.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspsvqcur.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gcewtexdq.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorwhhumk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhrdkavs.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gghhfqxoo.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkeovugx.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjseskhs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdlrxxpd.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gkzkykenk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdryxrleo.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/glhgyrsmr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvzyradm.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxnfzweu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gcsdgmdyo.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstvafmhn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeytlkxt.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gfogtbypo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaqfxqrx.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/guupjrukl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gdnigxjsg.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gsofjfrxj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzdgklzd.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/grrtdkley.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gecsgiugh.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gikjoxraq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlcuqyvg.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzxlwgnh.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gmrmmvrlq.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwizlaznb.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyzkfcmk.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gemlpitbh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfiqpdvv.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gfytyyodw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gclpbivvd.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gwujsgvfn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcpemvwi.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypavddwc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxdmlgza.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/guurbzvzx.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqfelawq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gaflzgpgl.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gwpqowteb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmkvohhl.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gqeurowdt.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjrlcdei.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjzhyphp.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyipvqve.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfcjokwg.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gltwefrir.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/griapophc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gmxsicvxs.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/guwnvusax.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwcenuvu.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/guekpgyvw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgsdapqj.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gbeyolkmk.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gjfkjmain.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gklpuavre.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/grdnjxvgw.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjhyamui.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdavbcghh.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gmzgmqwhq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbxeaqry.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gczsawimh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwppxtosx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxzttwxxz.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwaewpjt.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/galmneffq.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gttmbrcsx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gypkxbfzi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyjpnveh.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gzqydtyke.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gthqozrzs.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gmlbomahl.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwpvlfjt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gppxjknoa.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwsdabwt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gjnylscum.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbwgahpy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gapdvhtqr.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjbubaej.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/ggqdlayjh.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/givhgrrap.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzlbnlmq.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxxwtrob.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxycqtigg.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gckcfgrjn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/ghspyvwiz.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/giyfvpnop.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gesugvkta.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnerqhfnx.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gzqjmfejy.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyssszkv.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gbvdgemwt.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmbjdgsw.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlmdnatw.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gglqaxxwt.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/glmxalgjs.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gctpcelur.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gbrvalpfd.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gexwlboej.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gkrpopdau.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvehykfti.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/givcrfjlc.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyglmspw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gntevrtes.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gimlcvtpk.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapaqfins.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrphbhzh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthjeitgi.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvizbmad.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gusntgmpi.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gwkzsrozp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjoxgoch.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gxvuhazfq.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepbzuwic.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gnuqcobsd.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/ggwxqulkf.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gfiuptlou.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gywantyjf.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganxwokku.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gciqduysd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goanbaqxf.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gancrbvgx.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/goumcoybi.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkusrofva.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghrfpdqwc.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdkxkllc.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/guyvtnfcz.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdogwpyt.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwobddbma.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnngzzpq.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/ghnimkusn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gjudmxywq.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gkfdtudsn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmppudekk.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqqoucsbt.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gfskecbmf.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gckxrhtek.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiwxdyhg.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/ghwvihsev.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gcayiwgnz.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gohhbgfab.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gxujwzoxf.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gjxztdfvv.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprcbbule.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfajytjng.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/geugbapgy.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geawgrnzc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gylzmagnj.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbzkxiqe.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gjjvitxuv.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaeuvawxe.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsrlvhzrq.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgetbvlb.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gltycrlmp.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfmkxdau.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggyosszdv.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gtvgzextg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhgdarnm.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqqumufzb.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelitbgzb.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdprfmjww.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gslvubryf.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnnubgfy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/grdpblhnj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/glkungwwa.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrwgpleg.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gwdzkjkoh.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghejuurav.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtxbccbl.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdkgwfgb.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gtxksfcix.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkujgdyp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfkaahdr.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gfikgeids.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrgugjbu.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gswbnskvj.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkeggfkvm.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gdqnpudyt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gzmxdieiw.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/glpejwmka.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwxzsdst.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkoyprif.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvuitdwu.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgjiallj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggepiuytu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gryibzhdh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavachhdt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcqeafswb.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhjvgtow.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/ggzhweird.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gnulrypau.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczqzfkjv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrnxazsb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gearfpovp.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcqgvild.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gdrfulfdk.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/ggvhgvyix.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/grroxeyay.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzokcgzjf.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gaxuvehda.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gajpyfyqi.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gdgjxqfcq.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxdxngru.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgdsgubg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gynumnmnt.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevnqmolp.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfusfnrj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrhaoobx.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/ggfyguztw.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gmxqeudtx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfvnymka.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gwjatqsuj.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbryqjlza.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/greoftnxy.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gtcedslfn.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpzaqpau.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhqdztgt.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gpwcootec.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gqbwjqsmg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gnpstlaig.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyrtsvtf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjflvxwmd.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlpnavhg.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpxobjlx.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gvtgavxbg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbvocluz.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gmmtayssn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gnursuuce.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnmwcnxc.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlmrazxd.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmukiaos.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqslewcl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gixfqvelo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gpcbyraev.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gfompkdeb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gehmydcay.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gpccrehzr.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giibataoa.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gqkgsejuv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcswwslck.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpbwnkox.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgyzbsfp.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gnqhzmyyi.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdkwsuwk.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gqmljqkzg.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/ghkvlekiy.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuzxrgtw.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtitvrdul.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/grpckrjsw.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjueyngh.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gwopzsvbf.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/groeyvjwz.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxkzizxy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gonhsnjne.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcygtvex.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gsglehnvt.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkqqctwo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gzwipyyyk.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gtdiodaha.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gthikwkng.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gpoajfacc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gmrngtohm.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiyokctj.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gyonsmdmu.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzfvqwoh.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnutgzhzx.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gglylzdyz.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpzniszb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gsmtwypgv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgmziuxw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gghzgopbk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjvspkwd.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwndexwo.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdktzpef.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gxhamxwrg.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gosaxqwke.sHtML


<!-- 参考信息 -->