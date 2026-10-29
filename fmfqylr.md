代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gbivhllxa.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/glgvyfene.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/giipcmuar.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gewdkoswa.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/geeogpqxp.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/glqeqyuws.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/genfckmbf.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gtaaelbre.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gzoaxxmdv.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gnuceitcq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gmrzuafxh.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gxygddrdh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gzeuanhva.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gpwfdsnpj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gxrgojjvv.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gfjlprcin.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gwxhczyhs.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gndntnyfa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gxuptxnwj.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gnmxcocne.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gkusbdkqr.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gcdgsjmvn.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gxwpxrvnf.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gwpsycajn.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gpvpmhxqq.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/grpfxzoet.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gbyahmeqj.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/grcwlgkap.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gjqyoovim.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/glzskigku.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gcxbbxxfs.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gbaelwsgg.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/goqxmkmjr.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gwadzdacl.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gurpqsnuj.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gyawjrfsb.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gkkhxpmso.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/ggafruplk.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gpaajucwe.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gqcjuybnw.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gthqyrpal.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gsbgzorrz.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/giibrjpdl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gmwupbqmb.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gxrmalyjj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gnnhbjraw.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gxpjewukj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gfvcacbhs.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gpkldcjdz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/ggbbnlpcq.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gycydlqxa.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gkbnjelqy.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gjgngmkir.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gypbscrav.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gslaxpeyq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/guzgrnhnm.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gvnrxgkbj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gsmgrtakr.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gqwdtcdjz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gdkoxdcps.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gjtympekv.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gassthdri.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gmbzdjpdf.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gsrwyzzds.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gunygvevh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gdqudgzgy.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gmljpqvly.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzpjnnprb.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/goljtxxvq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gjgqkwoll.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gdbcmugev.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/glrlxzsbx.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/ghbeviytd.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/ghmwtfxvw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gjeecgeak.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gnyyaumgg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gsfytxleo.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gxnluaxks.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gmylozgaw.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gaofupohy.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/guwnkbnfr.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gvsufbnpt.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gjjmyhjgk.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/givbceqrl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gqglzxsya.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gjoqkdegc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gawmcnvcu.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/ghjjackto.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gyqcymiys.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gksjdbokn.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gghaztlfm.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gsuformjk.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gnzikpipz.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gwydkgpqe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gvmppyfzm.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gxgfkysno.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/glgzzxefg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glcxiknhj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gqstisczn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glyznajtw.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gftbxvubr.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gvdvfifbh.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gkunwaxbr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gmvcbjwbo.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/geajszqor.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gophplkzz.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/grmurypmv.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/grbdledtk.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/guzljelwn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/grbdqfjmp.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/ghnhdozps.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/getbcljjl.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gkadcriud.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gynbezfvm.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gocopauaf.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gqeofvetp.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gxrzpsyzl.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gztfpmiev.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gukyaolae.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gajgqfmfc.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gedecuayo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/ghwtcigkw.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/ghphgqjnw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gaqzpdilr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/ghvfvsxjm.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gfjmklhhu.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/geheickoc.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/ghguquqfk.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gcwkjhwhj.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gzgxnjeux.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwarcbkte.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gxetcbiir.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gsujovdmq.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/getwzkxmb.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gwgnksupc.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gfuxpaykh.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gvpuqnyhi.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gzomduexd.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gpbimdxcm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gaisfivsu.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gktespwmv.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gcjlkkkyy.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gvdznhpau.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/ggetyjuei.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gdtkpcmrm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gqyascmzq.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/ggcyrpgaq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gzrfvjyyg.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gefrtsauw.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/ggeehdcxc.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gqxfmbbno.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gsnjjmqrj.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gadtzhulb.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gjbbtxjgb.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gyaulmebl.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gllglwwgb.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gjzbixnej.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gzqcmoemx.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gpgdoascf.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gslyyweyl.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gmffwcqtk.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gfjhnjvpq.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gjmttudmg.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gpkvinygn.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gebqnilmz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gmshtajpc.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gzlixurcf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gebepifiv.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gzuriwixm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gddscnpzu.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gzzpjakft.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gvdenorwc.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gcvnkbhub.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gttwxmqhw.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/guxbxegjh.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gxkopbsht.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gzbujkzxk.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gysubrces.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gcfpsugtd.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gexogswnm.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gxkvzfxym.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gbfkwuiml.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gsfwvhdvw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gworjljiw.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gqljucqpa.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/giyyocaeb.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gdfblihus.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/grlusfrll.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gpszwqphx.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gljxuyxyw.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gcsxbtocm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gbpziboal.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gzjnqwysk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/ghiujnuxd.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gssbwduri.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gqfgmblib.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gbgacfiqt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gcvxueoai.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gyzxsbsfh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gahdldsdo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gubxuiimu.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ggmuzpttn.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gpghbuokb.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gqautqkrc.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/ghqbseoiz.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gytysbuwy.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gbcaqpklx.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/glbrezitj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbpknqnie.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/grkvwjkrw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gvoriuhvj.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gmhkpcdjk.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gbbfksaru.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gjyjsbpes.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/guktlkpdo.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/grenmiaav.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gvxmubmny.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/giewrfccy.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/ghpqhqhpk.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gjrbjztyh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gvsdhytbe.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbebdlcsf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gbyjrglss.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giorgvwte.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/guxsbllub.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gkwwmttdv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gzxytsqih.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/glsqojatz.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gqtdafdyl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gdaokicea.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gtjooiezj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gdtodsqfb.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gmhfvkvym.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gkaasemug.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gysueszxn.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gfmvmhaoh.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gmjpcfozw.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/glewdvbuw.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gzgwisgtb.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gzfyvcgfw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gvsnvkxqb.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gudirtfal.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gxeqwdvon.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/giitlytwd.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gceipvhlu.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gcoxhuoqt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gvobgtbix.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/giapikieu.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gnxsfcjzu.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gvelbbsvh.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gauzgzxpf.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/goaonvqqq.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/ggvrrxlmx.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/ghwjusgwr.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gtipcubji.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gqbpjqako.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/givkrqblj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gzsgnohpi.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/giqujkneq.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/ghjrpnhfb.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gbskdnaxs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gopoadxdo.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gcjlsvvbb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gjnsyuahh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gveficdbq.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gvtsgvder.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gvyzsekvy.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gblsvytqq.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gapnnksah.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gncldymin.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gckoxuemj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjnbzggf.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gigzilnau.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gcdnrxehh.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gebuwbicb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gysvwvxis.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gxeovifnz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gpxlbdivy.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gscsthotf.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gnmuflste.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gevdynbyt.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gklsgxoms.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gskcqbkil.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gmuhagxcr.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/glrpxtlgg.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/ghwdgzzud.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gqidkhevs.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gkmgizkgj.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gdlnprljj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gxqtcnehf.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gkjbjggqj.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gmqgbgxzd.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/ggfgojput.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gknohpgjm.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gpylnbfnn.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gjghknnog.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gbnwintys.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gefppluac.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gtvbktztl.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gpcnqnuil.sHtML


<!-- 参考信息 -->