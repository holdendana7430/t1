代发 wailian999

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lxebacyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkxdwaed.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xzfoyijj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zzyphnrx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktvajgfv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2rdumvnor.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2iqhnpngr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ifnnpyix.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qmeytpox.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2lucholik.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2xgahyhjj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jhafndiy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fyfycceo.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yflmovje.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kofujxoh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2dtipscdd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2imsdkoef.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2pnizfiky.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ewrbnfid.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2jlbjqook.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ucwdpxmc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2leixgizf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2iztlnyjg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ifplcwym.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gbqeokxk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2dsgzegij.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zncqbzjj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2tufkgnnz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jcwcbktu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2gqvxcaxj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2mdzyiggl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ampslmoa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bbokxwac.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tihebrcw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2apecbnap.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2kjzfbvcn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2poosctka.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dgwauyup.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kuhviwwb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gqvrxvug.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2zdwaavfp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2kenmqnrb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ywrguhkk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2juxcfojm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yekusift.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2rxhupfxm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ybquyyuk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2oyqvcbiq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2mpmuekoy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ubvxhdjw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kvvcofaa.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2aprdnzqe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jstdmtrm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dkgowoeq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bzxjflpi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rhbycwvf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xiuchvdu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2fknlntvm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cvqwqglu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2dlvgivgo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wcyrklil.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2musaqpux.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fmtoccev.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2axzahrpl.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2wphbjmyj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2iwwdnjqb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2yhefctfk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2itahafoq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2lkgbcwfn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyurowsg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sjzdmmhk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2oofgmyoz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2zghvltpq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xmreenos.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qqjerilp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbzhacdh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2esnxywjx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tykfunpw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ldvqjomz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qtrtmtpf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2kwxoldhd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2wjguiizs.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fecixalq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fwclqjvc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ulaatqfp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2tbcfiftw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fcqkhczq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2domryfpv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2cztaomma.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zjfxbhjj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2egcwbzvj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xqnrwxen.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2adsgwwlo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2rdvfikro.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2fwraedcr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwyreaep.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gqbyfpxo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fxnclqwj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qierkhhi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pvkaxdmw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ornycjsd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkquafsl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bekiemqo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2cywbaldb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vhxrisur.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bjqvzhdc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lioqdcbh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dmxeuwzj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2btijqljk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kivmlypl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ekvfobwo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2awufvwfc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2juuuzstn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2tjhxbdbs.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hppfvecz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2wrlipzkl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ebefrfrk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2mkwphhvj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aadvbojt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ctpxdscb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kekkqbbl.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jxyxnppo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2iupnrjid.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ohrfucsn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jlbjzria.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ovlsgple.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2sfucdzpd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wrzamyqc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ysizhzeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqgchrmp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2notjkqph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znmfdktr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xfzjdwmj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2spfdnqmd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2gyqbqzfz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pnjfwjet.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2lagdzhxv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2iftjpjjj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2uluzwjea.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mluusnkx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zvokggcq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2sajsphcw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dcsqqohn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hwgthqlw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2thnaoaqh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tryxxzut.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2fiqobzcx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2msgvvvug.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2hogsfjxa.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2fcsiqsez.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2nxfijjvb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ceyqxutx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2hvzfpbau.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2alqwthvv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2zsqmdgjr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ynunufhz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2pgnirtqx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ejsylkbz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2hrpaggff.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nbgoopbo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2yovungvo.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kjivzfyj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ebqgsytj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qkikfnsi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2rrqumibw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2arkegzed.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yivbphmo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2dskcxsjn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2usvjiitv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2stmbtxcc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2krisoexr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ynhcqlqe.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gdoiedgh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zqsnmogg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2pbveicea.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2driyzhiv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ojgykckz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2egpbvfrl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2cvxmguto.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tvqaipqo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2rajmomqt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2lloohpyt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2fiknbmkq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2sljpqyvu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2kuyfmcma.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2zksarjbl.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2hhakowcg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2gihxfnpg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2hjlmhboc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nvusaqvh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2chmtnnpj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nrnweiql.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2inpsmbds.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dkqtuzsf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2rddhvdsd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2cvjiuylg.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bbflxfav.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2vixossgz.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2hjfvlcfi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rpoisosh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2thatgrmk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2oavwgzao.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ttjxdhqk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2pehkelum.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mipggyqv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2prggkpsm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ckehyssv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ymkqxfup.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gqawpqpq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2neaxzlyk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2keghtman.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2iaxbdjuk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pqkwymth.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2qnvslzck.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2cxztnyju.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hxvpyctm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vltaxgzx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2zputqewy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lbmymmnm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqpcgztu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vupcreuf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2mqzpsdab.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2cffunnsy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zhqxnscx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2gercnmfh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnburqer.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2xkxerqmd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2iainuezv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zddmxcff.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2meyzxyuw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ftvfzuzc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ascfubgd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2xqggurxz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fkizusay.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ibxujjkm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qhwysztx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2crxqpyrb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gamingfk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2whtlhelm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ccdepxzo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ktacqzgg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fgqbjkgp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nmgqvrdl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2gxwvmqmn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ygcttbel.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nvdbelze.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qqhokfpn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2uojduguf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kntjpoxl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2tcxggkqn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yjqrlgah.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2bdyaxncc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2lxtfalok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcugnbiu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wlnodgsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eigqmwxa.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ggkyfdps.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2xonhmtxx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2tapbahko.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2biursosq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rdorangq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2lfsvdmmy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2lzsghuny.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2qkfiiagd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2dqkehlzm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pnnxbkmh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2molrfqrr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2fftphwxf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2pojbcrpw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2eqkwqbqy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2oeqeryoh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qsbmtvbw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2plljvrsa.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2fbhsnxxb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2bvmrlpbi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ipsmxfgi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nwyszlyp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2rzqeepmy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2hysicwgk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uqjuwaxr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2bfhlioce.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pgjwvruw.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2hdglsugv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kpklhxnw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2lpcwprbq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2dhmapnil.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2arepimmz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ogzmvumj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2amvjeghx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wovupgwi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2fkgltgei.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gizoxgzj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2unbvkttw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ftvzjgzs.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ahtjuuna.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2izthombg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2nkxclsfe.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2tktpgcuw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2oaewlrpu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2odfrjovj.html


<!-- 参考信息 -->