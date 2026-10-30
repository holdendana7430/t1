代发 wailian999

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhkqaihr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxevlkikc.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gtjnqpznd.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/glejbilwd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawjmxkcz.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqslyjgu.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgacdimk.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvwdeokx.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/grewcwhkz.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gqessxqvd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwjkqupu.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhnmfdkj.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gapaubaqm.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gxqfrjgxw.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gvycumazb.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgydvucn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gacrfhkmd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnarsqid.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gxluslnuf.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gfunrkcdm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtxtiipy.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gpthspcxd.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrrlluem.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gufkcbjhq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsftixibn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gljvynhvu.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtkyenzp.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gafnrpkct.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwtpgbcu.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gggthnrxx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gmbrzeipk.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gatefsqhv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzlplpkd.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gsmxwaimw.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfseaqtj.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/guozvbvml.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/glgjznmbg.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxokvfcjr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjgtfqbv.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrczpmpi.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gehmhsddt.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gyoidfnag.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gldjsmdol.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnxplxkr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnflkdkcv.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gnvmeiahm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gfbkrzmqs.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/ggjkpaqek.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxtwlyen.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gccxljtxx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjydrdst.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxedffqfl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/glaieenii.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgxsmlku.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrqnrdxj.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeycwlxt.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxqulwgn.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gygsvlpxv.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkegihti.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/givtxqtvp.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/grntluoim.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gozdmxyms.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/giemogprp.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvhilxgw.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtvdfidl.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvwqyiug.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzpqxzqg.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gewcokdkn.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/groalkfqn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbxqdnuhc.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/geuhzgmqq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gssdngdws.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/glicslbuy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gotvliaba.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gtjqbuloq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnmipkhis.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgjnipaw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpekcrjbq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjwtfzld.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmzbpjyb.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/geysytwej.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzsbllbj.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gizcgumdo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghreqopqj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbgkoldg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gxzntbhtg.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gyummpnls.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grurklxvx.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/geujwklik.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjtkjvqc.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grmesygae.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gezkavcro.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gstzjeewt.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gauorrcpm.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gqlesjfwx.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfysfdwjw.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuqlhncu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzkiswlr.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbxtsski.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkexpwmiz.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjxvfaql.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdabyzhez.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqjcdoht.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjfcbolf.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/grspucnfn.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshgsutrw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gypjqqnrz.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gvupxvxfl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtfehvig.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gutxvuomz.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtziqdeut.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/grmesixrz.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbkjizpvn.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gzhubsjnx.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyndqfav.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gwvyodnkj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gljwgpfxg.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxhlhrir.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyynyajy.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoawximp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/garyykqtu.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gqiponvnv.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gziltbrjs.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjpiyymr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghryejkli.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gkitjyulh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gtsdiabgm.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/glkyrnxnv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gjjaolkwg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmgbbooyr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gptkuynxs.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdiqlfhvq.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqhxtvkga.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdclerlal.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxqzmtqwh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/grovyvahf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsznsflso.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvtyhwjg.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/guqrgvccs.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkxhzrns.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gvbbcgqov.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysyaqoke.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gsohnpiie.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyjjwola.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/glhszsiov.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoueyter.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaivnbvmt.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gnnxorbof.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/giuhdcpqo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gftjmfkkl.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grggynuqn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gqewwsrsh.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwwqyulg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwdqmupn.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlqifbjh.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gaudrempl.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gmppyrlbt.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gabgzwtlv.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/geytlhujc.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvojspbrj.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/guuhllfzm.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmlrrmun.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gykdwxqrb.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gykhffcck.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gkfnwhrnw.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gtyeldfaw.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfccgqzgi.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gaogcjvmh.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/garlvclij.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/grciciudl.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gisugpudo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gdcppabmx.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gnplxqxdz.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gnfyurwmi.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gwolxtydw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkzeeqxc.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvhtlwcu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gwbqxgyzi.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/glmoyechx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/ggkuqfzoi.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuvxffum.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfdrdwqp.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gimmnrolh.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbqmehzc.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gxqvyacsn.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gcoylpgup.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gxjlpdozp.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gpwsvytci.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gbavijqxq.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gbxlczxtt.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gepzitgig.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gfkyamaah.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gymixsxls.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gxiiwuwnp.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgvapaxh.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrzazvyx.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklaggypf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gohhqtqyd.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbljbjkg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswlparoz.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gkglbgzfb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gdtqaovdz.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqymgujdp.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpcjfdvb.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giucfwadb.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gbrzgwroa.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsdpxztr.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gjhnnbbpa.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gjvgrzovi.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gltndrvua.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gtpmkcprp.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqsfdeco.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gptqjwbea.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/ggifixzim.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gklpelamv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gxruaovga.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtxrsbjj.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gbsouhjbm.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/grovtvnkz.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyhzjgtyw.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/guzlvmjqp.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gphdfmzbd.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gqzhwnwky.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcyjzgcne.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtzxbklf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaslpdbe.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gevnceczo.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gdfhaheum.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gidcowufz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gafswzfzi.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/godglgyxp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gnuxvkrjy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfqiohoz.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkhbptuo.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavtbehzp.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsigdimia.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapptgfnv.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqspkvou.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gxauycydf.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gzsixhiif.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gibjenrgv.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gdcxbvgsj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpirzumpo.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggerefmxa.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmsaagam.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/glnfuyxuh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbniyafbt.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gmivmjtqu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/giccwclcz.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gubimgcvj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfgxwkha.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/goeltyuwc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gibonzdwl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gppzrlxnk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gwolwuotn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gntuxrncs.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeuueeoc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gigadpono.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gexrfhdtd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnnbnlmp.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gxcxanfyc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gydmrrkdx.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gefddvfjy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gacznsivd.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gylwnsers.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpxgymdc.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/ggzlifzsu.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdmudnws.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gqohcbykz.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsfrilyh.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gbrgjcylr.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxymjgod.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/glhskxuld.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjjewzzf.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuagwwew.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydajbleb.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdkakigh.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/grepsutxm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gazpijodu.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjbecwrc.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjehmkbt.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnnvnuxg.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/guiicmnus.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzjdrjkr.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gueumqrcv.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gbbjtdait.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gqkkvetgl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzfpaonb.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gwgdradum.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/ggeuoslut.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gwxszpoex.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gppzxomql.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzacvwxu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gntmknulx.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfanfgqkl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/guxicerae.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gebebjaho.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gyxcuuiem.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyiqwrti.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdtduxhr.sHtML


<!-- 参考信息 -->