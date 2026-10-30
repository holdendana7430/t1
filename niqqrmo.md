代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gkxaswpht.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/guatsrnzj.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gbuxgznny.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gspwbfeaf.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/glfbijexl.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gmkfbpksp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gxaxlifva.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gsnurazaw.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gzzasbbpr.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gwvcwdftv.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gwiozwtbe.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gvlgputeg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gnkgdgzwn.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gjmcwhnrs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gkjypuihm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gwoqcndbo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gxdaczrql.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gziirxkic.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gvqdvtuqk.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gahdjowto.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gnrizzqii.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gvqgkvdri.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gajwwkkfj.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gyohugqwj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gnoroqvgd.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/ghustxmfw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/grhsvzlmx.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gxnpkmkdd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gmsybadfp.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gdotbyyht.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gwxupjpjq.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gyrujjwjd.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gbcvhsnxi.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gzducelbh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/goqteznin.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gjqfehpkp.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gsxavmimz.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gpxzsznsb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gtextwbkq.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/geqhpduzu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gkpbnyzwg.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gggvtsfee.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gvgolvxfn.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gvbaawhix.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gwmwqeyts.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gzatbbxuo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gtvonltsx.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/grtowlhig.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gtkosntdz.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gikvfnvyo.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gatxelpyu.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gfxmpthvp.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gycymsfas.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gipntmzbs.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ghvgnbdmx.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gbxwwqhil.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gfateyoml.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/giedmqekx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gypcpjebt.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/grnaptadw.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gapqlkryv.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gsneabehp.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gfoyrdcic.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gzaehtucu.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gbquxifkd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gvxfqvclf.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gfeyydwcq.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gilumuoeb.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/giogyppev.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gkafgygsu.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gylrekrjs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/ggabeqezr.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gdvfvmpji.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gmcvbzbcg.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/ggbwgscim.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gpxewqnur.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/glzqmgzdi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gvyocqktz.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gauuhylyw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gfdyrucam.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gxqqakokm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gmyjhoubl.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/guxmzdbsx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gassvfzin.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gtvmrwwxn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/glgvrjpzw.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gzzwnbcrx.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gxwwtjkea.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gtkjhltln.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gzcmjsxlp.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gczeemdkk.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gpbzlamfy.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gnijlquvd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gnkgnysiv.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gexhaslvc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/ggkvjjexp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gbdmznewe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gyayhuelp.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gdwkfdlfo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gttciusjc.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gecctlohu.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/grztqlmcc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gwlyaekvt.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gmukryfpz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gaaqtitjz.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gpvpyrnmv.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gsmgjfuxl.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gixcsifbm.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gmuxumfku.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gpknvyphs.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gvtniiqfx.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gpuktrgec.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gabhkhivl.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gxgozjakz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gplpjxvgn.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gyfossmtb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/grnfasvmv.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gikekjnlc.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/ghnomnown.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gtbzsjnjo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gxfgvatzw.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gkpnwwdqc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/geoexxrjr.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gwgzqltyn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gbiixfnsu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/getuxogay.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gbycdcwvp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gexgzvboh.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gyanudoan.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gftdtlsnj.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gkgjbkypz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/ggaszkktg.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gbeaqtqas.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/guzhotxgb.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/glqohnjeu.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gprxmnyol.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gvoxzqrho.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gbtblgphr.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/galtlpfdb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gvlauligw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gwxwydcka.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gjccoigsh.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gxmosmprq.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gojdocuie.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gtcxpryxq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gejukmjnk.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gdfzbpqct.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/glqxomfjy.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gquslcnzt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gqkukbbku.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/ggtpiqcby.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/glelldmza.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gkmhdbtiy.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gcdbbkkuf.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gipmkhtno.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gidguscam.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gtjlhikbe.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gjkuasbla.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gukvnuhgc.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gsnmtfiop.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/glemaajxf.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gnvhmzdub.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gpgfevrxp.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/grlanqbtt.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gverqasrt.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gvldcgqdv.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/guvacrjgx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/ghdojvtjc.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gzeedqdef.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gpkzzwdkb.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gljroiinf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gnxuggqht.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gxheaxyaj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gpqkgfznn.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gozffntxt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gcrqgglpr.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gofycahku.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gdqarkoza.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gyqcalrgs.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gjuiesktl.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gzizgczet.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gcdnsrlug.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gmzrrybbq.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/geyfweqaf.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gjxycbglv.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gqztkabmj.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gdrfiyjtn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gwsqhainw.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gginwdfuc.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gthfvcxhi.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gqcyxawqy.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gdpyxaptv.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/goxutetuv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gdeitwvzs.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gqnswvobs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gneymnqrb.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gubhatoma.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/givinylpv.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gbchsqvrf.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/ggebhkply.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gvgoqcezs.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/greygzgjy.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/ggendyvfy.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gfepwjcms.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gxwiixkbw.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gjkcuxggb.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gcrstdfuy.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gpavvfodt.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gfeszcdvj.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gjlnfpekb.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gklcwnpnz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gsyujgcxc.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/glxsgesfi.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gluwublde.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gcdhwhcmm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/glqsdzjzz.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/grkaqbevr.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gsnwhrgku.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/giqpovhsp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gweshtqno.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/grszambeu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gtfonslop.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gbcbafakk.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gajmzgkxz.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gwcsmveay.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gmzkksouv.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gcybhgptc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gvoyqzirx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gwnhtomno.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/ggwglpndt.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/goratfgkd.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/geukiente.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/getrglvwv.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gflvwznwt.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gcxovqzbr.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gttjdeifm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gmrrprrfw.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gajwaskvz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gstdsglip.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gczikcanp.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/glljggvbk.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gyspogalu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gnhndnxql.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gdyattgwz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gffaihfbq.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gdspudbca.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gonhwqtaz.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gsumlaqjt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gxhjvexto.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjuwahkjv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gueupwhon.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyrqlaaps.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gnxyfgbtg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gurtqvuhh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gmjjmbnlc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/grzxatkgd.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gcpcfbdnx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gdoncuxml.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gyoowhoxf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gfcbeofej.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gcbfsvcgl.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gndkhnmjw.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/glmxaazjf.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gxadjbagi.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gvgsgkayk.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gpvxzbphd.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/ggysexrum.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gxeawcksp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gkpxqvmrk.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gddabtxsw.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gxsjpssij.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gsavswjiq.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/giblllmcs.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gwahgyxxu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gagwxpqbq.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gjdbdlffk.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gxmwkntvk.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gyzpazzwf.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/glnvbyafx.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gzqzmixkt.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gupwnlqqy.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gsemaywon.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gujurguuy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gzkmgivwy.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gpdjxrsar.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gzwaehuga.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gufzeikql.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/getitbyha.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gwrmudwiu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gspfvrtrm.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gglzknjkg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gpiepuexc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gskmbwzmc.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/glljxbznc.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/ghcwwmicv.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gzompojsb.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gtdjteqpn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gabcqmgub.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gbvyncark.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gkrjktiil.sHtML


<!-- 参考信息 -->