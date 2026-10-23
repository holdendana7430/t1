代发 wailian999

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3qgrvkzyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qqlhpfuf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kzdgrkxi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wnkcyeyp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3pbeprzjp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qixnyvfr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ibmthvsr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3frgmugns.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3gpqrpumn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3pvafvtza.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jommvinb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rbopizas.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3wiuyarkx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jexrepsa.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3sztptqxi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3nwqkglyr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fhijccnr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3axrflegz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3bshuimhh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3okmkbdbd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dcyfiaxn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3esjagxqz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xlnguvrj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eglqqiaq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ygbbhqrj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ujwkukev.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ddhwaiii.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fiznnklx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kcjcaouy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3bonuywzk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ozttjqof.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3pnbzdlcs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fsdvqapw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3yegmejiy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3yxmahgdr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3zacugsez.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qzkftorp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rpndgqqs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3mizsbopw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qsifyout.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3lxwryuet.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3qjguazaz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fucigwzv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3mzhpmibs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kjsmgrts.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3wnqisczr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dlourhpk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3csglyqrs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3objqhnqk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mmrsopxq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3sllnteqo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3fkqpmijb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3elchtckd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ktpcjrer.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3pxgdbkhr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ptfxxvsw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fdyiutib.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ldboawpa.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pxoqqavn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3witowxwm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3gjeicicc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3fiakkixg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ccjpurdl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3mlbejixc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3yekrluvb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ibysxaap.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qcfwkopb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uqndpozw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jysyggda.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xszsxnwe.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3anlmhvmi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3pxgmcjqw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3oouicqdi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3dctakkai.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ioxoxpqv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ltjggmed.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3gpzpzuuv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hdfqjblo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3bhgdqidk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jiwschex.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3gajkiude.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3glzvlekc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3drowlkfm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nekvyctp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ciegeuje.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bbjogymm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3mbsxpyny.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lcxhvqpv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dfvyrrfl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3fueghbxk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3fgifuzai.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3iovdhtay.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3vctaajhp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qjqrqzyg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3cjxlwtha.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3drhogpwr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3eztqpwbi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3rpqkvmmv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rwagpfyz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kddbjwws.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dcggdslu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3nijkhisa.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rawysuis.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3pnvjwdzz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bsnwwyhs.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jqgefnsd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jxdiljqv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3mtrsubmv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iqshwmfu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lnupnzmt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3zoutakzx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3qrayhfwc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3hvqditfj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3lghgkmgr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rzahbutb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3nywigevy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3msluidkp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3tpedzpjk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mdvbgiyf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3muqnfimj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3psxbdvkm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3djiwjuql.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3krbscjpz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wqcdolbt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gwnwubuy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xituhsyl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3bvdrdasg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3uxlaagtn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zerpxjvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xigxecxl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ebcxoepb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxzjoioa.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hwflojje.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ibwivztj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lluxmrlc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ctaoxkmr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jcqaeati.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mrrloanu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3gxngtygp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3btpfuwlg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pibfaawb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zjngiaeb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vfzwrvqd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lczsywcm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tyvfohhl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3wghjuodj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3nhyjbgrq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hlyufibh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ggnttnse.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3sfsgxnyo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3dvuketwt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3bxyfghab.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3dbmwzkiz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3emksenqk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3txwngosw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3daffnwng.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ddnnejls.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hniaperf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3tenculsa.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dlqzznmo.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jrmawiiy.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ugtcksfc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3stmkgmpz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cbcpzdjo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3rcxnevpe.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tshovidd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vyalzmye.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3zxjjulsi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kqovpbyo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hlbmilye.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3xvoohmdy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pgjsizrt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3etewqbrh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fiomiydq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ggvwqktc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cyeerjjf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3wkyjrcev.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zirydxgn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3dziiffgw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3botryozn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gdzpounl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3tqziaexh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3iypgnkfh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rvjxlfce.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3osjlhtkd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3bfmldfix.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3yntjueti.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hvegrieh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bfnczkdc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fsuswbts.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3fbularpt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3svaoenjp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zgmwtotm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dvhkxfls.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vlrypqqs.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3aplmjrhc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xbpepyxr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3wlufpjau.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ngfurxer.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3acjxumnc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3pjjfwvtz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3uzedsoqw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3crorybms.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3njqyqnbn.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wlfwcnpf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3uzvtglzy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wqxdxiyu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3hbfdahon.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ypmeclnb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3firqndbc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3rkkwoifd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ovwhkpod.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tgjduhxf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3qvrrxihv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3supljbiy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3aizetbqz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zewfmbpe.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3junifoyb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3gbbifgwg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3bmwkselx.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3bmksongd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3xyzglmuu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3yodbpwsl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jxwpajmv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3bixhxyol.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3npgaofkx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3mdovsseu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3uihvundv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xmikdmdt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3unlponbg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfksdzgi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3owzrkoon.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwyhhfad.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tcckugwr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vlinviga.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jlujzlxg.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qwjzpxby.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ckjxzgep.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rwiposwb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qlpclnks.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3zzrdjdtx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uzpelcmz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3lzgrryil.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ltfzvpfd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kjqstwej.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gfxtouck.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rqasmhhn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3rwbjwilt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rdaavlqu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3aujkvggw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ntkqpexi.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3lrrwegrm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kjginiie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slijdpoj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kyntdhnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3benitvmc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qiqjqvtl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3tdwiuhlx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3mhgpzjig.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3trdpmvpp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3exmfbemq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3amlrektr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vvlonqrn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zukjiccr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qwvcbbym.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3bjzoagzt.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3rgozxknr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3mtysbspv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3zdhynaub.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hfvdumqn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3jeqmfatv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3wrcuteil.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3drgdqspm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jhsqhhcl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qaugbmfr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3asbseqto.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3gyavuksc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3smouxhoi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3vgiqzbri.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3oqzfmvap.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3tohlhpqy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fvircfnm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jxpigzxu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vtdskdvg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3evztvjwd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3wgfzlscl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3umzzzzoa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ebuccnkl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ooievtxq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3vnxdcfho.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3smfktyvm.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nuuouqhx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3qdtfmvio.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3bnmghxih.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3asakbbzm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3bczfoyre.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ghztlqms.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ojupgxgw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3bqjhskmf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3suwotkhk.html


<!-- 参考信息 -->