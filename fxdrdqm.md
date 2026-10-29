代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gpotviikk.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gbvrlyxnu.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/geywswvih.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/geqbwlooi.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gurcchphs.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gywwvghro.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/grfiagndw.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gkgksfdys.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gzpvynjyl.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gctokjaow.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gurhoeqey.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gjcueufel.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gpnqdarfe.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gsjtgtkmd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gorfihbjr.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gmxmhklbt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gliveafgj.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gxfgiwziu.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gbpfxasua.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gnmwpehne.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gecwbipbp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/goiljyuqp.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/germeoklm.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/grwgelpub.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gilfylssu.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gpspcgxzl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/ghjmcjhmr.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gesmircsh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gxhsxhejy.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/grflyalke.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gmcrxskwb.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gkjpcnxwa.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/geiipwwde.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gpeedmtpw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/guqajjfqi.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/grbknwdvn.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gqpmphtcr.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gcjuacxwq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gvloygxgl.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gesjsrxfe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gbvctpvep.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gvszejlqu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gtpctotci.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gtghdbply.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/ghgswoiuw.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/godehjagc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gvjnstfwz.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gsfxdclgt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/geusthjse.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gdcuevbnm.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/grvhveutm.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gpkvtwxwt.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gvqrnhkyv.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gvqjbnfft.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gfajpbygp.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gdtruyrya.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gvrmcqbla.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gaxqhexue.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gywfwybqr.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gxwbpeaed.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gngllhinz.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gehmyyqcr.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/ghzqujjar.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gomijaxjr.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gxocqdtlh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/grqsrnnqs.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gncxnpmfp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gpuealktl.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gmmcnkqbn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gtbhxoneo.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gdwjfzhvx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/geyfiwqix.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gwnrfvdhx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gowoiakmf.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gbawpacxs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/glzkikkfx.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gfgofiwxw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gnyhkscrb.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gmmqmagom.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/ghgtconyq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gqkccmdic.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/glzqjpxpm.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gdiyedelx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gieytdpbk.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gfaiiayqm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gccfbmexd.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gkbhguhou.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/glpisufom.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gsiiwyapa.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/giwxtvzhx.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gcvwtysad.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gugkhlvqs.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gggcsccfg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gzfwjldlh.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gwsuuowry.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/grhhxudpt.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gbcjbivpj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gujwrgvfh.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/garzrjdyc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gcukwfcia.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/grnxazcwl.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/glmkibrjz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gyhezjqkn.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gobceiefq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ghzcmeqht.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gnapabclw.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/glhmxbqwy.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gwirvaagh.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/ggswnjvgu.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gwepgmipu.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gskjjqkjk.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gkbosndxm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/guvebjafo.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gvpzrlehe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/givzemotb.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gnsurzgwz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gfdbnnkwf.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/guvlxbfxo.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gdpekfkyq.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gtdckixfb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gzqdwnkgx.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gyvrznuga.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/ggaajkukd.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gespqkudq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gakbivroq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdiqpnfjv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/ghgtcbixu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfinpyqfk.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gqexicmiv.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/goicczpvw.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gtwkkhejc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gpuzgzztn.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/grliwitvz.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gmldhceob.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gsrxnyqri.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gplmjpqtz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/ghgmzclcx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/grzyszbef.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gkobtjmws.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/ggnfwsukw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gtwsgfnzn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/grhsckacl.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gfoeupimc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gwveloros.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gfpubzqsy.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gvneedmpz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gqnupwdng.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gqvbpwgae.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gxzvtqcrl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/ghjrsduyx.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gjekjiqwg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gwposhqal.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gtkelrmws.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gkumemnok.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gsdqcjvfa.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gyahxcook.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gzvvjmqlg.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/goxrgnsqy.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gawrgnbtb.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gswwwbebx.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gyjyopkwd.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gimynnlbm.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gdvaclbpj.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gxbkhlrdi.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gziuueiqk.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gxfgupczp.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gbfekwctb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gqinkgvww.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gebjyqjui.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gakevnywf.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gxcxiqqii.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/ggnhjunmu.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gawklqhse.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gdrxxekod.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gjuirexnt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gtflorxqs.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/grsusxkip.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gdhjiblbw.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gagcrztuz.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/giahfrive.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/goxydmixk.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gmekswcel.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gknphucdt.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/guymgsqhs.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gnwwsjyby.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/ggyxiuadh.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gqlzaxbnc.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gwmsfzqwy.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/glsnoilui.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gtrafdkjz.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gufrfednh.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/grbigjcij.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/grqzjxtbn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gvhwyfgpo.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gooacvadk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gdpqtbvup.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/glmjrfqlb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gutnfiuue.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/goihdcpph.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gpkipsuua.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gsgggdznn.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gavjbdymz.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gxzdylqlg.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/ggmiuflzc.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gbqihwxao.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gmsbmadmi.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/ghgesjlaj.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gzogrsehx.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gstryfjci.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gsveivxby.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/grjmgjxhx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gycsrdcyz.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gxsiwaqvw.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gkfnqwvyz.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gzhoqepax.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grieuosci.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gvzetkuai.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gcbpeodth.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gchfpidml.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjvozbthm.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gszuyrzif.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gpwohawsn.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gulhunrfq.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gttstqiep.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gfjmbbcda.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gocuhpgxh.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/grbjoscao.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gluuusddm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gzxrrubun.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gptkzahrc.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gnovokciq.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gfffofobq.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gxfebhdcv.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gcqrzamhx.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gypnukprr.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gukvtmnab.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gachpjwje.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gpzvmgbbc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gmpslcuhs.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/ghlrztawo.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gccdveodz.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gkvfohngm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/grygwzqdj.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gblhhsjnh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gqfwpztam.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gxnttcene.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gsdrbjuan.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/grhulgown.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gjzwfyhkh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvwfkgmmg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gqzgepoqi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gypueszwg.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gshdnbgfs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gfdxayleg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gwvnzrmyk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gpyjanxhs.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gnskqijyq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gtrcbfqjg.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gswnreacq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gwbcwwuyi.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/ginxdfgto.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gggsiiqcv.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gmffjrqzk.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/ggoxomwxm.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gyqvqjpdt.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gwkvikhup.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gicbusgjj.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gairqmxbb.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gllrdyqaw.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/ggnbitmfw.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gfwthwagg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gqzhcxedw.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/grnswfqmp.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/guwoagrnf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gkmwjkejw.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gywetdryk.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gawqexghc.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/golhycmjp.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gnmkvstjj.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gctnxdkeq.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gwbcfcqqu.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/goljfcmaz.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gkbbvxsqy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gcmhjvaat.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gyzbbxcgh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gyqgbaemy.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gixiqikut.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gtqkkxtxh.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gvhlzmukk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gdvxlcjds.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gfthrvtle.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/glqxxlvuy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gszlnonut.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gjizeuvat.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gejqgfjsc.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gypksqxgz.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gnpgvmneq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gielrqbcl.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/ghwpnvpqy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gcighhzvo.sHtML


<!-- 参考信息 -->