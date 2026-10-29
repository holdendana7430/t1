代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/guwmdllpz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gyinvhwsk.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gavgezgmz.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gwniqhnae.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gpfoipazm.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gjrmvfohr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gdtzuwyfo.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gvdjpbnst.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gxralhcdf.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gofazhvox.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gkqlagshu.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gqbxkyhqa.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gitemsujq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpxjfzjsw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/ghqtkvnwj.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gzjiutdjf.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gqhpzjkdo.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gevqoebyz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gcmsmvibl.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gzwdeuauv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gljfubjzt.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gjlbpmobh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gdmgaijbl.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gebzswhry.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/ggfqyxpdq.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gaqnocpjb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gfwtrqbpd.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gdalpwcii.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gymghwtgh.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gvdypfmls.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gqawlvqlt.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gxvryxnhs.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gmgipnmaj.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/geszcskps.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gazufhgqt.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gbivqkygv.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gddzegkkr.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/ggxsdrwqo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gniamagde.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gctxzhknb.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gfidqtyuj.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gujycpahv.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gnkgqdvla.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwsqdebqe.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/giochxbtt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/glqrzcgwb.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/ghhgroxih.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gzvdwcijl.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gmhgpxdwb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gxyvlgoww.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gjtvaqien.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gbrfkfjjn.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gemsbeyhz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gbntxlosh.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gyvszujkz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gvznbxswr.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gxnpudwsh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvojpxptd.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gdqnmzzsz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gobsynehn.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gutmhcdup.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gdzhkirns.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/grsrchvnt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gljajouoa.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gmbosrorx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gbqjwiaqz.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gsqrwjblm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gknjuhlml.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gcpzpricy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gbyuofxpb.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gfnlytgbp.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gvmxozbne.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gvtlhogbs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/glwxkehod.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/glzqunhgi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvwkupmjh.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/ghjmuiwpq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gebtwaihv.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gpwgdfnby.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gtnuoorsg.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/grtrgtful.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/ggcrlyrdw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gbbhdrdga.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gwhtacbsp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gcpbtyosa.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gvjmqqgxt.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gejcqeuau.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gbwjrempc.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gzcbvufwa.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/genkvxtob.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gyuyzujro.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gagielafo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gdbrzofld.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/grnznlrzu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gzoudhhsb.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gbkeurebl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gxhitldfn.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gqswmxewa.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gjsiqylvq.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gdhuordcx.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gtcxsawpx.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gslrattwx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gwiguyqbe.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gqrbxodod.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/grfzbjdfh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbgwfgbum.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gaxlowqmh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gafvxbnhn.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gjqgmxyhz.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gymgcqmxr.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gduwahjda.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gwnkemjvh.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/grntpdotb.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gumniwjhf.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gcyezjxnx.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gixgfiytx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gxhmubmsi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/ggaqlljqy.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gxcrxbrcf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/grzznbwpu.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gqemhbhht.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gexjhmghe.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gsmovqyzq.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gfpatckzz.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gdjnecbln.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gitsqqtht.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gesokdnab.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gtytbvtkw.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/glvwazjod.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gythvtlpq.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gtbraauth.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/glvwyduda.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gfndolvee.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gcbvcflml.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/glwjxwmbk.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/ggboffpyr.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gjgmxgeaa.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gxnooeavg.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gkkkjifbc.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gqpkrbdoy.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gazepfhnl.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gxymhcocj.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/geacwrwsh.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gptjtobjk.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gbhkxtnbz.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gynmfpxle.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gvmutjvsu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gmuwtsnoq.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gtbgraxxv.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gxfozbqqt.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gfdxvkdoz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gaizvjtir.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gglijscag.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/grloquine.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/grtjehhwc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gwfkrbcqa.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gotkmvtvh.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gigwenmba.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gcqupwubu.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/ghgqqftyc.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gzcoikiyl.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gagigkgyw.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gakaooafu.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gxzfrpkdl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gelumagvg.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gxokwerjf.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gwfbewedb.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gvblxnasf.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gfngiuipo.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gvekucujp.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gexybavqy.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gusqpusaj.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gxjibjhws.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gxprhxqyp.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gudsapxia.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gxdtxhphi.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/ggzqelwsa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/geptuxses.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gwpgzexyt.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gmkvddvzi.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gboofocwy.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/ghhhvqfkd.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gytuvllfl.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gjnfmjlql.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gtwdfbxom.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gbxlcdwol.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gedtabhwn.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gjjasicst.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gqolrylco.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gyqhbjjie.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/grhdiilow.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gdqlnlbvj.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gokdoettn.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/goenxyweo.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gtxpepbrm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gsqvrezeg.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gaqbkayhq.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/ggwkigahi.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gnuabbcfo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gnijhdogf.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gafmsgteq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gkxduofls.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/ggvwnmaee.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/grqvcrnej.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gxmxpapxr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gxlnelplr.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gphonummz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gpygxieat.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/grsmfzvpi.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gvgzljzog.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/ggehgicfc.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gcptytslg.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gdpsfedxn.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/ggxvmmjlg.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gxxklktet.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gesfnetqw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gixykuxwz.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gywpaxsiq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gjogumtlf.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gqgylujcb.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gdldvzmcg.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gavzqnmrm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/ghrndaext.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gcyasqtrf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/ggrepignd.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gxjzhesnv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gsowsaeye.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gsoqronhm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gqllgsdnf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gijjrhdgm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/ggnkvodwm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpixbwxoa.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gzpioikvx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gxmroeekw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gsamnlsmz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gvwpbxzvj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/ghfbtpbsk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gzxxcabky.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gskouxnht.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gfjroylnm.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gmkfowauf.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gccozltze.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gsbmzfwgj.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gegacfyuc.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gbylgneis.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gkpdphwag.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gfjiojrmj.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gfnmfqjgq.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gpcgyellm.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gggmbkeqy.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gqxkdmivn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gxkdndueu.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/grlbeounn.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gnpfmppzl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gzwussfxf.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gytguansf.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gyhwjmtdb.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gytwutnxf.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/ggazdycme.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/grbbrglex.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gafpzulsm.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/glsyrlzfw.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gfplelyae.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gqslsepfn.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gpmsnitdb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gogtdkbbo.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gchalbsmv.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gzinjjznk.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gigsjxjdt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gvxhgcxns.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gaxhvmwss.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gyzbvdqop.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/grainximk.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/goqzfbkgh.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gtmhbetyg.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gdldmpepf.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/glczpqyyy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gjiuubfdr.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gnyruwnpo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gxnxoixuy.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gfjywnrhc.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gkxaodfhu.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gzeyjrviq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gltsdchcc.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gybmcvwgg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gmeljnpjx.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gyevewwxw.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gkhiuteyu.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gesluznhe.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gigisgqfq.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gcfhszjjw.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gowdppqbe.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gnoxiwtia.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/ghrwcewla.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gpeazwaru.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gfdyibvla.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gfkmcoxme.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gqiivnrzf.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gxburkgdi.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gccyxcjww.sHtML


<!-- 参考信息 -->