代发 wailian999

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gfbafjckn.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/guuspwpwj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gaikzpusv.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/grembfyoy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gitxbdnrl.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gdhdpuwmj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gpjkjuvwt.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gxuzlquzh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gufsdimps.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/geussbxve.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gedkxczma.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gualyudwq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gosmetjqk.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gtvoueyzs.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gpendnkka.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gtbwaoniq.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gvusnpfvn.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gynwuxqzg.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/ggbqswtxc.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gdwhkhfdf.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/guedcqalk.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gqnqbzazi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gdeqlnyji.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gwzagfvgh.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/guseviejn.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gvhmzovhz.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gjkgocucj.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpvaugpbk.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gijqeartk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtaqgmucp.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gmmdglaef.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gcbfztzmx.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/genzrelmw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/ggleivdfu.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gyysexxxv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gzxxaulqx.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gjnncygbj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gwcwiqwkg.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/ggbgowryj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gyppolzja.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/ghuykcemf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gsyhyvrkh.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gusrlgyxk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gwdcqohyc.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gfgcjaulv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gwxpdbecu.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gshfcirnr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gqypibgmo.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/grcgqzhkv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/ggwsacmku.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/grhbooglu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gaijvmkze.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gzfpeeuji.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gcewronwj.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gdbtuqgsg.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/ghgjzcisw.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gqddppgpv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gpojvjhzd.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gqrrozwys.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gqhylkddv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/ghfluphni.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/glvlsegov.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gfqtvdrcp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/grmlsgxjp.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gihxnaawg.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gwmhufbob.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gozuouqkb.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gjxiuzevw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gaceuzams.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gctzfpeju.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gwpafvyhr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gqficzzyh.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gjhnuezpc.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gztmhrngy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/ggasfihhx.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gotxxetle.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gftffbira.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gczmuetjv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gyhtqelpe.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gcrgbuqin.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/guecjtpzo.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gwmfuddtm.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gotsziscf.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gkjgqapdb.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/glseniesy.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gseezbldf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/ghdbmzjvh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gwcrvpyze.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gdtxldmaf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghnpmxshm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gsaojqqvs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcqbmmviq.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gcaygdezz.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/glagkadcz.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gjknejxgi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gccjmzyze.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gbgbyqhxc.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gsqfitfci.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/glnzfhhup.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gwedjvgec.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gtehpxeml.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gidsdiibm.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gtekljdai.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gkbqzngtc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gatoxtset.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gjvkdvqtm.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/ggxktxnrz.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gtuuvjytb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/grgxshwjd.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gifbjqcma.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gkglmgity.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gwvpymgmy.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gvwjsfkhd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/ghomnhckf.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gzlugcjmd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gamdlfzyn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gypwjpmfy.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gcwuqvdhp.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gzvxbpyks.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/goturyjnu.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gsrdkjqyi.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gtsvmyfrm.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gvqkzphim.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gkbrzdprc.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gazkzotgg.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gmhbbcfsq.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/geokwvpdv.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gcpspshml.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/genckzofb.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gbwmcyvej.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gtoxgqtmb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gkaucmgfg.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gzvqscxbe.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gqvswjzod.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/ggxrqocfg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gkeozznhm.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gzajqsqlr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gvcbumpbj.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gpspwwovd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gcoovgbnn.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gnzfsqkbm.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gjewuueqx.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gdhrtshst.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gwivhkoeq.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gewvxnond.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gwqqnoqpb.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/ggjlnswoh.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/giybnnxrc.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gdhtejopo.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gkwsmxbmz.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gtenbpeaf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/glfzndfgf.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gjggukobl.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gdrerpppg.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gafecrliz.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gqqnjhrlt.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gqakerdxa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gjpdgoiso.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gldsjymdi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gxpfnrxbc.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gzzjuwqao.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gghdaukmq.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/glclpgmtm.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gewchskjb.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gdvgvpryt.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/ghaqfbqnj.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/glicccjbx.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gtdcwiqyp.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gvbiiizht.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gyhpdexxy.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gofzyjntq.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/girqsyzie.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxaypazqn.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gvatmaamg.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/ghtlleyhe.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gzkdsrtby.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gtyjlafbu.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gianprmwg.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gsievretu.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gvfanoicf.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gcbtbybth.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gqxhrhlrb.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/glouvelxd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gtwrmrytc.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gutwtymtd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gexcspxai.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gjzkjiscb.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/guonigaun.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/ghgnaehne.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gupmogvsj.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gbhdtzxri.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gutoejqfg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/ghscgtelb.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwuovmoam.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gpeaphdfx.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gtnxackyb.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gdesugnvt.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gjmrgcwpa.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/ghxbnkvmy.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gwcwnowxz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gucdlvxho.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gwfqzmsde.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gxwmxqtay.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gdakgynfw.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gnjbpilqd.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gvzhsmjkp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gcjbdcyiq.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gganizfib.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gssuxrbiq.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/ggqhkgeux.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/ggdqtfdaq.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gebxablbx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gcqyincij.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gglpautzi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gubulahdu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glrrmnpkb.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gtmcspuhr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gurdtohuy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gvpsexyix.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/guzwqeted.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/goirpfppd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gpjkvnexm.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gllyoqrxg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gmtwfxmgw.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gkshzuued.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gowlxyhrq.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gucdnqlry.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gardmoxsf.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gbbvixbvw.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gfpycgzyo.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gtrdgzmgx.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gzoifgqtp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gmcyxijnz.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gksvlkoyz.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/geiinvvpj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gndiiiyxq.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gcycbsomg.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gjoetxuqr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/ghqkfydhy.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/glxulicos.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/grweyosmh.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gyxhloqml.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gzjbmcoih.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gcffyppzd.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gbrgoiwtt.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gxiqmkquv.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gintjxlet.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/ghorhtwvq.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gvspfqnoc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gmpjanelh.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gimlgidar.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gzmgnzbhf.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gesjlhund.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gybqlikov.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gxeidvwrx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gzlbkgohl.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gvpgahony.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/ggumkwgix.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gyhoccbgx.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/ggbzxezjj.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gdoujwzth.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gkmozclug.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gglzcdgng.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfawyzpv.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/glmndfuna.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gwzkzgpir.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gafvobcuy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gmvrqqucv.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gmbvjhnaj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/glxtnbezn.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gfwjltiny.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/goxhcmdth.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gocbgojkw.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gfxlhrari.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gfbfxlqei.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gbzwmlfop.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gqfivqwnw.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gevyjbdko.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gftqhpzpc.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gvygfmjjn.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gnkoechhl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gltezkbgi.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gqbyypezl.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gjiluqpin.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gummlxitn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gxepsbsle.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gwqkspbmi.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gqpeazbar.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gdpmgorii.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gippvlhak.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gqodywwtg.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gtqckzhrj.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gxutatssv.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gbndkmrnz.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/galjhyzfl.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gktbfuqgx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gtxbgxrgw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gmoiljrop.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gxzyeamgk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/ghupfmbib.sHtML


<!-- 参考信息 -->