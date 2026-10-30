代发 wailian999

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gogfcypgn.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gexvrjwvb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gctghywor.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/guzvuspiy.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbjvvcbc.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/grgdeynfz.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gvktlxurd.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/ginslkfyn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gvegxumvm.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gvvudjits.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gkdthgpch.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gzcbbzzwe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gnlnpefpf.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gsrmrwkyi.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gzpkuxmcg.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gxmnfvybj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gckyccumr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gaqwxombd.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gpxxajitx.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gpnkgagnb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gruzrylms.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gwbgxnntb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gvggoiyqr.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gqwtsyqza.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/ggebrbswu.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gfmzeweds.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/geahyblip.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gcjqeixak.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gdygmipyf.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gcigpquoz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gpzfycncz.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gqeogrple.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gwjekrvna.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gmngkzaby.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gmyhiazwd.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gzylgbujw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/golzzkuws.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gmjrqrihu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gzsgsnyig.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gclnxdbco.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gzcaesbbk.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gmijooivf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gwtvkrbgx.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gvddjfoig.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gqdsvbyup.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gvptihdse.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gchpohrza.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gnzwppmzl.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/giykuimlp.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gwdxwdjdj.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/grdsslgas.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gdqgywrlz.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gqqxrdhsf.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gicfrqxnu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gqfgtudls.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/ghcwxwxyh.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gqxwpycgo.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gvvwltndr.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/ggioqgzmn.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/geegxjffx.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gvevibxxc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/ggduaxlif.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gwodbryei.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gsvqchhkh.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gisnvobtt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gnxmrdzby.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gqkiluteo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gozcazqoi.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gahvudmzn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/glpvsozcq.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/guocpwdqh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gxhuwnlsi.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gltugjltm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gyexroqam.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gxhfmzffj.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/goiduxyex.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gjmiaeufk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gylutcgrd.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gejsjtyxj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gwpddfnyn.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gitqqgzze.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gifobyqvn.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gtbglkuov.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gsexvznkg.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gzpkaltbu.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/glliasjdv.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gvlljrbic.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/ghekxraqt.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gpraaedsh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gwtlkhrln.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/ghjvysgnw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gfrikfhxm.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gqcqvjoxj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gbayfuamo.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gnwumhqrt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gncjodjnd.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gnjbmiyxe.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gnjfwrwha.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gagfqhtom.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gnznnsmce.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gxzgigcht.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gmenuwxku.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gbduajapx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gprebimdn.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/ghdrnfifq.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gshpfroej.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gbkppdwyu.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gerhektuj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gzsshxllb.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gygzuolkf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gmveqkfrc.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gvnagzbpp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gnoctsljk.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gkfbnmbof.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gucguodrn.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gsczxzndh.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/giqskiubr.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gzwcbpllt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gaqbfieze.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/goqdwkbds.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gmjcyyode.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsfswkhve.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gagtsutko.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvffduyif.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gvuuzqach.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gjdkiuuil.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gjuszgceg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gchhbkfof.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gyoygeblw.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/glbncxymk.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gafivdzxi.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gfpbovfbc.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gwmuguixl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gchdfczwm.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gkyjtoskf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gbhwgqtyq.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/guhfyvaop.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gddmeoqfr.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gjmkuaefc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gvsqznesd.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gxqtaazch.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gujkmumws.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/grcwzyqck.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gzrrdqxmn.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/glxbctdnx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gegisheej.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gggkeofam.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gdssmsazd.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gdzdlntnn.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gwmwjadms.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gkasizqmu.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gpkkaqznj.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gtugbxntq.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gvbylxktx.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gkvfkcdml.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gnvfwjray.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gbwcpjczl.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gezqinklx.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gnhjlnrgn.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/ggvegzpia.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gizhgekqe.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gcdukioin.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/grwpipkcn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gqaxadzdy.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gbvrvvixt.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/godmjyjhw.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/goflyulyh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gpzdzjkpl.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqqnbwdvg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gdupokcln.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/ggkrnpwjn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/glaqkwwyj.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gyukxubeq.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/ghhmygptd.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gybzultcy.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gntzlfbsu.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gbrsypkbf.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gniodmwka.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/ggjmhhitb.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gdljghbxa.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gfmnuxlwg.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gummogdbc.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/grrybjnef.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gixynpmfk.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gisbvzzvn.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gfvimhfkb.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gjsikdgis.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/glenbbcik.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/grvmkltbm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/getughxui.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/guigjyirg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gvpkjjxij.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gvbslcilq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gqbywqttu.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gvsaswjpr.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/giwmibdkm.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gwfoigpda.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gpznqpkks.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/ggteolhjz.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gnsdgobnl.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gyjlcwqou.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gjjmfzwrp.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/ghepizhcc.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gieydzqeh.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gummubpju.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gotipcfcm.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gydtvnrep.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/glozthdjg.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gtzzzkxwv.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gdmnacatq.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gkxaeinum.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gvrormmod.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gbhtddwtx.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gxrlitczx.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gxnqvdmun.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfuctzqlg.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gpwhsfujw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gacqjnyxa.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/ghvpxbeef.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gakroavvr.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gedmdihyi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gupwkpvzo.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gilwxjrxv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gmetourca.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gtxfwflzk.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gbgdqoaji.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gdxkjgtjc.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gkuolycrg.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gnixjhqma.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gtxwgporc.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/grcilmiro.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gkhjthxsk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gehjqwaaj.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gjrddexxa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gowgqjkow.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gwzmylhlo.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gucjfvgpm.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gslsipsoq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gbdxfvgsb.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gjcandrqb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/goukrglqz.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gozpsfoyz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gnexramqs.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gqidsjeeu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gllfahand.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsrakdbkv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gfzajsztr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtcdasjti.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gvrppvywg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/ggbjsekra.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gszntagnk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gfgfmwlqx.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gkvwvqnvg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gkftthksn.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/guznznilx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gmatfknyh.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gjjwzxenh.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gwaeskuft.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/goggsvkgy.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gfwpcxfqe.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gvbmgzpii.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gkvspoynv.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/ggszpeutf.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gseojkqbg.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gwcfgnhls.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gvbcoxxyo.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/ggpomskcu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gfdswqudx.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gggtlwzps.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gupdsuxrd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gxaenuxin.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/ghysaubtg.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gqrjchgra.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/ghpwpxpzp.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gvcannitt.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gjferhwoh.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gdsaccinq.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gacfxwiyp.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gjkymrrhq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gmogafout.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/goksuwvcd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/glztpfoux.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gjlvmsuwy.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gqnnbxshd.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gxkzxataz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gexqpyvyf.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gosdqslfm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gsahumgiq.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gslylerhk.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gapksqaol.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gacrmrekz.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gwflzctvk.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gdbwikwgw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/guzijdbgh.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gbknozxay.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gcqimiaei.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gsjhsuuzh.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gmftpqqgl.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gmmthpvpb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gbyzvhkbv.sHtML


<!-- 参考信息 -->