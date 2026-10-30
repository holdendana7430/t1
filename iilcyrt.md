代发 wailian999

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gomdkdggj.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gfxvzpteb.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gbjvzsxax.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gfocodtcq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gacpqspsf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gdtmzesbc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gakhfzvdm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/goljmimsl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/grbrtmucr.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gqbjxamvk.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gcjmrgjzy.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gxliqjayi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gqnvcqqdf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gdvjmruxm.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gcpvdmwjo.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/ggtixetky.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gzvpmxcjc.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gublrsffr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/geqtnwwzl.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/ghuohyymj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/ghlaoirxg.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gumxxrrkt.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gbjmymfdp.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gaspqdjro.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gaijusatz.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gkglcsldx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gzjjrbmap.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/geixqmcqv.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gihxwvbiu.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gnixuyrwg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/ggtaovcht.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gkpxltzkh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gkkqshhum.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gehccjojk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gywfkcjdn.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gyzogohbp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gxvxrynzk.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/glsiunziw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/ghocpvmpi.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gzwzssbnw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/ghjbohude.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gldnouhmv.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gevdtvvfp.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/ggvbezrxb.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/grefksgpa.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gmzfahjba.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gfjnuujtp.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gritpguuu.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gablzrvmr.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/glqzdlpxk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gvmynyozx.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gimfnphcf.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gimdehuwj.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gqamzoiwx.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gurwjdckl.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gsbussxlf.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gsfkpjwdn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzugzyma.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gpjqmtczp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gjtnibegz.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gxzdbrjwo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gdiirbgrs.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gxqrxlcha.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gykcmywkg.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gdzfrncms.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gglwhuvzl.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gshofxkjm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gdlxhqzaw.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/grvsdvplt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gofyxalvv.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gbvkuhihk.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gtrjmoqqd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gxtfdigod.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gdcvdhktk.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gbqvlyvqh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gglbxnbpc.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/glssjenfg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gnlvxraff.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/ggtmqysvj.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gukyqancs.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gbeuxccxu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gcyuhxixl.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gltdjoxfv.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/ghvdadshc.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gflothcjg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gfxgbeaws.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gestiqiyf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/grlrrqnxo.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gihrutzdp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gbexbvogi.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gcvtfjpmb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gdnegcion.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gidupyjhw.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gjsjnrcxw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gaklfrwjl.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gksazeqsu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gchioiojy.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gitlurtph.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gessszefu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/glqaffsqd.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gnnauzjcv.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gogwjaqwl.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gywrgvpzt.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gzbsbvhih.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gcjhaqqor.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/ggqxlhffs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gckmchntg.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/ghqrqfxmf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gzkqrcvoe.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/giphcnppv.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gxrycczsw.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gvqcxwevw.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gkseagaqw.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gdmknkphr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gsisnbxkr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gilsmfcgc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gpxfjuksh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcegwwpgu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gwticlkru.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghduqocox.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ggmwvklmt.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gjdkfuekm.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gejlkfxph.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gbogwjiie.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gmtyqwaqw.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gndeltwwo.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gyrdvrzbs.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gaucbypta.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gdmjkycvd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gkmpgmupq.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gbtuskagn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/ggnmrkunh.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/glfwnrcok.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gkfsytilr.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gimzygqjx.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gxrhzrpoc.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/ghwfbdlyy.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gwyjivnep.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gqffaddwe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gfrthjgrg.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gskvziklc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/ggmldhbsl.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gxfjyxfeq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gsvfcqmlc.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gjgyzfmbi.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gecqyffwm.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gmbsmbysx.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gyplmklgq.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gnwznhwhb.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gqnuxkkbw.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gpvtfzbdp.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gsvxvpzfj.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gidohgbey.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gsujrtopf.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/ggdsizkio.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gvplzfcwk.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gtgwxdwfv.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/grkpaenyu.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gowyqojdz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gludbalyq.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gnpyguhay.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gnznlkjxu.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gznjyamua.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gieqwcimi.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gycpjtsuy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gflgyxjco.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gsexdflko.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gjzuyzjke.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gynlzzzkw.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gnnmzdguq.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gycprjbud.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gtpbejkyj.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/ghtwzqzjk.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gypsmmfra.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gyidjcsno.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gvdryeope.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gvmigljnk.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gwerlkion.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gwpcjlwej.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/greeqszcd.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gaavafweh.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gjqvzterw.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gbuaadxic.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gwywqifqv.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gkbwgrukt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gzrbyuorg.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gmfyfrlzl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gthajlfnp.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gnzvwygwq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gmsbersqq.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gxptiqoom.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gwtsefdlp.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gagzullka.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gxiybkoff.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gqejsrcdo.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/ghuulrqtf.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gulgrizvp.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gxnrfbltq.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gwoxxnbeh.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gadwqhkpx.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gceplkejq.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gldnletkc.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gbkppadkv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/glkyslgyr.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/grgurmsep.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gdutyrlmz.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/glbuwofxv.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gymnyztzw.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gaecmdwcn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gutapkwud.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gerrjvjbn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gfaftpspp.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gsgcfrtjj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gdcilfoxc.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/grlmarfwo.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gnpfjjnzp.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gbvhxwlgb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gvvskiadi.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gdjtlwewe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gklijrfzx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gvoekewvl.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gyzzfwkfw.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gutgyjzdp.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gwgmvlybl.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gctsowznt.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gvhbatxkb.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/giddgbgtr.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/ggpfmouml.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gthfbarwb.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/graczvysb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gswuedvom.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gdpsilskw.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gwrnilaaz.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gohymuviq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gomreivmv.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gxkkonhlk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gfttylfdz.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gsqwesahw.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gfdclccmb.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gpcauktrz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gmewdwpvq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdpevzhmg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gmeuqwsbb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggaduixid.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gayocshdz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gedgcmqfg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gqmsrqwds.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gyprwutgz.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gxxhnnmbu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/geazcvbgs.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gziyhnhrp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/grlmvmitk.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/grakewsws.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gtrrdrzwf.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gfxcjgtmj.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gmorkhnpm.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/guuyqcpyk.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gjxazjptu.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gkephsuef.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gnsocftih.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gbhpavgss.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gqpojcvpk.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gtssjijym.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gwehhxwml.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gyupengsz.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gqapibmkh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gxkwlhtgz.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/ghfzygydg.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/goxcwhdff.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gonxokqps.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gghtpzxss.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/ggcufccnl.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/ghyymdcyr.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gyswirtsv.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gmjfuuhjq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gvousxlxy.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gkgltpudq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/ggtoumjqn.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/geqrmvwle.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gfedcdffx.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gjbyuyxyh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/grccyivtp.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gjxqhommn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gsssvnhmx.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gursitybd.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gbqswafrt.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gcarouodv.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/ggsmncemu.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gewrhtdsb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gzyqkkzbs.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gpjdaecuw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/ghujqlovi.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gpzgxyraf.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gpgaxulwo.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gipxefpeh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gwvudforv.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gisttqprr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gmvojuiwu.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gverjufuc.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/givcrlafd.sHtML


<!-- 参考信息 -->