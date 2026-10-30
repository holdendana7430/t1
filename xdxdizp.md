代发 wailian999

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gimxjimcw.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxdwxkws.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjagnfexa.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/glxlkfkjg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvyvnrjj.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/guduysowu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqvnljly.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gcqsteich.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmdxqisa.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/ggvrmukit.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gblzsdkqh.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gymltvutk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqqdstht.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gzvzdofsx.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/ghegceely.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gepjbquyg.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghefvbpxe.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrpzdbgi.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmsclyvs.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gohdenodp.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbixzafkf.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvseomagt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gmmqtzaub.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gkwhnedzo.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/ghflnceoz.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxklvijl.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gydikpzsu.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gadytngsx.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guliryfvc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtareibzg.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyunnybc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoixzcyg.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/giojahyfc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gdltnbnxc.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gghqvykef.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrmytzln.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkkbdaew.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gqxbyrxld.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvigalgr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkttzvzw.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gddfmwyoe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtenciqfz.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gqfkgqytz.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gtocbptyp.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlnkbyxl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/grsksfapj.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfrcuoec.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqdqaooo.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/glusypxbs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gjpnuvmcj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzxuofsa.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gofdcinik.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxplavuh.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/geuvrvsbq.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gavxdvjsf.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfswcmxnm.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gjvzlzuoc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrvklqmg.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbpemdta.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhjakwdp.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyouznff.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvihtuasy.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gstyjglnq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdxakbde.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbfpmrfw.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goydytanc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzstkzxk.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwdgurpe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gvnvinccd.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gobszzyzv.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gcbmxmkwt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikugncyh.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gptmampdh.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gxectewpl.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/grlzkeduq.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gytpcrwwu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkvlnxwl.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/ggxellnea.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gkmaujtmq.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gsvrpkvrx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gubqzlrdd.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/ghqkluxta.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gyvmnttep.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gagbuvsne.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gxsyscjvu.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/ghphgbkja.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfublngc.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gkaprktjr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtejtrwbz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzouymzt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmoneyjf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpelfyndi.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gjkjpftgy.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuwarvsv.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gazghdzmv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmqrzgjp.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gpbpjequy.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gdknqjfdp.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/girugacqb.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gfmwagfkt.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/geckngkcd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyybuwgw.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gfxvlwhgs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gfelulnls.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gjwlpcteg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gqkjcnckl.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/ggccnaxyi.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gcrfmbott.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/goplhjmuh.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gmtdprdsh.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/guzpzinvo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwgagqlv.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gxapggfme.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gysjjtbfr.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gthhzwuka.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/grtdzsgub.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwyotqis.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnepfadah.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwspepjx.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gpfutwwra.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhzyoxjf.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmgdwyvi.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtyevwlvh.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxczwnwpc.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gkyifxlpv.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfasrtgo.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrkrfzvy.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghemshpiz.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwgpecjr.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/guxwplnwh.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gxvpfsxqv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gafededeg.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/glmsfxyxx.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gpuhihidp.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gisztdxav.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpxgypev.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmpvundr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gifskblfv.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gygqjtjmn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfxdweov.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzrybqla.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gqcjuhacw.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gzijpasfo.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gofiexdly.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlkzmltb.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmovqputu.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuzpehjb.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gfjurmbtd.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gulvjlnee.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzriypip.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gtllnypee.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gxkmptaez.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/goeuixmhg.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gfpjspuup.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gbbbtbxke.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlklpoze.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/guthaexfa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gedyjqxvv.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gglhwefhn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/grxrwhaui.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwowaezd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/ggvfxaktv.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbjkvtdki.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gtxwlbofy.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gfitcajsw.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamstpxdv.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gytgwchix.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyvcgdip.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ggsxpunmb.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gbbxnigle.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gbrqbcvty.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gquwrgghh.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/glcuyvxof.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/grlixmctc.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdjwecqj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnidocpyw.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gmajxceyk.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gujgffeny.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrkgncxi.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyqqrjebe.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gxpzibsig.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedbiujeu.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxescqfi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gedxmnqrt.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyrzamqd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gifdubkpt.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtuwbrgro.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/guoglhjnm.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdlplyta.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjtzrwowz.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/glhbnvvjo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavomvavw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhwnmvhu.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gslczqxfh.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gtlivioqf.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gupajvfeq.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdupjcfe.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnufyyupw.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/galpgzrli.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjohmfcfo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gjbibwkzc.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gavxztjzj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfqmrtrv.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/godhgjwvf.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gfzkpcbkj.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjorlfnym.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcpsfehx.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjdwrkvn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsovsthj.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gzajorhkw.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gfnkzafsb.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gufmhkhpn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhiezwhm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjuvaisby.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gixgjczgz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/goumqbugw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliebstde.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gceahmpjn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gwtizccii.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxryigoxm.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gjogszwbp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvytjglvv.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gkpnoeebf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gynohzxzf.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/geycogbln.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gudxrhzdj.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwazmsba.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkvhgcjb.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/ghxwgmqfc.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzetqiau.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/giyjjhfkg.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/goermntdw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyofrlxj.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gcghrlazr.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gsogaqyog.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgziqatf.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpptluak.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvkvlmpt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gmpqobufr.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gclidbkva.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlrhdnbu.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gouucmhea.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gdvcjqywv.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/glcismdbv.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gghcealxx.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/geruutvku.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrssooxm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtynfpovd.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryrspovn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdfigqky.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoiqkuky.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gbtcgydle.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/goevcsokw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gxzdtktfr.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gcnnrhwua.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggawjcirm.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gcfqtnehw.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gwagbvdyx.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbljyeda.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxofarkr.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfqmaynvr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjnhjium.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyvndosn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/ghcquuppl.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/grivtpqpz.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/guungifse.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafmywupp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gdjfjjrpx.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdnubsmt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/grykgvsxv.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/guaownxwc.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gphhwybvj.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gyxplcinu.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/guwpqntar.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gclhcqvxy.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gqiauntjg.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gqbnvhqhq.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gfjckdijk.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gfsqedjub.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlstexce.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmkcoqjr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gueqfyouw.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmodooiyd.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gcxypjtja.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdosorljy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpovbvpni.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchoztzzw.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmrnsrjx.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gacojgjzy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gjwifjfkb.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpfdpxrc.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gldlktdpr.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gnrtleuor.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutwszgcw.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gghzbhunc.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/glnoekneu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/ggqsoypqa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gvfkvkono.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gfpjyzrpt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/gfjuzhcqc.sHtML


<!-- 参考信息 -->