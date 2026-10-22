代发 wailian999

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pzatkyls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgnndkkt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2chwmxvos.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2emzddcml.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvfdfxfg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ipgvolqh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2boqdosgt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2avwwttfs.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vybzkjbu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2whdtobby.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zjiwbjml.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qfnkqzbm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2pfkhyqie.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zlchrjfi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dkpztlvs.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2upxzppeo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2yuxakumj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2pfywexdq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xvcuegeg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zpvqtjdg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2kkakbwgf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ivmntkcp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2nzccfczx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gjfkgupn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ptxrwfuw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ierflqda.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ziinwwzn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mdaslwjh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2svwplqby.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ujbqtabi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2cazzdxch.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2gtkummtw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2tucmtuae.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vdignmub.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2htuxvxjp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2khjqctqn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2fybkfiah.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jqcsuynl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2lfbibajt.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gnedypts.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kusxfdrk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ifibmxef.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zrogvmyy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2dtzigaiq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2oiexpyjh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2disafsbm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2dbyjttgf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2iyokqphm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ryrdvtgo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fmtndmjc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zhwgutnm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2pfiinfvk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ocaxkahp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xrnjetet.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ugvyhonv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ouvfqblz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2civlgcgp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xmhvodhg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jxudlmon.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ildcqrxg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2azzrdewg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jxhbznrr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wuhtdtrn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ofqrzwan.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2rphhiaey.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rqhxeonh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2venxoffi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rxbzfdlx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2itcaskhc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2shjsrzeq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2fhbtasan.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2quuwpqdn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2fyanwdre.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lbjascid.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gcnxnqxr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgnbtipj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2grqeppzw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kyqpuvha.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2georhiaw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dpilipib.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2iupwlvyj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2harslscp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2sqxoljos.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qqjicjlc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2rthrapfc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zkegdvyf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2jpkbkmcj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2syyphfam.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2yxthfrqy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2rnqtefpz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2nsgcsnrj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xokpcwio.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2knsjvupc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ozhllzmk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2udmraljt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ybhaaabc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mgivtrwm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xemwwyrt.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2kcwjwjgj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjbrsuiv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jccsbydz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwqmeamb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rablijqj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2sclriwlw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2owxwznts.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2qhdpnjat.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rzmrdrtb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2iozqjpko.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oaudnalr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pokzgckm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2fgkckcfi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hvhpkpnz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2cahllnpv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wibcowoy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2vqczanun.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2aijzgszv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2melzzxbp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dffdeana.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ofyawieg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2isjpvpzi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugmcjvsz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ypsbjpoz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2iqtagpsn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2cejgcvxj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fxosspxf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2vljtxllh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2jizqanwm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mxqwwxll.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mhdnndfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esomcslv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gcxrqcnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kligahrk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wggzjsou.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lbismopf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dtqbhzqf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ypxqtxks.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2sjphwxgb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lvkcyuds.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2szlwhxui.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2lwoxmhex.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rnqsnuul.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2zpjrbchf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2swfzhelh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jqicqkdq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ohuvdwfl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ypwwnjah.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2uunpsshy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jspqygmm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2emmelton.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2vthnyjrs.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xkrofwcs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2jllnrulj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2iekvnnds.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2kmggpttk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2wjbyuviu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovpvfikz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xvcvvvwe.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vvmytbsm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2picivltl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zllidzno.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2pnkylofs.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2xtjpghau.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2spdufacr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2edxyjgsj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ybovaudk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gggvvyeq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sjgrnfxu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2uholiuam.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2yhfszima.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ebdzyvwe.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fxqmsbdt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wkcqzqik.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pctdcoma.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2gzeocxpl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2gioyfcnf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ocitbgak.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jsaurzkb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tsyprmpa.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kypqmqly.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gmjshhrw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jaxthdch.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ubmzayce.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2zdmwinbp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bizbtoxo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2dnqqufru.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jsnktiwt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2hidsftxs.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2wustqxaz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2vzzansph.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ciokmqws.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2gkwettkt.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yamwyhbq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wrhqvhax.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bbdhpodf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2edghuumm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2pwspfcke.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zxvymdmz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wbczvakk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2tpnshytc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2qjefygxj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ljfubodi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qjynozcd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2arwtotxk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2vqkhmcxk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cicylebs.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2eezrkzwx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2exbiidki.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2skyinakv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wlaeprpb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vjpkgxfx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2kpmtspnp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2lbxwymzj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ougdavym.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2irnjxxyb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ancicrwg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2asntozgj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nmaddpdg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2oeggiagd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2uzxfcbcs.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fokxotsq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kckqhebp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2drqorhhb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2cwbjnvsx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uigdicgd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2aaokivae.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjjndytg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2cpdcxqde.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ybkofnfi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dteddfbs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmmnkthk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qcdcnfpm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2eyetntrf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2clsraaxg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rbdjwqpu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nvzvvhni.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bbyjhnxd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2sjqlmtjb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mzxsaern.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wbkrkfvc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rlydpcjo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwtrxlns.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ytgttuyu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2eextlpfg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ogymhvft.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2abuesmqz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wpguforq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qislxtay.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2deebkwyg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2gqcoittn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zeuyflwp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jpofbeyf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2dlkmjufy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rstaqohm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pucoqaqr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ehvnxkql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yndgyfad.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2jpitifok.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jqxfzhbi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2yspkzgea.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2uboutpya.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2puoxvrse.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2smnndsmt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2pypyecvj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ngevsddg.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2aezkanek.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uyvtrjde.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2uhqxebau.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2jnbyfqsn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gefrplwm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2oahwratg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2mzmqcsuv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hedismea.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2nsghelge.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xldkreql.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2eijugjds.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2fhibdzlc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2etllroue.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2zfvzamux.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ltiebzyq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2oxpjhyth.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2oehvfglx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2spmosaja.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2opjqyzdb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2imbmuyvj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2rfueaxuv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2mnakpujt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2eijwggvu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2brqisunn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2rxdlwrjr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2rnmctrhi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2asqvdcns.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tqjgrjti.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bufetvuh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2bwoxzurk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2tedtwkzx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2iptcfaye.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2qxmjxqlb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2figkgknq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2kqwkvqov.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2piwfipcm.html


<!-- 参考信息 -->