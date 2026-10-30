代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gfvfmzvog.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/ganedxwkl.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqkmnerb.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpuohjqw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/ggkwigevm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevtecttd.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeffuzdq.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdlhgqfjw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gqwpbmyqe.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdlbcitv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvlhnzyx.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gicvzjrjm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gotraptno.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqficecro.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gbagmzamg.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gktfhxkaw.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gozlfclfd.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyivxacr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgmweddx.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/ghpghgued.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gxazksqdt.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gaedtwzww.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gipamvwew.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyncomct.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqerhrsq.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/grpssjcal.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkuyxhpp.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gcdulzfol.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqkiyean.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gosxfmzij.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gfmgtnivf.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gmrfqqhqz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gfcydmjrr.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexuqeons.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfzclest.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gnrfzxnma.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gijfdbrbf.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gxodqjwtx.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gkmfhotoe.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gufwmkgjt.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmofhggwx.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwvzlfvla.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gurbkxrhz.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/giqedgbje.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqllxmrdh.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gqkmxtxri.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gfgefiznn.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfzrdcsyv.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gfciplbsv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gypbrdyua.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/ghsjnjgjf.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpgioopy.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gcqogxdeh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvsrfgwx.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/ggynvfkpk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmexahrei.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gndwrbdlj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gurmgxiii.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjgqfime.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gidugrarc.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gyocivyjw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gczpoecne.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkyuwkzo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gealsjfri.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/godjaptwq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwbkwjgp.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/glwlyxigc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gnxdqngfk.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmxsjiqgo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gphmymigx.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwqpcmsto.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtfbpyyl.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gdvapeyif.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbucvruug.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjxyrbwf.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqozufpt.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/grgdfrlcs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpftjndm.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcmztogr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkrcuxxv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlgbnowb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmuuungm.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gguudobxz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gpusqwjwk.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gctqecsaa.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/grforfooa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gligvzvyf.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvgqytyf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrlzvuxh.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gpooeggzw.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gpghuduke.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoahezlg.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpmvirbe.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gicxizlae.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhkwdjzf.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gtafxluzp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/guqytzsgk.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfnctwlo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwrevuqg.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/glztcvpwk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grpgnyogs.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gksuyyimb.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxifnejua.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gekzelkqm.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvhtplov.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwslzgax.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhgsxizo.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxzikicw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gnluytppn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdpzfvmae.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlxauiem.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqnyewzyv.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdmaylmn.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gpyeecfix.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvknqlsxo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubeollov.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gptaksqqu.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gkqvvkdlg.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gaaxcjavq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxpqaylj.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gppwffcmj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbojumkq.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gavctnsup.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gqmvxacek.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbppdesp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtghdwewi.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/ggynjzyum.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/griloeuah.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqoxtedw.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gcfyyyoxl.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gavtxtzqk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjjtgled.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/glmqpjcnw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcglnoser.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/grmngzemq.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhlcwpvf.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gsxzscouz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnrqpiey.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gmqzjofuq.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/grlppgseb.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/grfbyvcvi.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gytqglaqr.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gaxdtrmrn.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gsdsagkct.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gdmrquqzf.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gqotgbmgg.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gezfdlouc.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/ghmollynd.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gzxwfaykg.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/grjbblvex.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gymgvpguc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gjierxglt.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipjgtgek.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghshgkmol.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqglfvqj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gygzbprgi.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbnuziipj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gymkmwvxk.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gbfvgrfuq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/glbauuayf.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkytzquw.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuhzvqyf.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gbrgezugu.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gflbiqywm.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gzscazsir.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtwnzeai.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/geqrjemsx.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gkpcqkksm.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gdmzrbiff.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gefxehggt.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gowbijzah.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gwutpnskf.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gycoushix.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhkilzyc.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgmfinmb.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcvafifc.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gtwefskhx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gejnteqmv.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmohllqz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gqarcxskr.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/ggbvdwnsb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihdqtspb.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqglkkvkt.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnxmmbsb.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gvupofkht.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gdpffigwb.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gdqycurrt.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gtrgtzyoy.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gdgppsuhh.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gemnpraqj.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gfnmboorw.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhyhphat.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflebjump.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gvhmeydbp.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gpgfjkiqr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzffidvmu.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gepkwvnub.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gvuvqacgr.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfojztcqz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfqmqndc.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkcxnqfnr.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcrvnjtnk.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gegwpjjie.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsgejwap.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfgumcnt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbqooscrr.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgooofml.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gvnrxhegi.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gifbenaxh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glovhypnd.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhgysccd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcagejvf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajjgugeh.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhopsnnt.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlvvvsee.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvtcaibo.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ggefattvi.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glguosvxh.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkutpzbiv.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gpzjhrijt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/grddomypd.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gugwmrlxj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvujzuuzu.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/ggftfhhvc.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/govafxdeu.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkttjvcf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghisevqmk.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmhteoao.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gqdzchoam.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gysagmqzm.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrmqiyuf.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gxjnqfstm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gkaklwdqb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqeiqeoa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslhwdbex.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gchmpylnw.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmjbxhnx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gigcadswq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/goensobud.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqhieike.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/guopleufb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gwrtjfrtg.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gmepkxoia.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooeyojwx.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoaylcuy.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gaeeybmpw.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gtzfgsxoc.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnjzdfhz.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gllaoeeei.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwtnwelt.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/galtaonvd.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gtrfgafme.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnuskmhs.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhtcpazh.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gdntgprin.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/guhjdowrf.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gveulvttk.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/ggzmyylen.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gbsxckrpg.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gojayendc.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvhlgiqw.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepqqjrjt.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/grknaqibq.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gggywmqtg.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzqwmbit.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtacopuqz.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gjbwwbsbk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gkgszfknn.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgujzhle.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohdvicqf.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnogpxhw.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyqwkosw.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gujpsuuco.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpjxersms.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gecqzyhbk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/glskywcyk.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gwagfxbss.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gmgwhbgrm.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gzrebpezg.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gxwzxcqou.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghuabblsg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwarfman.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbttbtdrs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxriawwnh.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gvmscfcax.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gtcbcdgpn.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqwawpnl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzukedwie.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/grdfknivh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugfuedok.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gtfgfnnhv.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxidqpgxh.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/grwpfeofu.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gdavwjnqu.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gcnrlqbdl.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gnowcupmg.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsbohjkq.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqravtlu.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gtitjhyik.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsfzmkku.sHtML


<!-- 参考信息 -->