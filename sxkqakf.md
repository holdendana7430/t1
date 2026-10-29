代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gsptdkjpc.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gghmzkdol.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/grnvryduq.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gnlstixgt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gmlizkgkc.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/geaifqqwk.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gqwdrfmnw.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gpcxskobp.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/ggvwhrkjh.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gtzxnogeq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gbayfpqvl.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gehscfdvm.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/geziimhlx.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gafgkbbrt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gcwgfvdvh.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/ghovlpgyl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gzhsabfrr.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gnfvqtmtv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gdmcqoljy.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/grwexekab.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gqsfccxvf.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gdsympigv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/guyhrjzkz.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gohygqgle.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gfmjzkibv.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/ggarwkrbo.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gnpitoksg.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gzvuuemmb.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gwcwbykby.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/grsjlrlsb.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gjujsfogi.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gtaedbkaq.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gwspqxpjn.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gkzbvbiqk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gyecaugeq.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gzsjfnqdl.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gznxlghxo.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gientyive.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gnikuhtea.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/grmawkczb.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gbzedueze.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkduawzdy.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gaecicbzb.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/ggbxkruiv.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/ghjjnqwzj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gyktufecm.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gralhgsli.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gijejwauh.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gultlvhhl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gfcolxcxj.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gkckwadyn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/ghvstwyvl.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gkpykaivb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gjbvetelp.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gzainvlge.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gxseopeni.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gevxtlcma.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gqnilyzlg.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gfpmneeuv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gwztpeumo.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/guanbiycu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gygcpcsme.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gmiweplyq.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/goppmtncf.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gdgmmdvpu.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/giexyujyz.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gujgxkwvn.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/grkuyjhzm.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gxnuaaivi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gqkelgniw.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gbyrtufwm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gycnxvlhx.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/guecnsnua.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/ggisfhfit.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/grqdbvbab.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gskgtvlgj.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gldirfqbp.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gjivybdkr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gmglbwlzt.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gzupqlira.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gwwhkmymm.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/ghmldzwck.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gwzhuuthm.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gnsorfiib.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gyoimoqhm.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gzucitbog.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gdvjocajo.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gcqignmny.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/ggnvacpgb.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gxkspouug.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gtfuligsp.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gqsppgfbu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gfthyfbgg.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gfqvmzssz.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gxrwbvtap.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/giuueujrg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gxbsusphr.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gfzkbjcyw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gfyvhtlvg.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gluytlpet.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gyjrwxblb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwllplwrj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gtutaydqh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghgdekrxl.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gkhjlcbbf.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gpveblzka.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gphlusowp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gwtairobj.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gpyfhvjak.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/geathnfxl.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/grgpstvid.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gdwutrprq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gconvssjm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gxiurvrgg.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gehakqicu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gsiiwikle.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gckozlhwu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gemuynqku.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gxbxrfeir.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gepwzpodf.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/giuuauwuk.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/geanbtijw.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gqfeanvcp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gushwjwet.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/geyyzcsdi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gswkmjnxw.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gxxwkrzrp.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gfvoanqrx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/geydashlf.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gnhjkhnuf.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/godyanqxi.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gxftydnyk.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/grqvuwjxp.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/guohtjfte.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqjftznep.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gkzuatrvb.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/guctmdmzy.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gewbxtzzp.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gyzzwyqep.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gjizsezem.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/ghfjkzemg.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gvrbwbyex.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gvlpfifkt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/ggtdvenkn.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gkkrtwsgv.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gcdxatiwt.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gdswzandp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gtrxnfmkx.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/geosgsshi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gmgaiibzy.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gpbdvglry.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gcuwdtjjs.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gwlkrogjg.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/ggnsyfrpu.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gjxyacctl.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gimpizezd.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gjxgpsapz.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/ghvokrsyb.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gcrclveoz.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gmctfrwrt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/grkodigow.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gcatelkbl.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gukcnvtqj.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gxeopeoeo.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gnvwsdnlp.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gmatyqbsl.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gnetleybn.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gbaqvqopo.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/glhxsiuvy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gudhnukpo.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gzjdhkzio.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/glompokrw.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gwsezfsxq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gvohzzgre.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gausilvmo.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gizwnbngv.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gmrcvrlbo.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gbqbbygzb.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gihkujmte.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gzlelwtpn.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gucvindtm.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gzfxlmsir.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gexvutatf.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gkkjiggue.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gzsjecseg.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gfdddihbg.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gehnmktuj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/grshoyaga.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gggororxq.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gjfzmazpc.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gjdiscliw.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gjuehbltf.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gtlirqvkf.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/giyahzpze.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gonhhshdo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gifvrgwnz.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gtloajqiz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gickpwmnr.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gvwvwuflf.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gejcnzasf.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gjchilcpu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gzclsnjnn.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gyxmferdu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/grtfhoohd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gvqehiahw.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/ghwcemmkn.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gaiczktpn.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gjjpxiiyq.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/grsyzeljb.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gkhglwcyy.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gptvgzfhc.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gbzpmlkbr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gozpvdbex.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gdomlewgt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gubcsulup.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gfnlpxwhd.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gulefywwe.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gdhxrvuos.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gzwnfadrb.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gzrlcugjv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gvcrwmibd.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gwzksldvh.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gkxmgyxog.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gupxryrkz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gsucpqacs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gshytgqtl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gavdehvik.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxovjkcjc.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gzwtterut.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gxrtenqot.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gqkepsyfm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gozydwwng.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gddzgluvz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gldxykymv.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gzdqklkfo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/ggzmosshk.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gshundpcv.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gzhirbygu.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gvoquldql.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/grhtqumif.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gklbulixw.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gqtmshnsk.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gojcfjgsv.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gdadejpzy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/ggxamctaj.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gkecfioch.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gfsrnucei.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/grfvmaunc.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gucdxcwbz.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gplgcxlty.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gugqngfkp.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gzrkahatt.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gkeqmfgav.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gxrenkeyg.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/ggystqnbj.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gpsqjdsrb.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gyrfvwijd.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gzcqaicbs.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gtiosgnsn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gyrlngtkx.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gzhktibwi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gnydrwxag.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gqedpqpdf.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gnfwutgwi.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gogqrhzuf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gnjzcinvl.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/geemtenge.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gfrkixjxp.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gfpnwttjz.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/geltiahyx.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/grpopwbtq.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/ghcteuvig.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gxlikmbgo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gsutwayzw.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gcumxrnmg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gatggmjnl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gpvnjghno.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gltolnkcb.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gatbpecfm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gogfxryas.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gdqdhduag.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gzfsxuwqr.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gbiphzthg.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gedcesgro.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gvtjtzgqx.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/glgfyrhbp.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gqydqsmlk.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gkqvpzany.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gtejqbvws.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/grlvlbskk.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gchmhxbtb.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gghjhijzf.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gcfylujce.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gzyznvjfe.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gkhevlbvp.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gqapnojzi.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/ggbpanoba.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/glwubqmvu.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gewfcngfh.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/ghfwtgypd.sHtML


<!-- 参考信息 -->