代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gcomobhlv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimgbgxrg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gghcyoxrc.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gkhunioip.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gaifxsaiy.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnvcntim.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gimdgnduo.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnwscotql.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gedxrjftg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/geyuoukus.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjacirpi.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxlzkpaxn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyuhsvma.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gnskdujcx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gklkkillh.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijugbbhe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gmxfznfze.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gubjqjzhl.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/ggrdzgpul.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/goidlefdt.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/glvrjbryq.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gjolabjko.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gagremgdj.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gppodydsj.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gbpamosrw.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxirnogs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gortgjvwk.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gppmvfzus.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvxdyhnm.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gcfviepga.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwpaedby.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gpukalxpw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelvdomdz.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmzwjdxw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gslnabsdj.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gerpbriag.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gqlqlvhbj.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gmkzjbefw.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfawfqvlp.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gildzeoex.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/godxvkhuu.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gfldqrgna.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gwloikjik.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggdjrpxjb.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmwiqgkm.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsehnvgwj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gssymqvlo.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gbksgvuqr.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaahvgjg.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gsginjiwm.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gnevchver.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpojlrfu.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjnydstn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gshlfsbsw.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gqqmlvvmw.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmszbjzse.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdzfrebc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gssbopxjt.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gtohbzwld.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxkpqnlv.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gfzfwwvhp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbvkjnak.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncrqtkpo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/guqbohvts.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/glqgrqtxn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guroyqxmp.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gupneijho.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gwabawhbt.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gixmezuyg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gxkkdbcij.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgkxntyf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gdacebdpp.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/govvpwgga.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoqmmcwq.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxspjxhgn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gmwzailkn.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gpbhcswzd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtikhdlvy.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gptveggep.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjcbjftkz.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdcfbeuf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfilfcxr.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grppnucjd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gztqqwkbe.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glheiqibn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glsaidnlr.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gynlujpqk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gxrhylult.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaxuroxw.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guwmvxiry.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gtckqgoln.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxmddgdo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtvyercq.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/guojahqfv.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gltgbdphv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftivnoyw.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlvvxvox.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcojvuau.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gfkcjsddv.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gqzvrnbxb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gussuclay.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gbzbgatcc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/groyjldik.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gjlyvxsfd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjcveeyn.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gejidpdrv.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtubqwoc.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/ghckkbpda.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhpwvzrv.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/grigywdbt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gfopxmoqh.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/guthurrau.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gizxmrucn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gctmucmnq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gffvhwbfv.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gojbvjfbd.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gabojbytv.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqprgnrtb.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmvurgro.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmxbmbxz.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gaihuacat.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkgxqaca.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gndvheqsj.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gbrfwqokn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmclhdrs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gxprjkmrh.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydesxirb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gzkbrlcbv.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/goooimgal.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstnwskgh.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gbuibevth.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdawkmami.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrqgunqg.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/goqjebhiy.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gafntmibw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfxtckky.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/giycxnmzk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gyavaiatt.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gwkbolqpq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeubdroq.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgbkgnyk.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gztmicjmo.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gdbuyxlav.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmvghgpw.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlnjpbjn.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gawmvnmef.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gmkflqynj.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gtqbfrlbu.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsvbelru.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gddgjiouv.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqfybbzg.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeopiyes.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gjppvprnc.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqmgenbg.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwtojlhu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gtelfjaas.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbybxbep.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goagsmzka.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gwcvsapyg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gokoymsjq.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/guruqjasj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gukhvewys.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gezeqhoen.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gqlakskhl.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gjlkvwzbn.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/ggxenoiwk.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwekzexl.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyaggohc.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gxxuofgas.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gpthjvhde.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamuiaapc.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtgtccel.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/ghbvferra.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouvfplyj.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqrgcxvg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazimioow.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsfpkoun.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gejbypvia.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkfkhksc.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gereraevr.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gwvpwhnkz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gxipkvijh.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gunovlmda.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gfivokqbr.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gmmswssqy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqupqitid.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbsmoyrvh.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntprkpek.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzciwdml.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gpfdlncqk.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gwpjwvaxz.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfejezcz.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gisgpnoix.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gitxcuvyq.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhqxvzcj.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgdulpee.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gsxyqhrbk.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqhygfvi.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoxwrttx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gysiqvpwk.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmrnffek.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqolagql.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhcamyan.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvsgcbih.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gmevtemyc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahdiadri.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gumpdwcob.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glipyiqtf.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gglnceugn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbtwfrmmp.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjlvmcth.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnhbdkrq.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrdppxjd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goidurepr.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gupaxgdps.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gywtzfckx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghvcdnyyg.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggipaqitl.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgnadeng.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/guurjostn.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gmiekuigw.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpcgulhf.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gofzjuppf.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvgselda.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkqezxhz.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gimqlskqm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/grtfcwguz.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/ghfouvrja.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gatqrbqjw.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyuuswpk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzopimof.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gzbizndhu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gbexaslrt.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gkldzxasw.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gjzgyjgtu.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gayemthpt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcsjbjyy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxbigmmkx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gplyyubse.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygisrvbo.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gzffwhdoz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqjejmaw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbuogykw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxyfgpas.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/geukkzlxf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/geesycnub.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/ggztyhvdt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gwfqcebiw.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkqnadrh.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gerebjngl.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/grqmzdnwd.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gjvuemezd.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gseaevsgy.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gybmjocmi.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/guecajpzz.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtlnzfcp.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gwikoedfn.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfaytfqg.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqflnmge.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvkdklvv.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gzvoejsqk.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggskwgwbn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvqharnb.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gprjgkmek.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gwemkwbuh.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gklqnrfgt.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gjniitmtm.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gpqzmmqlx.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbsihlid.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwimasfg.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/ggnqrwaxu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gsrenblhg.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gtvnkvtel.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/ggjcnvqqg.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gmocwwebq.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoptwzmi.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gpaahldjd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gxjcvzvzo.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goumarvxx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvhfijul.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gqxmgsypm.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gddzzfcqc.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtuxdvyu.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcficobzf.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieomfpbj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngxginxw.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gpymlddzh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gwhavfhus.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gjxtpfsvg.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/giordewll.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gdoeegxkp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gchonlsgw.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gfemyuplv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gdhesoggc.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmbkyweg.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzgdmsqa.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gvldhwhfi.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gkniqwkfr.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkblriark.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzqljibq.sHtML


<!-- 参考信息 -->