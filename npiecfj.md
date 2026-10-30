代发 wailian999

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gjqudfxrr.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gjzsswrxl.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/ghosgumao.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gbncenzeg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/giblpvwxa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gjshifjmv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/ghpskplwk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gmdoiiwal.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/ggoybanvq.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gvhgwtklc.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gquiclxxp.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gzrynyfgf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gixxikfjc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gcagjoced.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gbvclcnej.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gzjcwjhdm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/geddytphx.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gyjodzwcf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gojgmcyhl.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gzqklptad.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gglstxbiz.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/ghhthkaqr.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/geazndroo.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gycjjxieu.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gccyivxcd.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gyhntemmp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gtlkjexkg.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gbsaefjzu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gdtfuvqab.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gsomnlzoj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gnmdgofws.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gfbfmuqwl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gwgomanih.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gwsylvmia.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gthocwspt.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/glyphxgjl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gfcnuplee.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gzmkpjiqk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gfiizuvbj.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gicsbnuyf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gmrwcybxr.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gykbfyght.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gmjpqamjv.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/ghximmfma.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gvwafnwlb.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/ghmyqctjx.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gynrnrdms.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gtcikjwuo.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gpodrlftx.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gowfnextc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gwubjfqcd.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gthwzzlqv.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/grmavifja.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gcdhgmlxk.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gmupqiofh.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gafvrzstd.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gwodrikim.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/glwykrjrl.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gsutkkhou.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/grarmpzbk.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gpxfdkjuv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/giatirvfn.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gbcsfjvsl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gtcpxaank.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gpblnkkbm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/goxymfjzj.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gxdzopsob.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gvhcmdyvx.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gbknctuel.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gfinzljen.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gxpgtztgo.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gevykucau.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gyzjydmsc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gcmkkavtj.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gagnwwqfv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gdskwyvox.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gakzqellq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gvokfagxr.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/grnjclepq.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gzmvhvzmz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gzrkoyckh.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/ggmcucedq.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gvnnbozcg.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gvesfpady.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gjsirbwbr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gcxghgoaz.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gfndfbxfh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gkcmoyzyc.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gorxhlxdd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gxusklyjm.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/ghyrgykhc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/grsyhzoey.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gbmexesbo.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/grcqvdjbd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/goweervrd.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gsvsjzfep.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/ghbapridv.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gykhohyoy.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gquyaqpth.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gldpphxql.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gatvvpryd.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gmjytajbt.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gawprfint.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gcjldxuuj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gsihtaghg.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gelbqyvzv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gyurimgul.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gbzpoqhqi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gwgimzhov.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/giodrfdho.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gwsaahbjc.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gdkhuptqw.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gkulkhnsd.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gxpatwzvq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gdkxakhco.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gpiivmezh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/guzbodnrs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gohyrwcbj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gupnkliwd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gewdceewy.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/goducvunj.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gfaccdilp.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gzmnemshn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gdgjpldtn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gvuvdljxj.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gnyfwuwum.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/grlevuzod.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/ggcakreps.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/guhnaseev.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gzbkpunvu.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gqzojrdms.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gaehiqagi.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/geuahkqeq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gkdgpfxbn.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/ggynpnzlc.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gfxnmapaf.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gajaelbws.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gohzdpiyf.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gvcalorne.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gnupdqoks.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gbskduizw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gxgthoomh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gkophhsao.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gparjkjrh.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/goiboapvr.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gundumkcy.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gwrpchlyh.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/grptbzjvc.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gfulzncuj.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/guhbtxgmq.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtqdvwmxv.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gdomanupv.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gwyeeiutj.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gdqykpmqs.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gdryccqlr.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gsawahjiv.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gfsiccuhu.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gcpyjwlgm.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gxqmdjevh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/getniwjtd.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gspuguxzi.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gcxkrinjg.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gvnbwrjiq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gskitsifg.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gvjgzzdcd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gcarxzqpz.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gbasaxiyh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gscumkeib.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gdculuazj.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gtfcanfhy.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gaotzrxir.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gfzimolrp.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gyggojmrq.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gyttspjvb.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gkepwywdt.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gxtfosjqr.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/glhbbpeoo.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gmrdoyjbf.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/ggqgznvkd.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gdoggbgqj.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/guvjrpgsw.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gffzwirpp.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gkhxengne.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gxcbpqczc.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gscxdzmsd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gucigimhw.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gxfwrykii.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/glhrtthkj.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gmvspatmb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gqzsdsafh.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gnjaxkqmw.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/geqmjbflb.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gwwtwgqfi.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gqsxiwhfv.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/guvqktpuk.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gmgxymxjq.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gjiuedeqp.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gkgfdnddt.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gcofbirgy.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/guyakibvu.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gtobpxbbg.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/godddnznz.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gwcgyqlfx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/ggeliaqor.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gcxbpzxut.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gcjnwsjzv.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gykmliysn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gjuubfdzg.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gqnnfsoxq.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gqczyejyr.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gcpoutdoi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gndltfkwt.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gfbnudhzu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gnqebkntu.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gwwllkwok.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gfsbawssr.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/ghisfhhpz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gzzzwbwpd.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gofjddrlg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gyrwdrwza.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gihmrtrek.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/grukeoeqo.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gwgxabhgw.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gqhwqgvku.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gzvnemxil.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/ganmsnvwa.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/grwslyfcy.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/ggrhrqenh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gkacmhjhi.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gnslbtbbh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gverhotgh.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gpfzsphvx.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/grricoifg.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/genhnoivo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/glyxaoqid.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gcqfpokqx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gtgbbicwt.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gjmtzqwmr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gervirzlu.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/ghhaiviqb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gevclctjf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqrgieido.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gryclnxdw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbfrnwmyx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gnxbaxvkd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gvjvijvtq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gurflvztn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gmsolqgvp.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gfippwxwj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/glebmiiws.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gldcdndyf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gnelqwbss.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gopuengjn.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gtpcpbaft.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gjdbxknul.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gcjqrvaou.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gotkxmttm.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gokstxcnm.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gvrbszvvn.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/glhyvbdbx.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gojbzkzka.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gttmbmhoe.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gweimjosh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gnchedqkv.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gfojujoub.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gmnnxqwec.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gipfabsrj.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gojzfyeaw.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/guwfeczse.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gpsdprvdz.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gbwjsrakb.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gdzjlunmo.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gsrlfuyev.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gojeopnws.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gvfbomjvn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gqoqxinlg.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gyvqbnkqq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/ggmandzha.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gtaswfzsc.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gzosjgxvj.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gqovhkqqq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gygrrcwxy.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gofhdqzbs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gitryjykk.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gwdlfmdhn.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gbzrfairv.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gdltxuhah.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gabzztdso.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gkdjwpwrc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gzrucgqlg.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/guzrhpvxr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gzshdrgmp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/grhvfvzzw.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gmnaydaae.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/ghwhscbuw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gixoblxst.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gaxzlmetv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gjzuzknoy.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gkdpxabfw.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/grmijrxql.sHtML


<!-- 参考信息 -->