代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gbdkfjrcw.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gtfnlwmzq.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwufmtnwm.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjozzwwfj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girjslexg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwoatxkg.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiwiovyd.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzmuovplt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gscfkacig.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlkucxxn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsrbsujz.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/guwhdzwxo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmyjitvn.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gbygxyeby.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/guhfkajnn.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gnaaylqdc.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcwqcdsx.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gnopwlgxz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuivpsna.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/giphodvfy.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gzchnjbjy.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmknheoln.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gzadwxpzm.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gimtltzmr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpwkqbso.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gfqqyrjhl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gdfhppifj.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnhmnelw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmismacq.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gtvqmriar.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjbxpilu.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfyaddbv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/ghvcjbwfe.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gbohmwdxy.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gshszkseh.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gprnjqqxb.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gwpqzwgeh.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgmzvhjv.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gofjlnkqj.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gflvztpnb.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjhdorlo.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/glasajpgb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gudwacpfu.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gmjmyuzbl.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/grmdeovzw.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsgkauut.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/giwxflfat.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goimiwpjj.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gpulfyclc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzuehpfdt.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdjwjnny.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gcbnaxqpy.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcswlnkoh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybuvqdtf.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gygodsfql.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvahvfhsg.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfowmdmn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/grexjiwpn.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvitdfwp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofyxnivz.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvwidnfw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gyqoifwef.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gtlvammsi.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gmyysdztc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaxkklgb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gevmxioda.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gxpaxwwcx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gvoswqeue.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggpvsqnuy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxpvitvh.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glthxmprt.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gucwjfqzm.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gjccfhpji.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvshthoam.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gvaukslkd.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsalhwhwi.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gprcwihnh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gvescsmuh.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkfrpbqc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guxnlhsmj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflpvyhox.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdszkmwx.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giwymmgbp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjbzhlqz.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhqrlszg.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyazanuih.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttclmfye.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhsgwfdg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gncardvgm.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gltcnvevw.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gufvpvjmy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaadxoii.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxerorxxy.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gwrjlfkwj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbadkvvez.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gyaepzudz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvqrhueg.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyudpgkn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/ggtdtupzr.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gbfuczrbq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsewyrdv.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsrwozsj.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gaglselqk.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/ghusysird.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gyiityazq.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/grccogurh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdurjvgkc.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvccopvt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/glhpgfljv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxgwcesb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/goquctjoq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gyojfxvev.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjdimqof.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbopptaa.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gncyghftp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gowdlwwen.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/ggydxpytk.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gswnfkert.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfesfkmfe.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gphcdqjxf.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gneacyvfg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/geqtbetlt.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjiajfmc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/glsssmrpj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlkvevsl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdltljlpw.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkispkqg.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gdofwwwgv.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/grxfuiywe.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaojuwfqr.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfisigfhx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgttmcoo.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gboptemvx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gesfmwitb.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gevzlxwpj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilpoyjgu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfzmmqsl.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwjlampp.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gugvparla.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gfaiexjrk.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/geovuorbo.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gknxibfwv.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gppkhtaty.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/giuiedvoq.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gccxbkjek.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gexwszznt.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/glgrwgoje.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gadhjxwsr.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnyknnky.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gemivhjew.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/goomvayqe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfshqomv.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gmefdgowp.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqxfpzof.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gjozkvyza.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/ghvivzdmm.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgkdzzav.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbretemjj.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzjgynkl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxarcfjz.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvkdwuie.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjexmmoqk.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gpoxwqaxi.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gspwzxrie.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gliptrgxa.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gndashftg.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/grxtrbwwj.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjfawhsr.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gxqdqjsrg.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gkwptmazk.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gbntjneyx.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/ghynnuqvy.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/giokskksa.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gwbypusar.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqhblnjvv.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gcidloanp.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gkkmtmuvh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzcichvj.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthvcyyef.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqefkssjf.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfxmlmct.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gzgdvrdkw.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnirpbrmh.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gmownmncx.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gdjhovknn.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gaxayizoc.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceiszwms.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpttlpqs.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gvtscvusg.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/ggstfzkik.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gedrchcoa.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngdbjphq.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzrrmnsgh.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxixqcdx.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfjscbug.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/grurxfxin.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgokhjas.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/glkaymyca.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzxioxyh.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoejpwiz.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzzfotnp.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfrydaihz.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gavuhkpad.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxnkzusue.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gzjrtmzlo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glhrzqaui.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyrnmafxa.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsbwxisq.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwxsseahe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gawnavrlz.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmioiinix.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/grhrtvuwc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqxykaitu.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gozltzilf.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjohmusy.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvcutmgh.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gkrqbjoqx.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuenazpd.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/geyqjmizc.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswmtmrpp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmcdyxrf.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gudlagbgu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gutkqwwrx.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gbemxknkv.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gtzeooldo.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrndtzof.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/grsrpedhi.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosiajsjn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxorfmwe.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gmqspthof.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvenfeux.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gsnpegzlh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/grybftjrq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghizbpomu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfolxnmbb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyyvqpxn.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gzvqiozdw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/grndqqklk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gcjplpkkm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdwsydaj.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gbocgjyhz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjtfhemv.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gfydawpwr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotqisujg.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/glafoktiz.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjsaumsw.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqcfauua.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfkkynum.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowfoxach.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfcygvpj.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjhuyiam.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/geovtvrby.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gmtzjvczz.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjfqkqeg.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gedpvayna.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdwjyjkm.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwgaeslr.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplyjytwo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gyipcsyae.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gynaufnsb.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtycdigc.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girvslvmt.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gisamxszc.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gjcawyecn.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowzhnxnp.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gzntsnapg.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvmfcxef.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gosladtbh.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwwtylry.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/ggjhdhryq.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gaedxzjew.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnchjcyuj.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkudjpcg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gilrivjnu.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gibpoosnu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkyjrtdh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwmqxfum.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gbbufyaag.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gonnxkcgu.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfecbjzjw.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnpzrwoy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeyghbiu.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gifwxdsvh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gwpxiugup.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gphbqoqrk.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/ginsbzkmy.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gzwogngbb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getxbkxuk.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefylwygt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgafczsx.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gssviilis.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gvqaycqob.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoajdaao.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gvyrudatb.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdbnrvkt.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtykhqvaw.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gthdcruez.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/glupwvumj.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gwpatrdai.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdjlmghs.sHtML


<!-- 参考信息 -->