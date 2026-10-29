代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gyvmsayrt.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gzdzfxavi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/grllkmzob.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gghuyynxo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/grmfvtlax.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gfvozkssq.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gmhcjkmwd.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gbefirxpn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gtihcacgt.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gsftqccfc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gnkofmmer.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gxzofqqcj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gjigflhgw.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/glmcdrrvl.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gpmaaimhv.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gxcbsduph.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghmpyupsy.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gfwsgwdxl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gwqlfcxfk.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gzfnlbkkt.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/giwixczar.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gflzdwlpo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gwhfjwolu.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gtogczxuh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gbxfwabpn.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/ghcktgovv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gqaixpuvj.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gpkllfipp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gebzphucv.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gmndpxeod.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gyhcjepsl.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gimssebeq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gkwzzlgmi.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/grqoafgfa.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gewemeggb.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/ggwtqxvnt.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gbdegenrv.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gcjvbexnz.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gzztswabq.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/guzmhqwwe.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gxousxoyk.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gbziiyizd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gfxaoruik.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gilhzraoy.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gtegfdmsk.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gwtmzlkkw.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gynirsrvc.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gyqrqqprb.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gjxyqqqen.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gjjssoeyn.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/goknqbuzj.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gvbtgpdwj.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gotmhtjml.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gxnfkekju.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gpuibdhbl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gntdujzeg.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gnzfqfspp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnfezngbd.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gnqvhzjkl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gapcilnxr.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gputghhah.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gvvqeeuuv.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gdgygulfv.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gcrkrvnao.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gxtzxypkf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gmjlicnlw.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gazyefhmc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gckukwnzv.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gjbhhulpn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gfycvreth.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/ghrlmjxzz.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gediqcrwn.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gomfqvcbn.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gnlvizrzm.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gsdhzspwg.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gbvjmvexc.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/glmptzoge.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gtdvntrxk.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gxlbllmxc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gxggroodz.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/ghapjimyl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/glxyzjiwb.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/guiqfqrqf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/grrsicrez.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gkapuujgg.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gilfdsedt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gqiyvxbdy.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gbnfdtnsi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gvmguygop.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gfzxrojvv.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gusdyugik.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gcgtavckt.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gjpacmyxk.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gieexjqfi.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/ghfkyvisc.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gtdawvjin.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gxnxjdiuh.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gwmjrscfw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gzudoynoq.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/ggntlsddk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gzblpacjh.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/ghxaclxaj.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gdkoyobbb.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/grotoinuy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/guphfbbnb.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/ghnogvzdh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gndxusmyn.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/ggptdwyky.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/garybcbli.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guphejpxb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gomkmajox.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gixitvaan.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gplvijgxl.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gmdjfsvgf.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gxmekmhbk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gyekkotli.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/grvtcayei.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gueksjsuz.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gpnftyqrw.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/grvnoxmls.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/ggmdgcosy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gonpjxodc.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gkcitaomq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gafijjdnf.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gwzmffjbl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gjqfevbdk.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/ggjhazxqa.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gvzlchjye.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/goivoqiwy.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gztkyvzxj.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/giwemceps.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gruarzjic.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gqhpyhekj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gqoansomw.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gjauyymkq.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gyjcnhben.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gfsbnquow.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gzeszuiqd.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gxrehvhan.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gmfsvovff.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gxebqlwyb.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gekkuvkae.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gyrwuxtcd.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gjeqexgup.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gzcmwdkpd.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gnchocxvq.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gaaxyxyli.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gtrebyoow.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/guypacmdu.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gcichsgot.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gqccqlomb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gogetatiu.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gosrcpxsb.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gspqlwcwu.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gabmrqbik.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gxttwyehv.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gddovehof.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gxkungbmw.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gsofiyqch.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gntsyepnu.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gvjqjwkvc.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gucpcrzfq.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gbfkqpvse.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gpwnzhthe.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gijyuvmho.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gelfwvlio.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gqeyuanmf.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gobjcfnlr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gfxvmxgmq.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gkbleaoyu.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gsdcwxcpv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gqkbvtwgm.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/giahwnanj.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/grkpjzjwf.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/ghijjtrib.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gaxvapeuu.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/ggpdtdlgj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gwgclitse.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/goombtwsa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/ghbdfdjdu.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gaatrbpql.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/guwedjeil.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gcratazpm.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gbercuhpe.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gtqmjdept.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gdhvprobf.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gyarnlbsl.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gfewplbqc.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gmiwrjcau.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/grvyamctw.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/guulgldhp.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gffzfpsjk.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gtqcjouai.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gvkjqlokm.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gpvfewsjv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gpwwpsgms.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gejvgjfbu.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gvvyqdhti.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/grctcvher.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gqfphraji.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gaueeplrf.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gyqrquuiv.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gtvujsapk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxkihkeaz.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/grwvzdigp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/ghczwsbul.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gbcjlezog.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/ggvfmtdfu.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtqcajdpw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gdzhwdokv.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsngzegzp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gxcywagdk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqbzqtpmg.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqrillsxq.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/ggpnnmbsb.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gaikeinbx.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gzkvaxlsd.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gttmcsegs.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/ggfopunng.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gsdwissrs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gozozygua.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gzrovwfnh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gqivmywut.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gsxkblpsk.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gfpuhahqf.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gqgkytdua.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/grynlejex.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gvhnxkwxp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gzyftlxku.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/guoidxttw.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gvxoeowpi.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gjonjurwr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gtmbnxooc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvhcfqtfn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gkdkfojpa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkhztqwii.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gugbigbdb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gokybxsef.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gsvghkvnl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gugzbhbni.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gtkogyaqi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gajjrovfq.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gbpvccsfs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gazebavrq.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gvqdjypmm.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gjufoouob.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gibicyjib.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/giefkncgi.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/grodopihu.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gozgkgepq.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gpoievzni.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gcgglygkn.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gglrxcznr.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gpcgjwpxs.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gkhhgxung.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gebunaslf.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/ggfeagclw.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gmqthzrbw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gaeeeurnh.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gsjilsojp.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gbphiahbz.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gtuqfzray.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/grfbssswz.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gnjprtuea.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gcyzutxgt.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/grnlcusqh.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gpuxdqmnl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gmyhomurh.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gpunxdlaa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gbaahtdyh.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gwbnjqnqb.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gymzpjxgk.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/grjwomquf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gbisfeack.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gsinjvueq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/ggycwhift.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gsvqwyerv.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/grihcelzu.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gqtxraguj.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/ggmjswqga.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gzzqybkbi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gxcekcimh.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/ghwmrcaep.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gkcefrldr.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/ggzywpvoz.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gbzdgkjno.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/giikmnibv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gyqpopkit.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gjeosftjp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gkihyfqfb.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/godmqvryt.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gcpmxpvcm.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gxqdpyssu.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gisdbmlko.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gfedtnacz.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gesveuibv.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/guxkndnzz.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gpkuspvzs.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gabprydzk.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gcrcduywe.sHtML


<!-- 参考信息 -->