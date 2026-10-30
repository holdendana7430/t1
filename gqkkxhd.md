代发 wailian999

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycbcwkcs.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoedyjwj.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuuwnugh.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfawxyamo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gicyxwwhz.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gsmejunzz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkkhaygp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdvihhuu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcadpzrl.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gwhiyasnd.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmweeljhd.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gerwtvpjc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/ggbpfsljo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnordnsh.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gctwemceg.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqixnbjvz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbcdinge.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/grdwddhwn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/goirxrgfl.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcieznmz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzwblhrr.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gmhwejpes.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gdjzihcfx.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/guujiadin.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfgridxp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gkttzxbap.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqkbdcnr.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohiekmvb.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhcedmuc.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gyqbszeri.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gdlhyqgxm.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/ggusyzvgj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtbtopev.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvnmotfm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gjqipnzbn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoynxddc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gadotaifa.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqttmsyhu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gcsvvvfet.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gfulbfshc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gsbermvhn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawejogec.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbdslazz.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuytjrix.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gnnvlutys.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhcueknv.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuexvdez.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhqudgkx.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjuyzfpc.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geghvbtvx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqeeafbj.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gzimoksii.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/ganmnhpsg.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqelikll.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gttqmuekx.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsqzzriz.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gqzkgxrub.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsivhmdjs.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhhcwdji.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gassbarov.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gixohrrhg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdtuiefo.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gcidkwmdx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfbffbdzj.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogknpyhs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpgyfxww.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gupeqnreb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsltgpey.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gdhrcvbky.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnunnyzks.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtburtnyd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/giilnvorj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdnxotyc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrrthcgp.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/givrztpof.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gibrcoqdd.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gylcyijkm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gpigpizkb.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/giamzrbue.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdlbpdvt.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsyqmcpt.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaxpqsdp.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvlakxcu.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcztmvaq.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhrenhis.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxghubqq.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfngoota.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcvoyins.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtllctzu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/guksuwirh.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkblxxqtr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoavcqvp.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gchdcjoza.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gepawwmon.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gmdteljqw.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gphittnkl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvoouzazh.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmurjggl.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gqilarkdo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtbhukmq.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqfphpaat.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/grvjnmers.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gcgfqdtlz.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcinhiuiz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyjfraze.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gfikabjmm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gbmtqzxor.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gfxapebtt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytxyzqht.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gqywjmqrb.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gnfxcwcbv.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gnfurfhwb.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gzbowtxix.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gxslnqyyw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gezumhaxq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzcweeuy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gjlxvphwx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grtvjzedg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoivjtom.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvwhbcks.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gllrwzwxh.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gatyuvdts.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmwtmyhog.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/glylahsub.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gitvmozmx.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gpabwxpwg.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gnzlczyun.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/glbkmfsqp.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcgaoato.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/ggelnwvra.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjivgvix.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwctkcjd.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gqbtzkpbu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcadhdgr.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gnpuvgpjr.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/grlrudbol.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwrhafvgv.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gimdvlezl.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmladhdjr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/grenphfwq.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmrmyaza.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gxqiorvjt.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/geyqzihda.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxxnyohn.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvsvmybr.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gyiqliunk.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvsqecvo.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gnkkjkdcp.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gbasutlyo.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbyxfuwp.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrhoyvgt.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gpchmxmjw.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqjsaojx.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/giwcwhuli.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyjilqtp.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gmhxbxedf.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuvwygxm.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghygxfujw.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gnlccatvd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/ggfnjdaau.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gidltozpu.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gbnrzzfls.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gfzyluezk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtontxsnp.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqconujdk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisbajlnu.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/ggtsrhjfu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvqtecob.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqytrqls.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpihivndt.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmntpxjul.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdqndqun.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkzlmkps.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzslywlut.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gyewcyufv.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gealomrii.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gqazhueqh.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gzkfzelqf.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gaiubaahd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcazoqjsq.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsryylsz.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpispwgg.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghqvokkdm.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzfwcxsj.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/ghniqklxi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbbzxrph.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gqgyoovze.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvygrcjka.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gryxctkjv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnpvyjcn.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfivgitzh.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gjmqwnpso.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoabsjab.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdatwilzx.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gsytrwcwy.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gdztoewpy.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gskfoszex.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/glqohejho.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/ginzwhqed.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gbflekzhi.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gmagdlsws.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gqojfkpif.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxdgporb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbiesfzb.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gewalmhds.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gzefbiyyv.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gqpbxonva.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/galsnmvpy.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gzlbzqwmo.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpsjamzva.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gixdzecsn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdicpjpka.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gafxmtekf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbzuixtz.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gdigqbkpx.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggownzpon.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdhydbvzs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gysgccxtu.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggivbuqch.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxhqwrzk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflrxkjlq.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjhkbgdqe.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpiittly.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gblaxflez.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gplqrvyuc.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxqxippn.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/guulbajsr.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gjglpscsd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gsrraupwu.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gzumxsnqk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/grtappxak.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlidobrt.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gfodrqlzi.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gqraikptj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/grcpavbve.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwacgxiaa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzrmmzul.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqcnloqe.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/grgchhqjr.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gzohcsnaj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gegbqmtin.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcgohmny.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gfcebnykb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gexnoyety.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gupgtvmqh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkoxkudm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gbitqfrrl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkihwnxmv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwhtzewb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gmwxgzgos.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gwejcaitj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnhekqjo.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotjcbbzv.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/glfmqlrfl.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gvvbnxrhc.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gmwbyfjlw.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqzjzjxs.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqznyfdvb.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/genaekilm.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzvmldpt.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/glgnqjyhg.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/glodennzs.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmnytxzf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/goniijlim.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/greotgofa.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkdobzxq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/glnpapsyz.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlcvlvxj.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbtnhnjx.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqncvazj.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gglqsvlvd.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjbxlamr.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesmqzcgv.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/ggkgzymbx.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gzywhdvzl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/ggnvzyuao.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnwsucow.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gzzriogri.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufgmhfol.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gnqkzaqkt.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiqtvadg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gxsxjbxxf.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhehrhbx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/godndraeg.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gukjiczqc.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrmamjmi.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwgxtzld.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfncjtkjh.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyzuiucp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gejzifvnq.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gcghywyzg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqsfkyuu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkehjrouv.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gmkuznpjc.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqewmlkr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtowskmk.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqetvvpey.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjttuare.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/geipzdbhb.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmpcggfz.sHtML


<!-- 参考信息 -->