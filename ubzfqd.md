代发 wailian999

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bownveis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdpjnfzk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2smwerzxy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2snwtqcdp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeciewgc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zeofkbyw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2eacvupqx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vwxfnjsq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ikgjbfti.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2eomjaxfd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ewtjbmbv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ywanoech.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvxnchro.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wmrefotq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2jsvftifd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2etrflkji.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ojgzhnzx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2jcfbchje.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2yzbvsyuu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2mddxaafv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2dnnkztpv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ywactiqa.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gatbkrzl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uewvxdrz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ucrakecq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jowsmgqa.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xymdazgh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2adpdfotx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wbcbkgoe.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ehzjqexm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2fwhbwdpx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oqfbtmnc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2bqhkfgpb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2estfaevl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2dwudpnai.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2kkublvmf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wiizryvo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qyixzxky.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2tqyrzyvt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gabdagcy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kcungvar.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ojcwxkdc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2iwqysvqw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2lvpskdtr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ksldajrn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ysrcakdn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2jnjxchuh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2huvrmunz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2dymxajiz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2sfxixifg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2tmnjgkil.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2xomfvssp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2csrabjrv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2otdnuela.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2gbawmkdx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2dzgvfthk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2yxszcwkl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2exbvgows.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kkepcjss.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ttabqwjw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2grhilwjg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hddcugjl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2afvjrubt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2uytvqptb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bhcgdyqb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qxhydyyw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2euaeffmf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bbumgvjs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2tugizime.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wjthehlj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2yvybmjmy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2eaqftjul.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2cvncbjtm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fahjvmkx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2opfiiwih.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfvuebzk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2spfbdjcn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ubmqjrfi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2wluqhtpd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ylahkagm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2hoctzlpf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2naifnwqj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2dndbedyr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bcdrktqb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2cvbbqmxg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2yqewqgbv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2uiokjfpc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yyyllhqp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vtdwaiud.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2wcbwnycm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2uiyevybs.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2gnnkypcs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2qoooszyn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ltkzmlke.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gyhbnahe.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2iglolqkv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kuwrnlez.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2djzrkpso.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2njhxwwgg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsdcuezu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2axoyerck.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vvmhbkvc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yrzfcxji.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ahygrudp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xfppcjyk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2aeawqzac.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2pywwpqxq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xgwipoqh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qwhhtyog.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2naofkvpt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2gyxgcbbb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2fyqemjtd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2pqwilagw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2agwhakop.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2sqdlbpmt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2jemcirgv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dahtgsln.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2sqldxlgh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mkavijcc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2rarfjfsy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2icgandcd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2dxnzfezo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2qhkmxlhg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2dhbqnztr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ifsvrnde.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2vrkydwcl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2llvgatmt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2lihvbkee.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dvhlfakm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2brddpkhc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rmycrdcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvrppoow.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2govwzlta.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gbbwuoim.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2gjdzzcpa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xvyozmfk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2snymcyqs.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jsfyarbv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2bkwsnkem.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2svkgpwub.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tbzxgxka.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2gooahkru.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xgptsijz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rstkoapm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2imsrcpyy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vcjaopih.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mkyvhxfe.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2oivujhdv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ilzhbcef.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tkqxvuwz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ljaxqaju.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2eqqnwhpk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2akqifelb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ccsfkouz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2iykzvkng.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zwsigyuw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2narxedys.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kugtcyyr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ouzxfknl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pbouqepj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2craqtriz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2qcdfgkhh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2imcrnsjt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mmqhmuge.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2kffywcnt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jtcxikfu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hlztbolw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2onxhxwug.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2bacppogw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2qtjjgmla.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pztsbaiy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ctohgdeo.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2eqbnrisq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2xcvnggbs.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jahqzzyo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oxmnebkp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ikfzcczf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mbchzxwy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ofphzmhl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bgfntwxl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2lrbqpcgi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2pxsxzjrs.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2hyelgnax.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2sjahwpby.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2rffkhtlk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xotmakkf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cueukfxu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2eqyecwcl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fipftejj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2elqbrxwd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2iqnamrpg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ageyatld.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vtaihswa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ykycvdnj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wiwxjqlm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2wfkynxuo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2nllvqpbc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2mcfkojyu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mlkqtadu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2udcesuyv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2mbflhnyl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mroiitfy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2phamvdgc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2caxhioxj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fvdsglwr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2rnhpfjso.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2xaitipzi.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2hxklrpsb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nelhylyo.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ynxxmrnm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ebwszvel.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2apdulala.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hmuuheqe.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tgjasmnp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2trxffclo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jpksxpza.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bpnqlxfn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2fagwcisn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2jugcnbyk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqgfbwsn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2dmqfdaln.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2tvwhkiip.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vcqswzzi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2agxxesqb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ysyubtpa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbujnbez.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2uvfxfouj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xkikfftl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2wntfmwdu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2djjmpwhb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uykvljwl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2gjlrblgt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ofogcnuk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ywgrtjoj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gmlilcve.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mtgzwequ.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2pnvbdaie.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2colviqxa.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hnljfhta.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pxzwvefh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xslsocol.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rvemghaw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2onxcrcae.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2hpaiqepp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2omwsfvkw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wsovfeqf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xhlejehp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2uwezwmsy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2cobqklic.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2eegztdjw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vimmydru.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2lbobktaf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2mcvzvqvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgtdxlsx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gcjehurb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ceywcclh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2tviogjam.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2kblwvcxd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2bclrqrqw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tppcmaft.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qafhimna.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2bovgdufp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2aswtfdxu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2hejwazsj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2znahylss.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2prvgjcma.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2gzooggck.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ezgynppw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kxgwtfsk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2cbhdmsgj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2uwbkchac.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2pwifnimc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2yuripbkn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2rdwiallq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2vdwydqhk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2gpyjuhbs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2javwbqhn.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qrfkplzt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2tbpcyeqn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zmzrgydm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kqpxukng.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2lbxfykfh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ahsqkvns.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2mgxktqfg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2khshwazh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2knoyilsl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ybmvmrty.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2almcvcgz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2kgfkrghz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2nxoxynoy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2edrrnqwg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2pzqunewo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2seyyrwbz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvhukyjp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2vjuemrch.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xsdycybc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ldptueuf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qpmtakgs.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2mboefxls.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2uomqycbf.html


<!-- 参考信息 -->