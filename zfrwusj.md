代发 wailian999

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneqrxsjf.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gykglxyim.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdxmacnn.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzjovxgnz.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/guvgdgumo.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gcgqwqjze.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqymcgxnx.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/ggioovknw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvlnozwt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyxwllmy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gmbhmbgok.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfcbysev.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gukgmrzzt.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gmczuawqe.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gasxkarnr.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnhmclznt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrfjguyb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gscxhaxai.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhbyzqhu.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gthqkzkfe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gbktpvxyo.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gfsfhfchd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjphjshjv.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjrirjos.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gwjufbhpa.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekogzzqa.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjracznv.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmcoqjgv.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gpzxlnncv.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdsnjpgn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkhsilzz.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/glrbtxhku.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gappuhwsb.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkjjqlsb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdshtnlkv.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gjqvdugci.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/guhellfuu.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgjiysfm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjikpvjz.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuvvtbuh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gidsbhzkr.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gaekzpymn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/ggcbfbuoo.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgpoxlre.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/glhyidoaf.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbgvasaw.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsjwkiau.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwpnubwf.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/grbehbbdm.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gavokgeva.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutrmoabb.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gatpvysuj.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/ggygdmpyo.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmzfffvj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gvljdvmzq.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhxrbirc.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/getmylysx.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/guoizrmir.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfmonzmr.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gzsrbwjta.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnsepjvp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gapemjimh.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiwxzpck.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkwfvrvn.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/ghueqmtpm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gjyvmqqbg.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gawvkyfuu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gphdkkyon.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnleoemx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/giefmgomq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruazxgpt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqubjqst.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbynhaij.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gfqofflko.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gdmckmtcv.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/glzxpdlbf.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghhjalzdq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhbjdqta.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpcbwlni.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gphaqcflf.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/glnixgiyw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/grngsenwl.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gsjabvxxg.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gzwdkroho.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gqcirqzby.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gisuzmcka.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gipztzlgi.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtedzdjg.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/glbdynguo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gcghyvoqj.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gaffpptot.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gczyrgmoy.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmjpqixv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfwvtuxin.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gakwdtiaa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmahrjwvj.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gzuafsfdr.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gabuabkso.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgkqvxgp.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gngzlpnpn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gluclrsov.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdmftqrl.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gztvxtpfe.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gukfxdmot.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gboelwtnw.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gxcrkhmuc.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gegcuytai.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghfmovdr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gskzqcfzu.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxtckbot.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdutwfsfq.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gucmtanyf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gidvbcdrh.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gmwelhdvf.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gwryfwktt.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcohbsgl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/govpwsyea.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gjkfobnka.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuyaapjp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtovisep.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssbnohkx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbunvjbaw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsedjqygq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqvkaehg.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gbhaglblq.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gphdisinp.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/giiclnufj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdstqragm.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gynmtmwvf.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjyshflo.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuvzamnu.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbxolkbp.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/ghrheeyud.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/govewzjis.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gzodashye.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gershzqaf.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/guavjwymm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/giqetalji.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gmixkihio.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gzcrqehfj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gdruowifh.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gmjonfncd.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilrulmeb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gmrtasqsx.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gwmmywlhv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxxvifzq.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/ggpnvkhnm.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ghwhamfql.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkofwacr.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtrwlxrjl.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxobjmhs.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gakscrgql.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblidycba.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrhucopz.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbckxbcie.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gxxiqczeh.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrwjxqeq.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/giqbxfgie.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gbvawwsrg.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvymufbq.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvhxmegj.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gghduivvw.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdcmlnek.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/goivupbfz.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gobalacxt.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpufruesp.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gofobcjyd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrdxlqpy.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglxftxxi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbhlhmxp.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesswmkhz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gcztkfsis.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gknfeiwjz.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrxholyi.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gmtlwjtqt.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfpvadze.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuvxhovf.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gwtwlceyy.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksqezjfk.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjkzhsel.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/golztjhas.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcmnicvq.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/glhyxchpv.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gtgkcipry.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjsytgwi.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxhbmhyq.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gopwedbtv.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gbftknokh.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpzmapbg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/grdcbqinf.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjgojoum.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvakjreoy.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/galempqtv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gratnpdbt.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwrhamsn.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzkbsyka.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gphptrhwg.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gnsspvpjr.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gzvhpwltn.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gflfcywon.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gosyrgrsb.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gocitmjxn.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfmbhfjr.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpqbddxn.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gcoohtmzx.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyrbqmcv.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gyonzeemy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gtxhgpyvt.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/glogvqhlt.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gljpofpyx.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgduemfw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqmsrwnm.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gzbawwyuk.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqojipbis.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gskhfvlyt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbiyjvub.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gvhwahpvc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbzogaqaa.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gduztqqhy.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gixguqglc.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gibndprjt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjsooohhn.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gecfvxbnj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/giztgtxfk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/giavnueix.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwqiygcx.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfuxfvxu.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gausyteoq.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/guqqdgivj.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrebmamn.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gponjmyhn.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gsetzvkrd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaakpdmt.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gkabbckiz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/guhzxgfbt.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gxggaalna.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gehzkmwqa.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnsybkeu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbxbpqqc.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvirdmdwy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/giocdiwuo.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/ggkbhrrfr.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/grgbwiaar.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gthbtahdy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/glrhospzf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxiegjdh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/grygjmhlp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnccsehfg.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfevmkyd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzibixqti.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjglwelqe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gaisupqzp.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gqiqikrcx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gpkskonpc.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecaatryl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gydxlmack.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbogbzth.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gsxahwlxt.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsxhyqjx.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gfjtqmzbw.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiqkndkr.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqflrglum.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gtbeqoozn.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/glwlnjido.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/glkbbawdb.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmfixjnu.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gbohwblzb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gteacwehu.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gdrgdhbyz.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gmyqnaxpu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxctealh.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxfhmllr.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gorjqugvb.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gqicoumpm.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gurqidlbu.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbbndbja.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrkyeezx.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gbfshxylj.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gibrzramw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/guvyxualr.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoxwsxtm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmdnkhhr.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhszocsv.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyeevbfk.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvdojplf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpqffnyl.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gzexopqbj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/grkxueaqf.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gcpjrjrbw.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gklspapxl.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gktjchmbd.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmscqlko.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsamzsmvx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcgofbhf.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgmlxvdd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkiaucsf.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsbzjojr.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gfdiyrrqh.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gstgsghab.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gwstvmyar.sHtML


<!-- 参考信息 -->