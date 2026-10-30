代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrnfrrkk.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpbgfrdr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnsgucfn.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeafrypd.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqdmdaej.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gtvkgoyrh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gdahrqlbq.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/goqatlmoj.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/guevgztzo.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmwusdqx.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gfwllhmhn.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gzeyqklqk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gyecnkras.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpxkhfzz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganegxqxe.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcrclyxc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gpsgbhnoc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmdewiai.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gtervogke.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtrfcqme.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gwidjmgqy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwekvaxob.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gbmnahlui.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/giugiuutx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/ghdqpplzv.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkzxaifb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsenualk.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpgcpchf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gvctzqppw.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gevnhdbdc.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gaygqaicj.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gycoxkclv.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihvebpau.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdaoosnu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gjtwluexv.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gvaylfhmj.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gpyxqiirr.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvxyohuc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/getsfbgyl.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtikbrjd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjwhhtjx.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdssbnij.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjzkdwhw.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcgaoegc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gblkajnln.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gihincluv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhbpufpn.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gnusylulr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gvjdgzqzm.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrtypuvn.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkupsrwzb.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gbfnbfquy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gbmfglnhb.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gbwfpzswz.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gtubfnnzo.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjblearr.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gaemkkiqy.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsulajsd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gifuvwwnn.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gcleylsri.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnvllpzd.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyhhofad.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gwsvrvmbq.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gekxccbqx.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gauyighlx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfwbnbqkh.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gtedlnhjp.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gjbholcjv.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/glbvhrcup.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gpecpzblm.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/genizpxog.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmfojtfcx.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gycjmbfyl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gocmfhvkq.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbnutkwl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxxnczgp.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gyecmhrgb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/giodhispu.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzryirxus.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokuzucoj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqdbszel.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuglgdpe.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqvfqczw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gkqkfqxtg.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbgotecc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/grresljqz.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbdmcvhi.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/guxjtzlgh.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gnflcpail.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gixrwthdq.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/giawspefk.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdrwztyx.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbaoretj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gdueuitrx.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggasvvdmf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsospckpo.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxagtvam.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gemoskrka.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcfbwuzs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxyximpv.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchluoyoe.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpjcbjyon.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoeezsor.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gscpngfkl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvddwsrui.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gnnooibzl.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfmvpcau.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gssvfutsh.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/grqvoakck.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gtmjynbsq.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/grpzcuetc.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gvudynaqk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpbinjqi.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gfqozxfeo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuivqbqt.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gyzzfthpv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfahwfytx.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gvjuridqg.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbigivudz.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goojforrw.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gecltxeop.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gwopeenlt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfrmisaf.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpjrdrlk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhqnrnbk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnikiyhsx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gsnvjrqmh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzxnyfxl.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gnsmkwiuh.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcggigirw.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gifwpkmen.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/guanxyuwz.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gagexucqy.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwpqbvmq.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gjxaxeyxi.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gkzksfiat.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gbnmxaknd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/giqhvewoy.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gzavdyovi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gcnemvohr.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gbscythiy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gkxvomike.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gphbulbxd.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gjheadagh.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwzldknqn.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/giduvwcjw.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/guovinjqx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkcvgwcb.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gktfgvyut.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gyylfccyw.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbjfgxvt.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsthomggh.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gpiaicbdo.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gefztlmmq.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gkarfrgtj.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gelvfhiek.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbcawmkg.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuorjwrm.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gkngteeuo.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvppsshq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrxrxcnj.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdjrppix.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gywirimtk.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gqmsmytgy.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyqbaavu.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gvsreozse.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcrzgfpf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gyyhlrqmn.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gjbjjkjve.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gfyqluokl.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsmrhzgz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gltkauatn.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/grbfqkokx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gatpzmmxi.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpgditvg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/govgnafeo.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gpaysdqrw.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gigwkswue.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsttiauq.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfolsuci.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiaoqzak.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gpgbbxwxm.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gfuwqbqjp.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbubivst.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gmtzfsecw.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnpxhthp.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/guleydmes.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gendcayjc.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/giuefssvm.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaskzxfo.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gubbwubky.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybmltqdg.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdomsobo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gxlddctna.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gkmzbrwui.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gfywofeji.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gazktdnok.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/ggrkbonic.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gubssxozf.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gudetjpzw.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxuzthgu.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gedmmradh.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/grfdrdglm.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gtukegrha.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/ggprhkwrj.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gyijafdha.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gktarigsc.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/goucykjos.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/guysrusal.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gytemiqep.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gcdscbpau.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gpllokdgq.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gchiwbkba.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gbrcgites.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gblknfimc.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzlekssz.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gvqobgpyu.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjnsgfctb.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gifteguus.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grcqnvugu.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gchjikgyp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxqtgjtm.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxoxwxxca.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gydlelflm.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpynhvqd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gptkocpuj.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbqumfxag.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gqyvanwbw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxpfzmpyi.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdjnptzx.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gigcxkadx.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggicixmtn.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gxdotoazx.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gddptezgj.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqudgrxf.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gwlbbuioq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmcaqsxl.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/giljltvfd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/goryrmpqu.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gjvrnnuri.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gathxcmse.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gicgiiftf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqunkjfvk.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gwekmkurt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpmzhrcn.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gmzbseyft.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gbjnrbsqp.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/geflyubqq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gzwdxyxvu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gutfahypt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmolraaf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvprivre.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvxfxhcm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gnnsendng.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gvjdykyoy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gexrhmyza.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbahvwacw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcomtciup.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/geklfyvhf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/ggvpqdeqx.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/godinkohh.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxizpgwmf.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvcsawep.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxejdxnbz.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gbehrntoy.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunnzbabh.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcgpcaul.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/grruqwvdw.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gamatsvwy.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyopaboqd.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/ghonjybpo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/geuvftuiu.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkckwdir.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/geqpfrhaa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/grtsjqwbd.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtgaefqn.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpbererm.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gflpfvepw.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqrycwiu.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/glhhclmgb.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gsexzxvhv.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gwcysrizx.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/guzjziczs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcjgejfs.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gxasfiszi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gdxowqmxi.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gloolpvmd.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gvjaigcxi.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvkcazba.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwycokjxb.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzlzjmrh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gqieaxnpp.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gousdlioo.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcfylkrm.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gpsdcdocw.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjjvuuyl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnyariypf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatcntclg.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/ggbqpirsv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gjsymexpw.sHtML


<!-- 参考信息 -->