代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kjkxlkkd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dypwppuh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3dnignvqf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gtlqfpon.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ubdlcoif.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3txjdyyiq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wnnknajw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3syjwauou.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tddlbphu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hfxduyhw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3kvpfrqpk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3rjopnyta.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3trumvefs.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3sjxfsioq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3heggexee.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3sqhboutp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xvnffiqo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3pvbfcqiz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3uawrrgwm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ezhlkwih.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ggxukyky.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3surlzlnj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cunfdcxw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rhmuodet.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3oyeihfdu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3bkuhmupg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ycrvjlgi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nbsittqf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3omgisqfg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wxjybrdm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3gddftkdo.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3divayphp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ogaearkq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bfqltxut.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3qdtogbbd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3oqkqqdgx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3gnmxipnz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3lvttayyg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bnnqomqw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3cxnalnjq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xavmclny.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3enhssvrp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3cemgmtsn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3oscvyhfv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3tqhhynrl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3iosohscg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3szfazauq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ayhfriiq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3uenqsfke.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cxuaehbr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3znejkhmv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3qnlremmf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uvmxaobi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3cvxhaicz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lyeekmmz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gidquoqd.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3pxsifmhs.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3epmotthu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3opfkgbyj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mqbtxgdh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wrixbpvf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3srqceplu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zdhkmnuo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oomeuuit.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ctxadfww.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3akgbklku.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xvduftvy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3desflixb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ffqypghq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tyicajyy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ftxbylxh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3udlfitqh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kcrkpngc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lfdwgmwf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ofcpulck.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rjjxgjeo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3wautcrts.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3kysocyjn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dptxjwnk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nwwimxul.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ewjxnsen.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3nkpnavco.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3nltlkict.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3takuxzlm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wocaeldc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wbkekiyj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ezpmjpqw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wedxvasb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3jheulotg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pihiceyk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3iexviyml.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmaobnls.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cclgjzil.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3uyyebsqo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3fxaafnyv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhikrkhy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ssgemnqo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrsyztfj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3raeeexnc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3uaiyaozb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wfpiqfgr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3eawoifqn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3kokmwruc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3efhhewos.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3medpqcey.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3iyzmubnc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fvizpace.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vmscihrp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ckflpkdo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vrdggumq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rhryjqur.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rovlvatr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uinvypcb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lujqeqka.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3npnhhpck.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zmmlvuzs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjoaztzy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3yqcrcrsg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3aofgqins.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jfrsmqmv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3iabodtox.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3mpxrvzfv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3waedaint.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3onlycdlq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jnsiqsbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oocqudyu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gxxqnhnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpxwohoa.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mntuveci.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cuvumgou.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3vyiifspf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3codyjoik.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3cmikulkf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ntpxfxzs.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3opwuliap.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ywsiqozi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hrkmvxuq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3oxotbkac.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zyhfvaso.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fwcnjtln.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iuexpdky.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bxrsezry.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yesfgknh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3azuokstf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxgizrbl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3aqqnccig.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3oltklrvn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dwoasxsb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3shnyblqm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3oujhmhqe.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3sumeengu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3isggytlh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3fjscgxuw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jexkckwx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vjxbqggl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3owmvccok.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rhulqrfo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3dxotkdeh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qhtmrsoq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pwckylbo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3cruianai.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rnqrideg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kuzfgihu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3kgujktbf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3dksgyiro.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3pqqkcxhr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3yyqbvplq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3jvfykhyg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3huotivlb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ckphfnct.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3nryeslle.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zhulaqbx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hrryuerj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hugtzxng.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qokdxhsx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3apdpuyxi.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3rsstdqma.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3osedxuks.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3wwaaikbj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ebhmzmuh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3okjzuzlw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3dmmvyypi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3gcasmblx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vegjogwo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3szatbouw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3sowdoejy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wzonogpi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lpkplcnz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rwmoikfz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lhazdlsi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3movbotft.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jdrvqbpv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dfhjgrtl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3xkpipfyn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3eowsztcx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3wieawztp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3tmikvnly.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3addrkpqd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3htwmxgfc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dtebhcdx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ydoqegfb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3usjeppah.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3dfwxytqs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mxjzvxwy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ejxmknhs.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qtpaedtu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3bgcrvtzg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qwatyobw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oxcbxcnm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3llskbmie.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wwasqswo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lguqztee.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wofxearo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3pssbqhqy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tcwndvyu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3gflhzmbs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hmasdyel.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvdfqxzi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zsvhotlg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjzabazz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ilofrqgq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejjffexx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3edfqjsgg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3rtglwpiz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3dqjwttmw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nloyyqqm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3igyhxtlh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ibybrsnk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3qfwvugrj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3asassizc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fkhhmwqs.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3mdkamwig.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ypaejtoz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fyjdlfdf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ffqyjsct.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3udczjlmc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3sfgarqho.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mzrjtwqv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wthordil.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3puqtnphs.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3gsrhjgez.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xtjivhuw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3joseskiw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3yfyskalp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qvglvxrz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kdhwczqw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kgupdpvm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ykcedxez.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ldjdjiaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtebygmr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3anqvmsjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbvnxhft.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3advgwxze.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3vzudzcwo.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qzwzvxpf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ohylmtwh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mjxyyvqu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dfovuwiu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3mvjoszbk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3nmzzzmon.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ggrpavqm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nzcwbgvr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3nebvjrli.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dvrwtfxe.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3wweqsgen.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3brychsew.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3evgmraqe.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3taqslnds.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ufiguacu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ezscnoll.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3rcqsxemu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3cfeztcpj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ncxtuyli.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ufuophgr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3otgqmubb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cabzoqpi.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3tosshurl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3elxbcyny.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3lxpapxon.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zdxnaoxg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3dhnfxdcm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bsxshxnr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3bqandznn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3iftsscch.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3gzyfobew.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3wlswrvzk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3dwavdrjp.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xgymyvnz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3khldjvro.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3hcnmwtjl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3crhhqngg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3lcqjtvfc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3gfsgaiot.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3weabpcis.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3smoohxma.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3pggbkiof.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3kcqahgpa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bwnxdjmp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3lllpwvgm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pjxuykop.html


<!-- 参考信息 -->