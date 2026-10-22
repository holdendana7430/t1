代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2zdmznubv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vaytumkw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2bblevydg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywhwkecl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ltrxcsio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stfvuezd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2smkwrffi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2znznfhie.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2enwqoyza.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wyzsdwmt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2jkjfofwj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nfpazqvy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2tjgjhyok.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ihkhhnel.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qqwazjro.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2evyjxjri.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2skcumdlb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cehgsddh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2tidnxmrf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dmiooshn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2varhwryc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2khvzmtsf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2sfnpfybb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2kgylfkuo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2llhbinzf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ooyluyeh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2twiadism.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ecyklzpc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ixbjxlws.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qpfwzobi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hfragxiz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gxwslysk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cqrhehqo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2mzntnizs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2aufxsnca.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2qsrnsghk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2yjdwerxo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zvzdwaeq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2yawcgmwy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2fybpnvrf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eeslsllh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uydzucgb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2cmcvnyem.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mwtbfbce.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2spqbtcst.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2wagkodre.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xjthyjos.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vuwqrhlq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mbglwoey.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2zfidkrgz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rzwrrqeq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jixdzssw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ufebvtqm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wvtptclu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hckawpvv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2gtxkghda.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fltvetjo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2onbkphak.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2jjkrfsag.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ckherjtg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fmzigzbe.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2nqrohvmg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lzhvpxdo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2zlntuhlu.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2lzdqhqlr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2aswbihtk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2rioqqyuf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2bqujwmxm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2kordxmpo.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2wrecopzb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wibouiap.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uecvwuaw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2dhapqtux.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xebotfmh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nhqbzqtb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ezhdkynx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2xpedzsqq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ahctnnuq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gidnhmdv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mymvxzvt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qdsqdaog.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bymhkutz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2nfmmycdl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rzegkmot.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2dydtcjia.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2hbaadavh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kztffpol.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ommnmilr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jobtslyc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2usyiaxnf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2kwjmyfog.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ytehughq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2aafninax.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2lrdclkqt.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2rauzbhzq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2noipepgf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2qewlujhv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gaqunawf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2kdahknbv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcuslvig.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jrszwnfc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2nthqepfb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2mewbvhgg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2knfcvrnk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2nspohouw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2erzkoysu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2skcoirjp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hkmyhemy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ewohacou.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2eiyflmlc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mwxhmtad.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hchapqpk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ounrteml.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2lvralqem.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fafaunoc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2svftxqis.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpwhvyth.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2vsukhirb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2jmufrdjy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ozrimrsd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hdmwepju.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2snjfprfi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2urqejnir.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2pkkcwiqu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2efpsojop.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2kmtwbbmq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2eojpqrkp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ldwmlydm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jnoyiufw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2aapeukmp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2nkoplgjj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mbcedcql.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rjupshgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2besuxxae.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ozvztaqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwjvmcii.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iahfevhq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jjjaotum.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dlfwcoli.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ibjkzibm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ibwthvtd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cfqpojmm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2kyoybtwa.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2kwcahdyf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ujaseadj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2oshpxhta.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2soopnvqn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vgozyqop.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xkvcione.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ymhbtprb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ghmhtpdw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2etcjwftt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rovgftix.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2qonahook.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2syeqvmlb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2pboljkjk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ehngorqh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2sfwmwvpl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2uzinzagh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dznzkfix.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2thefdgsm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywnpctmc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jalndmqq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lzlpgkog.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fbsbzbiv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2shotaqis.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kkrwquqx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xhttldcf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2nenbnlto.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2axgjxjqe.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qhaeuujx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2iwocunsh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2pvvmecue.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jpgcvkuj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ubdrsxyt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2azvafnle.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2zkskgjyx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2jdnzsqpp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2pazjewlt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2zjkiflyc.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2rixmdaqv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2jqzprrpd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gopohljx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tanjycaj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2tnlnybsb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ikeqrbub.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2dxoyqdel.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wxvszgxl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ahxbjabu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2wxshxhty.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2jdgcxbqf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2txbqqvjq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2owjibxeq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ykwkihlb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2vjpeyewb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gbrdwmog.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vdbtjwwx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jwfhnowx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2sehpdbou.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zsbnlypg.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pwpybydb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ffkrcldj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2qfbzyndn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2cszpqnci.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2pzelmebe.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rnelkxwf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2lyvdlmzk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2piuskavj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2eduvkjha.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ptwkxeux.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2fbewjegf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2cznolspv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gxkfbmvz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vsilkoio.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ywbhvngl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2lowklxru.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yploahtn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fxoxerne.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2arudtlxo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2luxxdnby.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ljfruuyl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ckermmxx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2lwfjrbhg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2guiwmqth.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2qskjmuhq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2xxtrhtrx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2mkcepodo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2szbsrebt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2usnevvcn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkoxeitk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ydxarrlf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2jxbnjowj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2zivwwshy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbzhutmv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ihkszkzc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2iwhamjrx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxoojrzu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rcqoleph.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ypwrmbgv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2vovxfmfa.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2skrihpww.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ddaeesfl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mkjksvwi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vunzkszi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2arzludag.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2szevoclu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghenequm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xfueoldo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zbprghxv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kajvukaf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rgdzocnp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2sgyqpllq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tejshdch.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ielhguqt.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2imdiafpm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2qnimokzp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2dwbpxppz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hlqriyky.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wyruhran.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwqecueh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xmokxowv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2vwgjewtu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ovldcsgw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rxqtrbhe.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xmkfygyn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2prpokzmg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2dsxhyvle.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2qeeakpwm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2wegpvish.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gmpnfuwl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2libtscdd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2oqogppkj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2zicdgmnp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2kyigazqm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lcrqgosp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ughipnfh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2blzqxgga.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2oygirvan.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2grhztkoa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2oiiihetr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nwjjjlso.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uvbqsarp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2mswlrapb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2qxyjlkuk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gjyccfzr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ilzybytp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2jxlhjldh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2sulppuxf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2gqydwmtj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2xqcwkzsw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2vguvuxsl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2jlvhgyjc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2boilybse.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2cvozofll.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nvtjmxaj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2axmddysh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2mnmurjtv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2pbjkiuin.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2bmgsmkkc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2fmgvvzie.html


<!-- 参考信息 -->