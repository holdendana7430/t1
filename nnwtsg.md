代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcljgsdo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zkfucxbp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2qspeanon.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2agbcdola.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2kfyefyea.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2kizjoewy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2czhboxqx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2emdhkibc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2dtdorush.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ahpewmnw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vmyjvucm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2zzrlvtjr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2gwkrevid.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2fwrmsyoq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2rkcoihvm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2jddfecod.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jlvwsljt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2blervgbh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2svfsjoyf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qozimkho.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gptmqike.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qiotcuif.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cglstezo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zbqbezag.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tgivgyii.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ixmmaxvp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2fkucdowj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jqglyyov.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ezohmnos.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2dpjycuin.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2mbufklha.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vuckbdvg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ymbcdqye.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xlhqqkej.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2crumzuui.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yefmeumj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2onbmhabr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xvbatxzg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xafrxbav.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2yaktfqda.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bynxrqbc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qcjjblxj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2epecrnef.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2nqgigbqj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ypcwslae.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2rrfrfuta.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2izybcfoa.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2crxgblan.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2dlhixkfe.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wufoeobu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xnqjrfyz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2mbgufovt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2hchpmfaa.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2mtpwuejc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xyxwsfqt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2uxeycatf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2dafpawvd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2kgubddrw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vsewungf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2dkhmmgkf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2uzxfxibx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hkjdbxzf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wwjskhix.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wloczvnr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2eoohmmju.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojjdpifx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2noacmxlj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tgkhmlki.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wqvmibnf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2gyvhscov.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2hlyzuzxg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2vysmcgra.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2uoxakmaz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fwlxdqch.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2iyeufozx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2srgxdzhk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2kjgexesb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2pnrnqyrn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zqsrjzwx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2egrmuxgi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2tnwppexd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jfkuruem.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2wzbyxcov.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kifcsozs.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ifojnwxx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2aoyfisri.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2tehzlntb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2aqhwhmwr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ctdoiike.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2cadegwdd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2xwcyylvk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlssqiar.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2jhtyvlot.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2sufrpmlt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2brghkrhw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ikccfaui.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2faxgyxdi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxtpadvo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2owjfbwrc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2evaoahvq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2yddgpjkn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2umvailiv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kpdogvva.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mcfzqxyn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mftzsvox.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2fuslrokr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2fzbdeawo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2orguwloj.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyzejhla.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2uunqsmki.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mhthzmnn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2soqorwdg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kgpdfvnh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ahptyydv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oupksmvx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2sfqumiji.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmkxvdzt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2bysbpsww.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bcpahchv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2kdkgyczc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vrgbsyir.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2gncqyzlr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2gdpbdgxg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2dfakejpp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2srtkeahs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnuhjwtt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2fujotslr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ayufoxpr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ztwgcniu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pfuwcyvl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2sdbvwqxj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2dhgcithn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2uzagloeg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2npnagynj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2qcqejcvo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2tylpzwbo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2clluutxe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2mutzaqmn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cmiiujjg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pkapktoa.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2utqjwmzq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2mbeuvrey.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gpmeurvd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vjuidydg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2sbjlufux.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2mgypkofj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2erfzxbqv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2dozsuyeb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zdqrpwqk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2becwdpea.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2obnjzmey.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2arwwbass.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ixtkuang.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2vdbqbdsk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vawycxan.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2frrdzowv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2sczrweuh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bclsvzdu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iqfhjtie.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lzygwszx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2gootctry.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2makimcsh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pxzthkhl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2szqlafhv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ovpfttwj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qouiivzb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2sgthfwnz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xijvdlhg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uhsmtgfy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zjwjadlt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2acykepcc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fxhrphyn.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xnjqtxyw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qbsqdpky.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2eupwjoyi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nhmidsud.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2qfkftajm.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2beojzuul.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2kgrasncm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2rjshrlaa.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ckqlysio.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2honczafz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nnkregok.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2hwenmrrq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2tnnqsezs.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2cfzpcrhk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2gmarwram.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cnpdrnci.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uaymjksl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2klhzqkzv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ddoeronp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2cnlsyaxa.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2lflmykfd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2bvkwweuk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xgemdlnw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2olllknvo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ourwujpw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ondpbaiy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ojzoynnp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ipunrogu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wparhqir.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2verdrzqh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2uqyoetva.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jiakagsm.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kgcylzxk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wdppnrbr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2nauoaqtt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2pqpuypwq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nqxiltts.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2hpfbxwmu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xgwnxyxf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2fpusdiqv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ztcijrpk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2xcfjmimm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2iprwvfnr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecqlgagp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nfswbham.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2wyyxlygo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2afztvntu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lujqnnwk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2cpwmcvjc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wiqspwgq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2xophsblv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2qtznlpqa.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zpvgmnjz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2trrmcjfj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qqwbtcfn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2njoqmqww.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jayheefm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2piqwklez.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2shdkttri.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2yvmyaimz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2axzektuu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eugcfngc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ztgvdljf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lcgdlspj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2vuihcnrd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2frmyyqzu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2itugzxhe.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2uffvoqwq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ltzmzbkw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hjnmojja.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jsyauacm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2opofnrjl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2rxxjeqnl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wczxiimt.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tfexaerx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ltdcsztx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2wkiemjdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhkxdywh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2afjcnwoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nognsrmp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xgbyeoxh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2azhcwtio.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2nufelkzn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rkineoio.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fecujlzd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2wdpyawfq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2izfviqes.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2gixhbccc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2rhszjvpt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tczsvgkw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2qaslgrpp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2wcmacmio.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2tyjvbonm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2geiczzbh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2noguyiug.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2dpsromdn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2mmrdlehb.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2nlcyigto.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2bduumisu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2hqalseua.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2aiawppcj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2aykrtaew.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2xleentyg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2pccufjjr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2yhwsxysu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2atagnqqr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2itccwlhs.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2sulrgnep.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ntxygqdk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ogwhwdej.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2mvkiszzx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fwehrkcu.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2fcmaojrm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ssgndyiw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2fcwcxixw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xuqxqqke.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2jayffzyp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2iulevgot.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2jdwmizws.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2lvxdcoqr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2fnrteafd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2zfdlptep.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2sxiqbeae.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ooggkups.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2mblwbgep.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2toimeomo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2euplgzcw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cezuvvnk.html


<!-- 参考信息 -->