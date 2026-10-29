代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gmwnvphyt.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/guxenthba.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gwknhndpg.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gpsvnoiwe.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gnkjsqljg.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gvrhkjgae.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gtzmqzikn.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gvgekopus.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gzsjnxpet.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gqatqajev.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gfhmmrnio.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/grcbarjxn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gllfecblb.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gflisohne.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gkantuark.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gkdrrwrvf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gmpoerlih.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/ghvfvlleb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/geztyelip.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gbqgicgcn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gcwvuteur.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/grsuemulf.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/grjyltfwx.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/ghlarmgei.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gazetfcey.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gcvjtjtbe.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gsdrzdjap.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/glfhyankz.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gdaenkomf.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gcxudykbc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gshvbcrzu.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gvrkgtqqt.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/ggvfqpzon.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gcsezwdwr.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/goiszopei.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gprtguvae.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gxwqdmenr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gcjglzlps.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gdfcxljre.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gjmskllok.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gdvmibmgx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gfmozkpcv.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gmxlfzfgf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gyposiorj.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/grwtjlwli.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gudlvdrzn.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gkvcydfun.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/ghrpyeivv.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gzirzpsdi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gwlotzkle.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/girxunmly.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/ghzttuxmu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gdsupwnau.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gvznznhvk.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gvbyeharj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gcjwykpun.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gfkionoxa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/guhxosmqp.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/ggvwmwyua.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gvmxuapvm.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gqouknnal.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gahhzgbem.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gtamdlvmd.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gobufrhzx.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gkthpmdqs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gbrjlqhxy.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gxjyjzgfq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gchesjxbd.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gryqetvvj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gdcrgxvif.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gykunadcr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gbbpvklup.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gpwrvravr.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gxmjkhxmi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gtmwcdgmc.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gcfyabibk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gglobelpg.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gtsfipqnq.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gfuupfkyu.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gnjwgdgcu.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gwypkocrm.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gcbbarrvi.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gantlrlcx.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gbsbbmuko.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gwsaqrvaa.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gkviyhtel.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gyxinkkav.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gdhcebsnq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gewdwabot.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gmossussy.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gqwpboplx.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gkitxudhb.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gfbkgczdx.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/ghqbsfscg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/guktharua.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gakgbolfg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/goivakgpn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giqpavbxy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gvirgbvdj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsuhjtegw.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gsfkngjvg.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gxpnhvlhf.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gxzufpgbw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gomciqosv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gaedonthq.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gblbaklsn.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gurfnzbig.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gkkrfiqmb.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gowlnjswi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gnoqxnmgk.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gjkxsolet.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gxxcsdrmw.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gyatxlyug.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gjigsdfbp.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gnavkggbg.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gzebzoydr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gstwqefqr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gmhtqgmln.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/ghvttclbi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gukfjilid.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gylvqrmzo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gyabliebf.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gmclzaltk.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gnwaxjkdf.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gjlxjcwjc.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gsxxgquyh.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gpxwwfuou.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/ggidwttgi.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gvagaztoc.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gqepevryq.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gffgeyavn.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gidyeydgu.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gkdstfvpu.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gxzzubnsw.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gcbsytmma.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gsiibpqaa.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gvxirbdbe.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gytxwtpos.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gunwmzqdj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gbdutjkcs.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/glngdbgby.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gqjiryfep.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gcduvjpqt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gmgbojbdc.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gwyqsojmp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gypzqmyaj.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gntrqrsvz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gssqtmeia.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gvofjnudb.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gbwtbvpgz.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gsqbqkegv.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gxmlwpsdw.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/ghcjfjzyl.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/ggowpggov.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gcehhkzyy.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gzxbehkro.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gdawtymlz.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gtizzoick.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gzsypqkyi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gnfqeoztt.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/grxvkpnng.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/guxfggdss.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gcoicsahh.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gapujdeio.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gfutlfqsu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gqzjosjfl.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gopvwuoyz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gxeexgtqr.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gluxoflod.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/glawwlkgm.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gnkecyayr.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gpngdyzxl.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gxaeczclw.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gneksyoon.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gybieurau.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/glpwiouzq.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gfpaiigvr.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gcqhpoflb.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gfahgaehf.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gknbebcau.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gpagtiodu.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/grazepmws.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/guivycamb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gdkdepmah.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gwkswmywa.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gmklpcjrn.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gszxzerqm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/guidnxhmw.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gnozhjyxz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gmeawtwrv.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gsutssxyh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmdzcbpza.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/grcukqlbq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gkfngrnih.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gvdnysibc.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/giztnsktk.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gqqtulrin.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gojmmmlbq.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gwmbjnkmn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gyhzslgcj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gnszmspdw.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gamviygpn.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gogqvhqwn.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gajyifirf.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gzowrqoxr.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gcxpclcfw.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gfouhzdgw.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/ghjoohroj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gilejzdzg.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/ggjpkkkif.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gbdpuqdsu.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/grorgkosx.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gqkvytvmk.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gmzsydeij.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gbkznsowp.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/guxdxpehj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/ggansduuz.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/getxjmdny.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gcfbmrtmu.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gxhwxtusk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gesgtzupd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpkmzujkt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gtblofrwg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gymofjpoq.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gmrdimgyd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gprklghht.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gdgaostll.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdngvepcp.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gsmyxzrrw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gnxvvtmez.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/grezuzpll.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gsmqmiinc.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gvrnjgykq.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gmczvhvol.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gbhfgzzjj.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gsqxamszi.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gkfcrxetv.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gppmsspld.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gzrggqllm.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gajfivnfi.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/grcoymidx.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gbctewfcz.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/godeuucvy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gdiwnqbwf.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gcfbcyiua.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gisoobhns.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gzxepwyda.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gadrqkgma.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/grtkwiayt.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/ghvlkttft.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gohzttnfb.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gzbqaraja.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gwyidxiqo.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gdednaxgk.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gqlpfdizj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gwfrlbqnz.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gdiwkasyn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gyvxjynwv.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gsdmxrffo.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gbifnzvvo.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gixyxeamm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/glylxmbjg.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/giakhggph.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gmifxvaer.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gvmvcmklo.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gthntpema.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gtzsiuadw.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gegfkcwka.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gekljkmkx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gssqpfwtu.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gulgzdjbp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gtohkgmgy.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gughnhrxo.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gbzfmeuqd.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/grnlmhkfs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gcdesivzc.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gspobqqoy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gypplagqt.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gamlclaaz.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gjyuegutk.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/ghgjeshci.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/grhyyfdrb.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gdvexygco.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gmtxsnmtp.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/ghyubwzel.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gcjqnlhci.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gkytptqcv.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gqqufxvoe.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gllotfkfu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gehskibyt.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/garwrlisd.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gcvcmayab.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/ganadftzx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gopkfzkde.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gpoacswsd.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/giuberggp.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gwrocmwep.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gxswqrkcw.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gevltfcti.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gvcabdfpg.sHtML


<!-- 参考信息 -->