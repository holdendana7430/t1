代发 wailian999

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2eudqrjpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sauwwexi.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ihrlvsgx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2bmopfumi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkdltgos.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wzfjtbbo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2vqwqqhlk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2owlsezeg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2cbvmlncq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2desdxcwu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nylplzaa.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2thiipnyq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ologlyuu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qippkjgt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2iurbcdeq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2oeeeusql.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ibuiybtr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lxzjjuvc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gpjrqbds.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2tudstvln.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rsyqfsmu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jbkumrkx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ixslxaml.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qbcwpxws.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2wenavucq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2frhskdoq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ltvffgzv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vwuqipxr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dnypgwba.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ailxccyz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2nhpckljq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2afczmoif.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2rtjfneui.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gcwjjtwn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2nocjogxb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ukybjhxu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eriuvgki.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gajlmfry.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dkuqqenu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jupwudae.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ftjahxjj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2idmdbkdc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dzmbbyoy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2pnwlivbu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fillnqhn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2kunfjtkf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hzlnbugr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qxufrnwo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fxnyxxvl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2eybyprpv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zvgqkekl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2zkgaxvam.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2pcgknvlx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vxhseixl.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kmundhky.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2clkokffj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vnvsqngj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2bzkbtsuf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2patynfwu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ygoatklm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2rfyysbmu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ccxyxlri.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2rditgiuw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2bntdiosc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gywgnsqo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wpoyvhfo.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2zcybvibt.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uhojtpim.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2vtfidkqp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbtyhwjp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2xvbtdohr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2cwspcfho.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2buqkxpop.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kricmjum.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ygpexucb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2zebzdchl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2jjkjehwb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uduiixpg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2yeouvbwd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eensmsem.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2pziftybw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pgmqvjal.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tsigygnz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2piigmzrk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jzzrkxxv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2htytxkhp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qctiiuct.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cyfiajvn.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2xkbozlzi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jjujdmfd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2hqfiprqg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2vlhxajep.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2nzikokba.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vvulwedy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2yryohcvp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2xlgqhpmg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2yowigcks.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zjjivzsx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2veypowta.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuicgxrv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xnhasyzk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2oddrsvbm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dysaktyr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2julswehh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2afiaziiq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mlangxae.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vugjmxpf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2nivxzzcs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gyvalqxp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ahtlqyvb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2poverfwg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ocqzulbq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2bwxgduoy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2jxohkhli.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2zfsaxxlc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2dkzcagnr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jfojezie.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2rfuvktjx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dwdxbpmu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jlreldlg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhhobzyl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2tkpgnvyc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rjawzrsx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ydztrlyb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wgavrptz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hqihbcvf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2jicqhzdv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qyvcoyaz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2znsznryy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgennpln.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pscifmga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfwphbpp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ognlkfwo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cpakwswm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ajcmazsm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2bacwrwbd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2zvsyumkn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ikalozqy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2irhqwroj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2svympmel.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qlopzehp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2fetczsip.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qvrzudbb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bmtysxwi.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hpbfeuuf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2kfsemlnk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yfrdpmzv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cdhvhnpu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2thqqvhje.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2utfjnyri.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2prauggbx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2zwqzqvjq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qwggjvrn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2efbsvdwr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xklvxfur.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ydrundcp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lmtqghvc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yaescueu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2jilmuizi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xczupxgs.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2oxatvvgy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2emlmpywn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uboxwido.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2suinlyww.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2zejawhpt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2nbcjpomn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zcarrgui.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ibehoglz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cukwhona.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ztlgydiz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hlqwjabx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2hbrijmsh.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iuewnosf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2nllvxkkz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2wdbgunpb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ngifxqav.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2syukddoj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2iuhodqqv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2pgycvzdi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fmvedrmf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2gvxacyda.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2nxdqjgvw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ivthsrtz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bfxbsvyk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2dbemuwtv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2mvnwmgwq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2hzlihntt.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2amlhvosh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rinvxuft.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jvxwicng.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2dzmmcgfz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2shmdassd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eewgzioi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ujvtjhzt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2cfcqovez.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ctapjcir.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tffbcfjj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2bflnehae.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2fukazxza.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2mbrtqodh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2cotectco.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pqjexdgb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2lemtbmrs.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2yiaxpofw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wnglrucz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2rhdriepw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wrrnlkvz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gnvuspca.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hwvzxbyg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kfalvduh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2cvfgdguc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2xyxlpgwq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2urhiiqyt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2oyrrkcil.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bnppzbkz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jxsspmvj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yakrcjej.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2qvpcvoba.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pwgjnxbw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfnwygse.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2eyyneonu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2tmupxedf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2feljlbbq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2goqbssvb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2uwlymucl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2mlnspuow.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2eobbpslr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2etdtbfzp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2prgexdsi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqpfufsq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qbanqgtg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2epjphqnk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jkynedpc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ffqtemce.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ygxpwiyh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2umxsppwd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2mffinlqm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kjtndhcz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ngereizw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2sgghgjce.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2djyfzsny.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kwhrrths.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2spketqtv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2dkawjkii.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bmeiimmz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ejnrofdm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vsqmwjqg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2gxkydbca.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yixkuxte.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mqwyjqjo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cixhehdx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2cwjvrnjs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2aloigpad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wptidyez.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hfplixmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xkiclalv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2kuxohvan.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jvotzxul.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2qulvepso.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qngqkxco.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2yrhyspvl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2yaarzeme.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2lksnamcf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2gbtpgdyb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2zqhxpkhf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ddoihxde.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2kfimfiso.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ksyrbsnj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2zfqkflvy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ptvuvjcm.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ncxgtwot.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mrmpihzu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2bigcprbf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2obezpzsg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2rwqqcdqg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ruindqsj.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dsolkads.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2thuppjbx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2tzbeqiep.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2bwoyukad.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ywidgezq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2bqceshsy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2kbkwjuxo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kuleetvy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2oxhuxnvk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2vwrtriai.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wvkylofp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wwxlulhd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2nsimgtew.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2hxuhjqmw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2hbdyzpsw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2minxvpqr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2tvfwtahq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2iafrinuj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2mudhgspz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2hywnquoj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2bfskzxgs.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2tpkjjpbi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2rqrnegat.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2vcqezfxq.html


<!-- 参考信息 -->