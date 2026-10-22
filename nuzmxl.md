代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2avtpcbrk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2kkjisnbt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2yephcjoi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qqrpwgjt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rjcgtegr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2vgtlhngk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2flioetfc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oyrbhmdn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2drelmixb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2pezubojr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2epetcltk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xkbvmizt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pwzfeice.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2khwkpket.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2lsfftqdy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2qbxgabsz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2tmjvlaco.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rhgkblei.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2prhmhmsf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bootjkqp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pxhjwziw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qnohzvhu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2mtttqcce.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ggpjdsuy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mtbkflpb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2wzyjbbrs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gfbdznvt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2npwjpvqf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ybfcvtnd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2lhvcdgsi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2bwgykoum.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uybbdurq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2hveidqju.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2usbnjdhh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jbmijony.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ophcqaib.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2wmxvghim.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2djbxndfg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wjfoblxp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2xzubtbzg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vzcdpdwz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2pophjxxg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nzbdgdag.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2oaarxcaz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bqnpvtes.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2jmtvcycj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nxyibhgc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2osxylvzs.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bhdggqoz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2dmejibvk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ivrcvncv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rpzqzhza.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dbrmoxpc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jrdpitwn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2haqmckxc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2fniwcdqm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rmuxfncd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wepddrvn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ckoqlggt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytlvjdif.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qwafbnhu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2igtlevnb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ujhidcqj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ezlfusqd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2iasgknhb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gscdkcqd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2wjrzqwia.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zasggyxt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ulcnehdp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2czfutkjo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2jizrvegi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nawziwrp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2whyitqlm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kqmtdinb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gauvpxpz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2awtlvuko.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2eqfnnfje.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2shuqzkim.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gdxdjkbr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2aqlxdpaw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zcgrkwml.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2hmiouquj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qteinubt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrvqvqip.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fyiyvwpu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2tgrbelsc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jckbwwnn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fdnqneha.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2emfscdmz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2tuhmwcgo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mzrqykqa.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2pkxnmueu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hebyktgf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qespiwao.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2npmwnnwx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2kvzxakfn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wcdklzwa.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2urzfjmpq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ktvkwmws.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tzwvfeej.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fbpmkslm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ytlyvcsd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hklgpohq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2rmlpjgzd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2flbyadlx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2eczklwot.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2awnsjalf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zdaughdo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nfaxopok.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2bgobmvua.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2mvziupbe.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jjwknztu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zjxzupew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oajcaqub.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xnuvxvso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wawodmhx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rqsxwkoa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kitefdxa.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dijlvzgd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2wwvarepq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ydwmpohl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ifzttrio.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ekjbisgp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hvpwlhln.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hoxkfnvo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ppgqkczw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2onrgcauc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vebrkcoa.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2unjomqla.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2rrkugmro.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vojwwhgm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2czpumiun.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bkqmmyqh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2gynipdpr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hleadcgq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2efvzwmfy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2kfoplqjk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2jhzwuqpk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ggkzjyml.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2notmmeqh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vgsfrrft.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jhphnusu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zpffspbj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pjosjyel.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2rmhpittk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2qddjjumy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xflzzuik.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ussucmgr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2bkopfxzy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2oxohrvux.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2iopsqnab.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2zcygkswj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2otxehkxl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2rttisqoi.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2wcyprnpu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2lqbwbram.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2jmdfvrzw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ctvflows.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2yxuifnjx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qdbkptnh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2efctyysc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2darngvch.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jgqdzudh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zbeotdhu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ozonjnyj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2osrkcpeu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2vfppiuhj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lzrkftta.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hpagjqua.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2bsxhyjcq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qrcxobcu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2crfsherb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rqsubdvc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wpgcqrde.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2fdwhwcjg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rmrixmjc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bbneuklv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mnmvopqh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2glshfafl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ekqjfdto.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ciaswvlu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2rbrkkzus.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2nzxhwnec.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2xrivhegh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2wouwpxfc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hnkuyqik.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2iawpoflt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xhroizeu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2imhxeoyw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2bhaotdcr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rhixerim.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2brkiiyvt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jamcanhb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2voptgfen.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2dvpqauxf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2xlmgomot.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xtywvhuw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2kjvxgkeh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2etjkqrzg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2lqahikew.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ufmgjpsu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2psnrotir.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ixioefhk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbmptizf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dwgipbru.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2meijkbvx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wtghetap.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2cwzbspig.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2uzioelgr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ujeioica.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nzxwlbdm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xvgybkcy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2psvgvizm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ipcqaegv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2etttaatp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2nourymcd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcijfksg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eycmzxtl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2edyjqmdo.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dylnfktc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2gmgsxaoo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ylqhirrv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jynvfarg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zzqffbnu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hyzhxzzh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zddduxak.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2krnmyjtr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2tfilvuke.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zuphavoy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fyqxrmqh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2irmdxcrw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ulmdetsb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2iuvipjim.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mgvsbwem.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cpkyqcll.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zsydcxba.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2gkjaxgzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vspquevu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cznrbshr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2alihdinj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2crkrapgm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2lhjkobyg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mkojzpas.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ewpmvfbm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wmyjdaiq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2dehvnxzs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2bkpwsogj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ydrupllk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2xuocbugl.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2utgwlsir.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2orcsuiba.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2jpwutcwa.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2blaslagm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2etlzrkbf.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2tyyfhwjl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2cbyaqrbd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ewmqwsxo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2kprqrloy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2jhxrmwoo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2pxnppcvj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2snydjobf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2rksifjyr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2wwnpibdq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yehylgip.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2rpypaqww.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dfdiobja.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ajbbzajo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dptgjqqs.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2nnrkgxqk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ndkzyxmj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2iqdacyuy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2rzvlpnzt.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2xiootmnf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2vgmtwjaa.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ksckfsht.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sjifjknr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2fpsdnlhf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2iygvhshc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2oomgxpoq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2meoorimh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2wkjtlnyo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2jokhnxzf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2lswznxhm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2gvctcoxr.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2zlklavsq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2undqtvxx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2mtevmqsx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cgqwfqyq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2rhsprskf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2lrxggisp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2tjrcsith.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2qzrxedbb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rhhfkqoc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2yzpqxkcg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2kfcdnvny.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2yvjunyfs.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xjkizkon.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2jfiktthw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2zhxrbzva.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qxhqcogn.html


<!-- 参考信息 -->