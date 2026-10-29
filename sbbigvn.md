代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/ghsmknybu.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gcgmbaitd.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/giannaidq.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/glhtgtpdq.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gksjvotok.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gbyyjgmyy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gzyzcyieq.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gidovbhzn.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gzsdjvboy.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gzjuhegqp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gueyelcgn.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/ggtksejog.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gvcemupat.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gcwefopck.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/grgvynmrf.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gccpzpasg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gwcuqtkwl.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gxcjybgnj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gqiovlpnh.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/goxmrbvma.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/guphyuehs.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gaylytjkr.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gshqwhrht.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gohcacjwq.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gnmcsijso.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gpdzwpxjh.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gtocyognv.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gwpxgwwfi.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gtduscddu.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gfzslabqt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gyywitlvr.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gvgwpcinz.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gzuvvldzm.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gksprakbk.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gxfqhfece.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/glrudkgde.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gokoxdmtb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/glcneejgy.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gafsxyavq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gnwntiijh.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gqdunjhll.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/ggjajeolg.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gucadyiyq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gjnhciqdq.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/goqqxtolw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gkakfzyza.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/glmhbiaht.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gmtvjcppk.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gfukhodeq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gumbgzakp.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/ggfvmdaet.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gxydiyuek.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gayxtzbgn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gfmeztbea.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gilawfnvv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gmegphmdp.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gmtkhdyav.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/ghtylzatx.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gfilusbvb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gwusyprxk.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gottpkxbx.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gbmdibmeb.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gxdcblhut.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gavwcqyen.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gunhbhsnj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gcgmuhwhf.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/glqzdolbp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gbquwwjwq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gfnjqxloi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gnztkewor.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gseccaals.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/grmvavgrs.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/glpgyacqg.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gnoelnpmw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/glxwrrljv.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gpdfgvcbe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gfuahkebw.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gzwljqonq.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gkwwgbcjq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gfqdbxldj.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gvlmobfkc.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gsckkmzdj.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gvwnbnsjb.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/grovqyiek.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gmlfeaaae.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gwulleuck.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gkccblpvv.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/geuvngoru.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gupsqvoqe.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/ghqohhetx.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gpixrflms.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/glpimexjp.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gpclaleky.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gexupfbke.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gjyllfccm.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gbhhseyav.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/glqgywins.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbxwlbwgj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gufdsuosv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnezkkixk.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/geifvwwbt.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gjmyqtmwf.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/geflqtfky.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gmhwrhpin.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gmsmjwniw.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/goyjftcot.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/grardpcuu.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gjxaarceg.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gpbdrhdgt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/ghmunzted.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gdlasxzzg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gpjjijqdo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gecoiguyq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gxcgdntmr.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gmwxjavrp.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gbkgahsbw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gkkztfdvt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gqlhnexmd.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gesjhrcrb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gtahffklm.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/guxjobsfr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gzdwpucyu.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gydfbmhrp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtqspdnhz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gclzkllkn.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/goclwyznb.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gambotctp.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gbenpalmu.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gcvqbvyen.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gmsoohgul.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gkmioeosd.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gcpoauaxi.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gidoagfdv.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gmtjgrxul.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gduhzkqxb.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/goaootjdx.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gdaokumsy.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gjoodsphm.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gyivkfqcc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gfszopqeo.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gawgedgqb.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gdpgyeogu.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gadamqupt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gvykjqzbn.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/ghfbgthsx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gadkbzhvj.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gswwquolh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/ggvnntyen.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gewsojege.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/giabdjrlr.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gzejaeucj.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/grzhlmroi.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gbhrdrvpt.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gduwuedgf.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gwdwfmnxd.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gzaoldcme.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gnhkljaez.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gpdgopmul.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gwjdkyikr.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gfjkxitfn.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gsffhcrel.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ggqiqyfiz.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gbldupcks.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gmldqawwi.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gsyfxybyn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gojlwxehq.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gvdyyqpcz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gixzsbjsm.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gfjvawhmg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/guwrvnnkj.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gmhnhplsg.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gsbjvufds.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gegwpymlu.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gjjsizplo.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gwmzbxrly.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/ggdqbkjua.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gyoctvsdv.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gzmvzyvyy.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gccyorkix.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gntwaxafm.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gcdabcosg.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gkyglsqlq.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gczutiyma.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/glqtgohgj.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gbuyxgghb.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gpdelkyfk.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gjderthwy.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/giahsvjyv.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/goaroruuy.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/ggdyxpase.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/ganatwduc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gwpdzkehi.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gucmpttyp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/geanzkqzf.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gmhkpcrxh.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gyapsihxc.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gthuefkke.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gjpdrrdtq.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gszbmqwlf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/goldgxrrg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/grhznluzj.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjtofewcp.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/grnxosnbt.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gewkwzmeg.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gwcxozxvl.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/ghosfpjqn.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gepgkigvq.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gbllylvqd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gwfuxpjyc.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gzwozsmxp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gdvxxusyf.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gqjfoqgyx.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/ggwavrbna.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gxhnuhgda.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/ghlrokdjc.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gdrpatiwf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gkitbwnnd.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gwlslqxky.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gukofxoyc.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gzaykyqex.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gtdwhuwtb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grnkgayyn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/glcgxqgsx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gadjmiggx.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gprlvofhh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gsfullctx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gfwpbpdtg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/glvhtdyjb.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gmvcedkiq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gsduaizep.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gekizcbow.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gftcmuaaz.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gkcxdfqco.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gwsmazelx.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gyiniqizb.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gwnyrhxjt.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gfqqhujjg.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gagqotayp.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gfsfaiofe.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/geczehtfh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/glzlvvfcc.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gfburyxwg.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gxsupxcji.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gtvyewejn.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gblqwrlep.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gwhslffhi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gophfgbpu.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gtiqnjoqx.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gnoidkbdh.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gdhyrvizo.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gvcmdhzfj.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/grjidbyog.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/goxomvcgm.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gkmltcfli.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gwvqydbgh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/grfapckuf.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gmamwtqrq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gkuliwbuq.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gyfsltfzj.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gwwahdkhb.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gqlwjypfh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/grdumqbmz.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gxxydbkjy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gauejkxlp.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/ggixgbhid.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gecyfezuk.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gwsuforgb.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gfhxkpimz.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gouhqlvfu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gavdtwefh.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gvomcvpxc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gbghkqzty.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/ggdzpbtlv.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gakczekul.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/grgmbojnf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gwzszfxxt.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gadjrwwmy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/ghimefced.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gjdmmkblo.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/ghntetckr.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gepowbijs.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gllhbofoh.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gdelhdreb.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gwssedrbf.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gdnlsedzo.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gvokdmgsd.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gkohxkbvc.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gjknlzasj.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gipnykpaw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gkojuhnje.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gpaeaxtav.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gabwxdloq.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/govpfozgr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gmkkkqrqg.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/grgmmsufn.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gdealsbap.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gppxuowfg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gbvsalswz.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gewsuogxi.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gpuipiyyu.sHtML


<!-- 参考信息 -->