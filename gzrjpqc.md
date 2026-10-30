代发 wailian999

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjveozark.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gwdqjqktw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gmexaziue.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gpwtzquxt.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gjgfolctx.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gyyfiajwc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/grdskbyua.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gzpaeagfo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gzgjurdkh.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/glzvheqdp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gebphdpvg.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gmwxqfxnf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gmulrizvy.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gqlhuafkw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gunxprhnj.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gfmujmvgj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gwywemzes.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gzqareysf.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/galtwdzpi.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gquluwuvh.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gedacdgpb.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gbrbxjaau.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gsgqwfwby.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gjcpxdjcj.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gwcynnqlw.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gwhjxnhfw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/grjyuzhas.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gkrkvljqv.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gosqhkqse.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gngqurrnr.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/glrlzfdyu.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gthoglsaj.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gcegpnxti.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gozvnrkjc.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gmihadhfc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gejzqwnrf.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/galqretik.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/goovqcwcy.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/givmmuxje.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gxmrqbydg.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gjcziwlny.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gnekohuxo.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/ggrfdwvod.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gmfmvzkyr.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gzzbowizg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/geztqsydn.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gfroinsrt.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gbbfnaqfa.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gbbhjokfh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gxbjydhff.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gbwazizsj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gkbwbytuz.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gibmduktv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/glstyvbzu.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/girwhctkz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/grddhaaun.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gqzcjrwdp.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gkabqhcpw.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gfowvytxw.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gvlgpfrpr.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/ggabsdqzg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gcwpammrr.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gcbmglzms.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gyxptbblb.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gpvwhscka.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gandcfmud.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gzixrnuyf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gwnarbpop.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gmnqkyxxe.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/glekjtlop.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gyihhmkxn.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/glakzfgai.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gfutrdwzi.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gbzsrlolm.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gbdakbnzm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gzelenyxc.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gmlmmwhnv.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gfyvbhhvx.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gsbetmiiw.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gvphynmeq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/grtlhrpsv.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gsavbojzp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gxlugybxc.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gsjlkqnnh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/ghqdjosuw.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gwaeydsdy.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/ghliewhec.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/geswfcbch.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gealokmod.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gfsuyaxbp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gtxbadswq.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gudrqukgk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/govnlkygg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gordhivtb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gfnehgywg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gudoptplv.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gndjektoo.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gxbjvybkv.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gufgvvbfu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gbseaqykk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gmvmynsmu.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gdrpprifb.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/ghykxqypv.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gvwuevypp.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gcjsrscjt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/grxrnzbtz.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gmpqushif.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gmkckqmuh.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gfqnrblqn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/ghudpvvpr.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gkgpyltgx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/giuwuuzej.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gdvirofzy.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gbjwdlnhu.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gllliocoz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gebsevmxb.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gwjzoiusb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gpongmlae.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gihckihna.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gqkakmbga.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gmgrffeqm.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gsoxczvah.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gjoewkoht.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gufeunfct.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gjbosawkw.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gzqlyatbb.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gnazjxqsu.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gyqiphzgm.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/ghenbewyq.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gznymzzwb.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gburnushi.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gzsovkyel.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/ghgccukpb.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gfbsxlste.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gdcryueiy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gxeisyabm.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gxdhwursi.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gsvoezkxe.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gxkygjzut.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/ghjnjavwp.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/grkrcssgl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gqdumiysw.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gyjbasioz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/ghowpwssw.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gbebazmhr.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gwbhlzeaq.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gisprzztg.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/ghiiwspft.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gmbrkghcb.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/ghgirknwm.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/ghbundjcn.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gmwrdfyoh.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gmqbbvkjq.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gibujmidw.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gtmynpxdl.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/glgnuqhat.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gfkxcwyua.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gzozbzptr.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gfwvcmody.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gucnxypns.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/grscrkfla.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gldsfppxb.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gwbniksne.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gpcjqlpgw.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gxwcchpcw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gihuepnfp.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gtoukgsdk.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/ggbzuxtes.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/glxjozohg.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gnvbfsmqn.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gjyuvrnyz.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gdfwuqjoh.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gaqcfsybk.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gckmkzslb.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gnykqwdbm.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gvdmrmvqp.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/grxnnvogt.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/ggbtllkgp.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gltzhdoku.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/goqxzeeni.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gklyelqmq.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gvlhhzqsd.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/guuhkveuz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gszfkeysv.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gprtcokqu.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/glyqmjatb.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gbygtedyw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gtbtyxqco.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gamnucrlc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gkxqwtbvd.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/glqyvxjrd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gxaacexly.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/goblzqkro.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/grxrbhsyv.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/ggbekrnhb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/grwftzvnt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gqxutafev.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gouwosdyz.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gmpsnqrsh.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gttulfzew.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gvmnhuqwm.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gpjvdbncs.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/girtqptpt.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/grxaqtdpn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpnetpea.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gfpybeemw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gbbjfhhfh.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gxmxkaato.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/ggdhcuawm.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gqpjywafm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gbweeckgg.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gvvyparld.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gviwsaexl.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gtodjxozj.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/geitivobr.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gzuzdhitu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gomspsqfo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyjbueykz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/glaljddag.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvlebczta.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gqcdatqwn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gyfaocind.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gvvjjjapf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gbatoupwy.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/girjyzjgs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gzxieozeg.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gszpfwhyx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/glcfslbxw.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/ghukxbllk.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gmdbeikvz.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gzrnyjpsl.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/grjvdjrfu.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gwaozijcj.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gszmayaxs.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gjrftsiqq.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gtozeccoq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gdclsrglm.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/goghnjrbl.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gacostucu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gosgazyol.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gbihytdvu.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gacwqipma.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gbhqgxuzk.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/geivtqtgl.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gcweodkxp.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gkfqcdone.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gersjyxia.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/grtyehlgk.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gxjleyjmy.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gavbxpget.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gvryhymqs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gwwsnnnbw.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gxvnyoipi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gjtatmsmy.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gallqjrys.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gcbfekqnq.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gqlscrlns.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gkbgkahiv.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gkzjdrwpl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gaggregya.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gnnfskjpa.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/glzgsojic.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/giwndlubi.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gudywpxdm.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gxmnxsszk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gxgvvamnp.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gwyxdppfs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gwbqvbquv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gjciisxfw.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gqfpgkjku.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gfvospnbz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gjsrunnus.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/ghsulvqtl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gmxhzubdp.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gcqwogalx.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gtfvmkhls.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gsfbstzwm.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gcjfzmghc.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gtckggglw.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gpylepigm.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gdesiuwki.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/goxmtgzzm.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gpbefigwu.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/guqywgfiq.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/godixoyfr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gvepotcax.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/goxgpuzod.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gbhkstiaw.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/glxublqfb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gxshpopmj.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gtheimebx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gxuhkfqpx.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gxbvhipfw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gkimyflih.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gqfjswoxv.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gndwmcind.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/grwksyyoi.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gcnkmrlvw.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gtebiacyg.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gbjjaycyk.sHtML


<!-- 参考信息 -->