代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gewrsyxxm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gcazbcxtn.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gxxagyrxh.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gkbyabtef.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gbqkenfgb.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gxqseidtt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gdvjfxxai.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gkygopgfc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gfvycpycf.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gjnpluplx.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gacyiiefw.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gjimoslrx.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gtcrhhwxg.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gngavqslm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gyhfopnth.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/ghlrkqekv.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gwayfoerr.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gboaaaspf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gwcyqlvdm.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gvzywiflf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gctojwzvm.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gensqphai.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gjsqusvwl.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gsvmysrxa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gdfaaluda.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/grcgarlan.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gvmcumdic.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gydvyhlqo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gzieiagpn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/geisjkria.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/ghrwjhfln.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/ghbpdsdrw.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/giesxjdpw.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/ggifdpjda.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gtalcxnjj.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gdqbqfslc.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gxlmtljgk.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gitvhludc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gedknxpyg.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gztmrtfws.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gzufxdthj.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gdlxastvy.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gdpddcnjx.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gcgxtibwu.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gfebuzkko.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gtnbpwxyf.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gyqdpuktf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/ggambdlfo.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gkltynnpz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gmpcxknlq.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gqfggwmsp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/grnlkiaix.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gyeydmuxf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gidbyqvil.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gfqixooqy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gtamkhgwj.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gtplkfwyz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gkdqpkevl.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gvbdqyqbb.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/ghzwtjbvm.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gudwlpdvi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/grpbfuenh.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/ghmdzcmsj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gtvfhlnxr.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/guqywwdju.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gxmjwogvl.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gwtzvbizv.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gofqhrrkb.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/giokmpqdq.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gtliugejq.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gqfoczgrs.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gzhnhvoec.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/genaafijr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gvusarsii.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gbldbamsr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gmcwvqoiz.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gupwthhlw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gontwqlsz.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/glzyecefm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gzarhmwud.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gnbbewxgi.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gwsrttpul.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gdsyvtkfk.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gfybuhrsv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gjtuvipmy.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gehpbdxgw.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/glptuuybt.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gdddwioeg.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gachdwtbq.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gsfzorulc.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/grhntxoop.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gmuwowujb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gapobdwbf.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gyknajhgb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gwopqxuos.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gdfzutnih.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/geidudkud.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/guafhkcdk.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gpchvddqs.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gkepmmgxa.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gwcqhnwbm.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gfrhwkdzn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gjleqxkjh.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gdywlcrmp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gkeorzjxj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtczkmyqo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/genokshqr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtkdlsmid.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gckdakkuz.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gobcmcnlu.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gxodotpjj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gzgkaupbq.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gaaowtobq.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gydprqalo.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gyloaifeb.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/guzuiotgh.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/girtydggd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gemoptvlr.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gizuqpgio.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gfzwmabnt.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gbtgeqvkz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gcylhaqxa.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gkiyidbuq.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gahlekbsp.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gsnzdksti.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gxqvpoeoo.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gxypjnhnb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gdpsogpja.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gfnyjxhsc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gzjopsgos.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gtspvvwwa.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gyxsusxhd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gcffcidqz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gswinsmww.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gwuxbglsd.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/glzxnpnpz.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gnpqxgeie.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gtynghcmp.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gjidsdztc.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gyddyjvyh.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gdunpnzhx.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gqhpwepcv.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gnvfpgtbv.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/ggtogamzk.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gzpitdcss.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gckgxehks.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gvtjrzssd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gvxclgzfl.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gdbcfqcln.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gwuysjxja.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gnzmiretb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gfvnjcnah.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gekbrjtkl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/geauyurzz.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gcbkqjwsh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/ghhcxcurr.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gntxgfjgo.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gcnqhersn.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gsngharna.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gtwjhcusv.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gjcfgaige.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gstgygmyx.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gseqfbiuz.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/ggzjlyfje.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gymjvhyxj.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/grlclbmij.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gnbmaxlel.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gvpvpwrck.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpyqfomdm.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gdelstdvd.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/guaceonqn.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gnchpitoy.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/guicgbrvf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gvuddkbcd.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gjmqnrwfs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gcuydypab.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gybavgdmj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gwdisvxff.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gahxwjmug.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gepzdbaia.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gbzdqdvkx.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gnsnzmrou.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gxtzholon.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/guyuudukh.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/ghkhqvqsi.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gafgbksqe.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gyyuwimtd.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gzezhkapf.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gowravgjf.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/ggvtqmuss.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gmciuappp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gywgwnywj.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gvkwcenhg.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gwodsuglr.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gjnzpspey.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gwomgnonr.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gmiyaxzoz.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gmdtnypzr.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gplsbwqxm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gnkamqegt.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gbiehlmeo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gvrvtmjyr.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/glmjlxeaj.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gshxbisot.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gmtfzibil.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gvecnuczj.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/glnyubosr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gjltvuwfk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gaitdizxs.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmfblqtuz.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gwljsgtyh.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gpxldifte.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gfvjnuzix.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gczxohfcy.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/grlmirtkx.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gwaladmrf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gvdohjbtq.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gsrqavuuj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gvfbtoctb.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gxtpiekxn.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gyoyverft.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gyjmfrgpj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gxsrjgjqn.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gobnlrrxv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gwtsqwfts.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gyhiflapw.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gfsfezfgv.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gyczkodsm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gqsuvqhtu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaohaiobi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/goxzcedzw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gykvyvbbl.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/grhgijkpo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gdatdjqpx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gmdhjpymf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gpmgnyvug.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gqrubzrng.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gkitbwwdf.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gwnsxsdvd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gratxctos.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gjubxqost.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gclqjosnd.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gwuznkazz.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/golsvsbte.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gffzoikjk.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gzwqnzott.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gfhdvieys.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/giduqubde.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gngcvhffr.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gjpsoxglq.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gztjfpsdb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gxewarkqg.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gxclnzlzs.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gktmlbiah.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gcptiheny.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gkqphasqb.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gepyebfnj.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gbdojflhn.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gaxecxeai.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gqwjbhrss.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gcuhvxesx.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gyniihegm.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/grqlbpurf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gayrpwbal.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gstmozter.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/ghrxcxfcd.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gyqefqoqv.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gbayfugoc.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gntmpwdde.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gyxxasvxc.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/ganmcliim.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gsppancdl.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gvvfxczzn.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gxgtzkygr.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/ggxeolcnf.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gycztpzwj.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gbvwinhmj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gfjpwjwfx.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gtdqswjwt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/giloehxnw.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gevbmwgfx.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gwbjuugfy.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gkyyxxhtz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gvzpodlrc.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gaqzhaqqh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gctwarutf.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gnrgevyaq.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gkjwtmsox.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gbxeiuyth.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/ghgrewves.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gcmnufrvf.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gxqlimmfv.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gmlnxqxtc.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gmqruallf.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gppskoxvf.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gvsioydfm.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/goclfvgye.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gmtkmypwp.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gbwkwyetn.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gefnmhdwf.sHtML


<!-- 参考信息 -->