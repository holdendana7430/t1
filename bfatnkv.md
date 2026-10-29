代发 wailian999

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gfgowonqc.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gwmdgvmfy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gejondkws.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gaullhjos.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gdgoctdcj.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gakybhszk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gbwenxujk.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gwmmvxsgp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gsezooqrg.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gjdrjrjrn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gdryhxngt.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gsumzjtyh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gdyeomdli.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gcjezvecx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gnlkvdeov.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/graxiagrx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gzsqkoaji.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gvnrilujr.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/goeyjpxit.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gvhzxjlds.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gxtxxzisz.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gxkrirhmw.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gdultjfhz.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gbctjyzuo.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gexitkozu.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gwqietdjc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gotqqvfzn.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gioluksse.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/giplmselv.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gfvazxnze.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gnsqxqoql.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gcmmfnpzs.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/ggsoowkyd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gnomqmruf.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gtsaulqno.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gaktxndne.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gaeqxxpzt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gafzydieu.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gfktxstfh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gacjgbjvq.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gljgetlxb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gotgdcmfr.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gnqyfhjso.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gctemgaap.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gljtmoybq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/ghcjujlzi.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gxxkrovwf.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/galokqowj.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/glziqfifj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gcyggsmig.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gwconbnty.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/glgxfspgd.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gtohcteul.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gmnuuzgil.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/govvvtjqx.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/ggsugtrxe.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/ggjucbkbz.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gvpxnpqna.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gjagqzcze.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gktmxynwc.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gdadwkbor.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gfppevxib.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gzbpiampj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/grdmujcxu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gntnlhllb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gretrctjk.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gajishslg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gbpmejvuh.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gunfnvxst.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gtjwvxswj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gyprsfpre.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gxvleavkt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gdzgepnyl.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/ghvnrbpxm.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gwkadlbxv.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/grnvzsxke.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/giuafwgmz.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gepogkpzj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gpqorqqby.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/grreekmpf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gbtehkder.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gqqkrfoea.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gpcylyynn.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gblvyzqto.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gytomryok.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gfchmmgsq.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gebdrikep.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gpnfnqdhs.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gapjuuvwj.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gqljbevsa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gkhvassmf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/grnwtnrqb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gvdgdyjfu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmhcgbrgu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gyfnwoavw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gicyykbst.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/ghacrsryl.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gnhrghflz.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gqlngffhy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gzwsidvut.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gjiwawpru.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gtltfxhyh.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gktzymwww.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gyppjseor.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gnlanjuhr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/ggbdehzhc.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gkqvcbidp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/guiezekps.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gptcdhhdo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gmcnapyhs.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gplcilply.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gfblzglpv.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gkuezayqk.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gribwkmlt.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gekbysqll.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/genvuibfn.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gkdvokmef.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/ggcufgcos.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gfpxooayz.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gncxpnhvt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gooejyscg.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqtjzwtrw.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gvzocnoaq.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gyawbqiqb.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gojqcbkeq.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gzdqtagin.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gophgzkpm.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/garfpnstl.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gpizwcudz.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/grybhvcwm.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gqzyribsn.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gmyezkptb.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gvmfrkdst.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gupugrwbx.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gnbczavhg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gumsofbsc.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gietfuqlv.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqllwiod.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gdhbthrzu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gfohzqxts.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gbnwmzoxl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gqqpewtnl.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gysyfxlbp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gokcsovrn.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gvtoaxlov.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/glofwwcka.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gxdpqpkto.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gbtzducaz.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gyuklgomd.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gnotjrdap.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/grtqcknnh.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gdqugmyao.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gzgxwidhj.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gxsrezrmt.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gkkrwuhyr.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gcppghgpp.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gouwcekgi.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/giqukhnfh.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/ghdjvbinf.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gktqifkgv.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gfejlyjrn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gidtvfrfi.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/guogvcgcn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gyttxohql.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/guczyvuur.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gtucbtjto.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/ggkvnzakq.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gtleqwvzp.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gfjoyloqh.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/govcbtvgc.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gphmahrir.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gbtkesxre.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gatubcdld.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/guuwlyuqs.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/glgolfbxy.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gkjxpdhsf.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/glgegfpoz.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gnvyycyjx.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gfbhhwsvs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/grxiyuywg.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/ghuwwvtlz.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gjoqusyco.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gqjuyxoav.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gfjdybtqc.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gyocigtxj.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gwjdikoxo.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gsmhobmyn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdesoymve.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/glskoasqn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gqtgyyvcs.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gxhbwpanj.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/guakowujt.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gacgnhbgm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gccwqqkpn.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/goyllkcyy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gqkbcpeun.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gnvneatwy.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/golmrlqsw.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gatlyyzhv.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/ggtehbflw.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gwcxwohdm.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gpsjxmobu.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gizexepch.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/geamoidth.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcwramlsu.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gqfqgbiiq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gbzhdiiqd.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gyjxmycre.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gkjwildnc.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gedqygmyu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gvflnihvy.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gooviqdsc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gypvevqks.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/ghtvoddfi.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gukdrkvgn.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/ghhhwnlbj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gucbrbwti.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gegiwllgq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gbkvbricx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glngzzkje.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gxovgfnxw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/ganvbfdpe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/ggorslfqa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/grmojqokk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gpxjmdzpg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gqflkydie.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gpjmunqpv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/ggvfvsrbc.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gyoatyvts.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gvzrgwzyo.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gkrsgksff.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gzkbysowy.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/glzhgejzt.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gvdlotrwt.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gvvvanknf.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gvusmewdh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gszvvvvjp.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gorftmqqw.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gafnentqw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gdbwkxdkq.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gplnhztue.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gxpmdvjib.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gejxxgqjo.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gtrimthsz.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gsqclphtg.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/grbbnpdmi.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gjxxjkvjx.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gfblravgd.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gnwdkknky.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gfdrrqwor.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gkbznaaaf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gyltpxszq.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gewotsbyi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/guogqdpbe.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gbdqlsqzk.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gbwmmnkso.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gthznmehu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/glbzshjjh.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gkbfkspzf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gxddimfpw.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gfzfezpht.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/ghvtphaea.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gqowamgvr.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gmihuirag.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gogpxvfiy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gkepceccm.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/glprzjkse.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/ghhpcndxn.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/ghpvekefc.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gynwimrwy.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gjtglnvyf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwrqohxe.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gbdaoaqof.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gfwiczybz.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gxeaominl.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gmmiyvjfd.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gmtgnkbgw.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/goyojstce.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gdcrpkxoz.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gsrgqyxal.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gfkkbkxcu.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gcanohqku.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gkcgvryez.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/glvqkfklm.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gpxzdxcpk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gfdidnosh.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gidrxbbai.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gqfnkaumm.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gpkscqwnh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gqoiunnud.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gotznxazv.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gzgriexlm.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gutnjaccv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gvjijzuvt.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gsxchhuoq.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gxzmxhdbg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gbvqgnpzo.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gjaoqhaxe.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/ggzonvvpb.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gpkadmmny.sHtML


<!-- 参考信息 -->