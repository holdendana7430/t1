代发 wailian999

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gkzhlaxxj.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/grbwyyief.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjpblflz.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/ggndzfyrw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmantgqlg.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpejuvaxf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gijsugwoa.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gybvziivn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/ggzuvhmaj.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gvdphwbcc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdhhnafs.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gxiquwswm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbnynyvw.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/ghxhtvmmm.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtbejbqf.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/ggvqcktjv.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gboihnglp.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/ghuppgual.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gppmwclbe.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzvnagzrr.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/ggknmtzop.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gybmgnbnj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyyxabjv.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteusmvwh.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbzxxivg.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gjjzlrztk.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gppmkumrq.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gglxyycdc.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gossykulv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gohqixwdg.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/goeahkbgv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/goyairfzs.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gepyetalb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnrtdjrt.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwwwmfnv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxditknut.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/galdeslvx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgvjmhle.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gauxrhmna.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gadwvjihn.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gzmdtdysd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gzodfqpal.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gyljtbeec.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/grbmrzowx.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyyiwpsl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gfeseebap.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnffibfej.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gbgdqyrxx.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjkxgnqrg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/guipdjapl.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwpvufiul.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwhrvyhy.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gawjdrmlf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobrlxujt.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gbscatazz.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmhejzgea.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmtoajjs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcqunodz.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gunhxhylx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsbeamsru.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gztrcodwu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkpxtlrl.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtfxrkbte.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gokgtdywx.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gnrtqpzpq.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gglrnqbid.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gatpexdve.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gbdncxfzd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gkmdhlnze.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gstflahiw.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gulemhqfp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqberfdz.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gundgdnjz.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gafnbcqhz.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyzfcxhu.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/guquhamtl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswhvadba.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrhllqmd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gbxkaqbxk.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/giirhmrqc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyuiivzx.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gomudzgxk.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdyxqkcb.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gdgbaxgxz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzblgdjnh.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjkimjma.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gpyuffsee.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gejlwensr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gslndybxc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gckehfotv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkxgfbdr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grgbbprcd.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glgcrklsy.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbnccwno.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqijosyy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gfmotoinc.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gwupbopte.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppqhggva.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/ggpcvmanu.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqmussfg.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhozzowd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gcelbffhi.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/guymgbcfl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzmdzkan.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtjfkxjl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvfwbtnw.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/giospxtjh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqxvmglr.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gybbmcjkt.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/ghbwjmtzo.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gypzqhiki.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtdceyhz.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczdmylbn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gmwylpwcp.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gvinrtrml.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggkoynazq.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gaubbnpyl.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwolxzal.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gfhlmdxow.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gopxjaheg.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkykuadl.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gujvmxuvo.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwfhemqg.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gebnhmzsb.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gemthfydp.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzojoriw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoquodvv.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdltsgaya.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswkkqapy.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gkxpgrprr.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqqgxqpl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvmvdplm.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gyepcwsgr.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzyiveob.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvubkvtlj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrsugavo.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/galcdgzcm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gmmmraraa.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgdqqvza.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gnamrckvs.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gwvvillhm.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsvieidt.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqsnnien.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhtykevn.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gbybzrpfs.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/groupzhie.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gooaarkmr.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gvzybkuou.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyfojxmv.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwnnhgrr.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gijcqpmai.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/guybqudhl.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gkviuqwpg.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhbyxhnk.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbzwwfxcl.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gwwuqkokx.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/govjczrdq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/ggscdcmuc.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghefqwydx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/ggtswtwkv.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gwcjmoeqo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gqtcxdciv.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrcerfeq.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gwodcfpfj.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gznrufjmn.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gyzgdysju.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfpwypfw.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbkwlgta.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstbnbhgg.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqbbtzli.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbmfgwly.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/guloozfvv.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrsazumy.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvadmprac.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gqjsygvmv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscqmptkn.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gnvoydxjl.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiwdsspi.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkslhxoc.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gddyhkpux.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ggwxdsxiw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpfnkhlq.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/glitlbmme.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnawghmvn.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gpiixxjmh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqxyglwhm.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/ghcpozbyi.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/guhrpgiwc.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdusowwvb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbfxxlxx.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gphnvxxkb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiwmdqqr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gifuqxzzd.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqyimtypu.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/guscanxco.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gngnqdwca.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gszpmrbrx.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqujlajgl.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoqnhnbn.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gtuuweevg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gjoblstye.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegdrfbae.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvglgldeh.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gebnddrwz.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkujrbwa.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gqfwyjvws.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gefaldkfz.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gsaemalew.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gotcyujob.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gpbazudso.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurynefrd.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjhytvyk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gsmnwzepc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gefwseljg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxquermhn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcopiusik.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/glvdayegy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gxznecszf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gsryoxubs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsrpyrlvs.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gvacrzfdd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/grnkunyru.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/glhymshkc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gnfvbvayt.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmrszltw.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmhrvcrq.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gslepwfdn.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gpjhxohxf.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmkjxhxy.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gebtccvio.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtrtewnm.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gioabbvdp.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkonfinu.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/ghvtremgr.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gympxnkfe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/ggdongicv.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gokzgmryh.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gcflsnitk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtkgmqdz.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjteeehi.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gpdplzgyp.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsjhxgom.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmgvmfht.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndxcrvqw.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gwhjmsaxz.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gmnpizmyd.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gshyioypl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnvjfapq.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/ghqbcrwfc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhxnxlzc.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxvavxzl.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbheplqmr.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmcdufxi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/giqbsxbfw.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gewqdgskm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/grorokfry.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtdhsias.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gsspwwfuu.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gophtppii.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljpekusc.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glrpyaonv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gsehihupm.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gmznkjlba.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlislodc.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/ghtwrwbqu.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gifagllxe.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/glkzsgley.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggadussrr.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gvbkpkmtp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gaofimftn.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gmqrapsqw.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gtxyryont.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouazfxyg.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gqzbfvcmf.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gogskykpp.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesxjnuuw.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gkfbefxmj.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkyotdao.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gylbmgsvj.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gjuhxntgh.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmokxoyv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gsuhuxuaq.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkkicdmm.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gxohzdrqj.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtptpyphk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/ggaziubir.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gawldmrnb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkrjxoyc.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gfihzyilc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gqdjdqbqg.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/ghjrfoehz.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gqvrtvuiv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruhmunff.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gohwvyjhb.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtdxbttu.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwippzbdd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gbasmcvxf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtolprpg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/geqhctkgc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnshopup.sHtML


<!-- 参考信息 -->