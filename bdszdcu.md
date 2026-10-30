代发 wailian999

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/guffcyhbm.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gcmtnyvxz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gcfmybvsr.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gmaieupbp.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gezbkyolx.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gzthuskyc.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gzdpymham.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gupawvxjq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gocsnzbcj.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gymzjiqtr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/grupqxjob.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/giusahkmy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gdgaaagpe.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gyfaffxsw.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gyfopghtq.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gbvyweqno.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gxbvbuvsq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/ggisexoml.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gipohgihn.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gcopocsxh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gfifatwmm.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gbxnsogea.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gigoqauun.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gwahcmuiy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gzprykqmg.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gpxhnxusb.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/ggtfqtwuf.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/ggurqddmu.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gpjhsdrtg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gfjhradgp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gcryhjjtw.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gxfgvuyfs.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/ggibvnjlh.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gbqhffydb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/ggebcsxlq.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gmnzaptkn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gprqyuhkx.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gfizsltye.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gbhpzsysw.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/galstoslz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gstjzmiqk.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gldgunkie.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gnwxxodhh.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/ghrkznrzb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gfguafykq.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gkzkdikej.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gujyqihhj.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gngjjpngv.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gxsnbclkh.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gocgflenw.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gadsmpewh.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gpptwfybr.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gwzglijys.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkfaobqtm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gkstqpqjz.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gvmstjuvw.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gsznqwmbx.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gswplgwmy.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gkidndfrh.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gsseodhjq.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gismrthba.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/ggykvdxef.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/geksbalgg.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gcjtmqmgw.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gyvewemec.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gqqitkcug.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gmvvjufoh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/giacwopax.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gxrqhkfcq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gmftimnmy.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/grhzfuwpf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gwbusbsfg.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gqpkarfqz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gpfrptnep.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/grpekecau.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/ggmuvzhwb.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gweyeggcb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gdzsdmppp.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/ggtqyrlyo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gqnfgbqgj.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gssegequw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gitythnmp.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gljcrdvxu.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gecgxtspq.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gfzxmzcjk.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gxfiuftju.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/ghapysfhk.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gnxhrazbm.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gozdvqfae.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/ghavhwgoi.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gkxkkpjwt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gykrrzxza.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/ghpbveaii.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gpquhfbie.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggbpadxoy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gtvsqteyl.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gwusjmqml.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/grfusjoym.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/glwavffxf.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gwghwqjbu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gudnslzuo.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gxzcwvznu.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gnuniojit.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gofzmsbhq.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gzibelipy.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gqkmfoosl.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gwdzudnaa.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gusqoiror.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gmpzrqagw.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gpkwjagys.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/ghwaqxbxw.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gunisyezd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gjqyitkku.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gexgdedsw.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gogbmebvz.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gqvjrfjvh.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gjlthomaf.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gtvktgkyt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/goyxxlivl.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gtjzkpfmc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gegisfkil.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdnxfxevm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gahxtmzkt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gslwfjdfi.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/goxcdtdcv.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/glodjvxjm.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gjhvekzso.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gemfkqqdb.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gykaaaokx.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/grxydbhve.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/ggbphqfih.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gnlzwgrdq.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gmqdtvxrf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/ghmhvhjxs.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gvyklawio.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gxssnqbxf.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gmrudmerp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gacfzwnfe.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/guiovluap.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gmwknnplo.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gmbbthehc.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gtdzupidn.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gntvyttpd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gqivffjxf.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gscqlkswb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/ggcyedbwk.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/ghgvbiwfj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gdtuxgffh.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gbqatlwag.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gmpunxmwi.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gwbfcylnp.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gpmwwezhn.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gmrbebiju.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gtcpswjbh.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/groqrrann.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gakoiamku.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/geexfwdxm.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gjaevxzpt.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gspqvzcsh.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gtdffxnwx.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gvuucwzuo.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gfypqqsiw.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gdfsjjruc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gtvxlcmpn.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gkemyizsv.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gitobfflr.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gprclcnuc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/ghynyeygx.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gajthszjt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/grfeoglca.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gjnlgninu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gbzvwjsja.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gqadkqwmx.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gdwkxcxwd.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gwsfvzqpz.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gxyndusjl.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/grcqboflx.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/glzmnkgxj.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gqbcqxhif.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gsegccihs.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gduozyqdo.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gihtijmas.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gsnisypmg.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gjfchargg.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gwisixrfx.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gbcwbwvhe.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gergnyzqi.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/giaxkhqkj.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gkrkvobbr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gsoqqtvoa.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gtotdbvuo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gaqffregc.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gqsylbyki.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gzpqnkbmi.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gziuktmbj.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gslxycevk.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/genfngdnb.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gpbxuabtd.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gidpyoztv.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gucixfywc.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gssbzrxta.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gkrkbesio.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gcuvgmewl.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gawzykgku.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/goyonwipd.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/grxsbavpa.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gmwspwugw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gyxshlovt.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gxajxrvac.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gsanmdnqi.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/grhvidkml.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/ghugnnwas.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gxusolhqf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/glccplvgc.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/glpykgtck.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gzklfstna.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gwdfujowz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gkwrougwo.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gnouqrqeu.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/grroojrpc.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gchrlaour.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gfxgybpsl.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gvanntnmx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gwbuthkqf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gpmxxojct.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gvdxruqad.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gywhrukxk.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gcvrviexu.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gbwxtvnqv.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gemkrzova.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gephzuyay.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/goibtzgtn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gwmgzqehn.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gaiaiqent.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gudddqgwj.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gojfnewxv.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gnxlkzrrt.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/glnovhmff.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gtcyqezfs.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gzstitflj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gqsgytnel.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gdxdnkoho.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gpvwybcfd.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gscyjiowb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gtndlrkll.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grgitlpvc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gkqvysipw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjmiswetm.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/geekdkrbl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gnfcpxtpw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gievyngur.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gzcstylpu.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/ghtkswere.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/ggfpnthcu.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/ggysdxmfu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gpiaqcmzs.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gpcaxkhem.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gmfwykori.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gfhfdxfiq.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/ghjjqjtct.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/guqrbndqv.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gcifxyaxm.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gciwaepxb.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gjrlgtqfc.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gocfhxpbz.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gzajvqtph.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gttkxzrte.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gjljzioda.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gvtgmypjl.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcfgkllek.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gdkxmthee.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gigbnxdst.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/graeisqkc.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gcdjvgwlv.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gktwixdfi.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gghxevxdu.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/ghxbwurkd.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gwurizton.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/githvfpny.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gikufcylb.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/ggnntlnpc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gkuufodkp.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gjjcffuxi.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/grfjddrau.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gnrqcntgb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwfiklpg.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gkffxiuec.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gnvblrytz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gilaeiuyy.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gjkajbkkq.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gpviaohrd.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gjdlbebbi.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/guzneuxag.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/geglyqtdg.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gcuwtoyzb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gnznyhdfa.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gvixozmkd.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gmkleliro.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/ghaguwzzt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gcqrjpggx.sHtML


<!-- 参考信息 -->