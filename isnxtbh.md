代发 wailian999

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gehfohpzs.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gfljwelqz.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gghtrergp.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/ghovlphqz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/guwticvtz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gagmmwyjt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gqhiomxog.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gosvicvrk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gkbtzjxwy.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gfcyxbngl.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gzlnuqrdm.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gviwraxvv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gjxruphjy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gmfqrczxc.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/glxgyirqc.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gobtjeovk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gezfppenn.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gcgqefspo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gxuqsjvly.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gynennrty.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/glupibjmq.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gwahzfsbc.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gobikyndp.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gkmbnjnan.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/glzbqffmc.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gzfqjcfxk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/ghsbsznbk.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/grdfpnuwy.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gtumruojf.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gqlhxmvab.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/guegzdbaw.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gglxjqttw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/ghmqakgks.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gghbmaejk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gvqilaarg.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/guvnbylxx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gklmmkdgg.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gniypprke.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gtkjcmxlh.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gdeytghcd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/grzuaujfe.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gfufxrevg.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/ggdkuayee.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gttxvqoeq.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gjzslsghu.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gtwakidli.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gbcbpefsa.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gdokclqre.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gqiymysdf.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gvqkznagk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gpadktxwz.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gimvkhzcg.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gpxbijiqa.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gyzpujvrz.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gubxcemwc.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gkdllcfvh.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gkrxnalkz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/garglkfnw.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/guvnsotrh.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gnvqhtuot.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gexvsvixj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gwqgtgskz.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/geccwnqer.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gwhphwamr.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gcofuzjhp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gbstyyupz.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gigxyxbvz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/ghcksrpfl.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gpzaozyip.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/glhgrbpfe.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gzmmuztyi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gyohlyxaj.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gxinhufee.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gkewakgpf.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gnovormbz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gabpyhggo.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gwpuyhxmi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gaerixhla.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/ghsficjec.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gaqbbwxmh.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/glnboypnv.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gilniorlv.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/ghurggwzn.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/goxktpoqi.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/geltbkjng.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gagjjdvdd.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/guhvznsiv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gbvvqtiij.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gpokcskzh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gyujhrfgn.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gdyzrwmli.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/glfeapdae.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gpzuevrmu.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gagiikmzh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gfgrgenaq.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gnvnomsqs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/glinqydbf.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gqztgwoou.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gkayelexl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gbyvooypq.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gylcthqpf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gljfepyyy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gqkwhzqtm.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gkwyxieva.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/ghzaeztbl.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gfbvpfbte.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gdnfgyaws.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gsigkvuai.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/grzqcafgd.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/grzbyurze.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/genzmvbnn.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gykvlrwct.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gzodkziuv.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gbmugmpjv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gkpwpodeg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gbecmknjc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gnzkrfyic.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxqikyygc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gnkgztyov.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvavmmwnc.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gilzaqxgj.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gnbasviqt.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/guadaesxj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gtwokarhd.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gtdozgwqj.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gemgyakic.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gtneotmme.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gowkutkvj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/getorxbqu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gomjudggv.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gooezznnk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/grkockizj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gctztrlnz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gnlqacpnc.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gslwgtegz.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/glehpdiwb.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gtwamsbeu.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gzufkjgrr.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gznbmvqdf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gzwmjycam.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gfrccmjvq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gmntdrpbx.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/grtnxbfzm.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gavquhqlc.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/goepkvxcu.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gppnaqfnl.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gpiftktrc.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gyxuhcvnc.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/grvbmomum.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gkkgilzkp.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gobzthetm.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gfjxqohbp.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gxnyqbrjt.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gyfwjkvsp.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gaxziupdy.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/grlmlqyid.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gjwzelhjc.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gpntpldpx.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gtyhwdywh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gxhwlorhk.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gckfcqmkz.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/geyuynsts.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/geemburdw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gphecaccf.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gwnisokfp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/guucpdjdn.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gzxxqqfvm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gdbmusqpx.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gpivoawqx.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gchvodcsz.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/glxkozajs.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gkvtfimoj.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gvgqytnch.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/glwqllsjk.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gkjjvvvmu.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gksrzgiez.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gpcmuuaul.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gvjdbiakk.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gdmkvunmm.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gnxgioegf.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gjxrppsky.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/geejmzxfs.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/guxqmuuso.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gpoyqeyyc.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gcmoykyuq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gwogxgpxh.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gilmpxquf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/ggytzuygw.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gehmjtmql.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gptjzjfzl.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/ggfkoxxbs.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gwiiqufth.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/ggkkvzmyt.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/geavnyamo.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/goocnichw.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/ghpqkwxfs.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gzpkaeymg.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/ggosdzosq.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gehucjrex.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gpximychp.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gpbtmfjym.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gbacycqfz.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gapqmqdpc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gvgcmnsrm.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/grgkrnqdk.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/ggppfboou.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gycpqnjsi.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gdyouofjv.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/ghcrnpopw.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gyrsamapy.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gueceicvg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gkadmxdot.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/giwasdcwb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gtcgmxgmf.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gpzgaftbf.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gbnvfhxgx.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gsnxexmmo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gbbplzxqy.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gfmdiqszc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gtgyoargj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gqogireqp.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gkesocaje.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gkpufdgnb.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/giabwmhot.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gdbywbedr.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gbsjsnbog.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gztglcrff.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gdyazqsch.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gtineinjt.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gwkxqzrkp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/geotrwigl.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/ggohczedv.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gpzdxwiqi.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gcmvmdwym.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gpjepzxzp.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gkeijezcr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gageutfyr.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/grnbocsyv.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gabfxnenf.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gxvadimvq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gajpyxvah.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvogptfkb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxdydttyo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gptolwmnh.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/grydfacux.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gynyrijfw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gyijibbkz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gtdeayqym.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gcdekwtei.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gbdxpdkxk.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/guiyidjrd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gqllggnoz.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gjtuhdkfv.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gizydgtss.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gdvfhvuzk.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gloutglgz.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gezpxdgzq.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gynuqyvbk.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/goxjhelvl.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gvygvbfnr.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gmpdxnbix.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/giiizlxkg.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gpwpejmlq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gipprflpq.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gurxqzvlt.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gkxisxedz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gcydwjrka.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/ghphjkmpc.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gconaqhde.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gtukexosy.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gdxjveqwv.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gprpqmqsu.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gzzxfugnr.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gneltdhqh.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gpquqrwte.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/grrtdvyig.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/ggpvxcrtc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gzplgqjjz.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/guyximihq.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/glyaqkeve.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gjzupoqlh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gtzwwfuxf.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gtmbkvcyz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/grqgxclqs.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gxdmesipo.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gbdqyusxx.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gssjaisqj.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gmdksjdru.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gsozgzwwm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gqxccxqnd.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gtnovjjmz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gcfmwcfqx.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gyojgetgz.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gunjcdmpd.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gpywotvfo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/glovpphss.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/ghmzipntt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gwwwnayxx.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gzvdskapt.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/givyolcga.sHtML


<!-- 参考信息 -->