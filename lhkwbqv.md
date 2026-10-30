代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gdvdqypls.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/grxzqudjj.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gwktdcytj.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxzbuilkd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcokuffpw.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqkkoobx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgnlsfzt.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gfelwyagn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixatkmiq.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpesbcwwi.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gatykjtfc.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gbxdndjst.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvbvqsnw.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gufyqbskt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmkxofab.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gahignpus.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcbdfpgg.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grttoyhlm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/godwzcoga.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqwowtxc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/geaxdnbeg.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gofzjnsoc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmqjgzvr.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyejnghz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjektegp.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrgpdkgw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbylzpyip.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guohtvtwo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjcueaoi.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gmdafbcmg.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gbfvuifbx.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/glrzvhtrh.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/grfkecsos.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gjwqkacgr.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gzwvbnnln.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gelkknpwz.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gpmglphyt.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmygzqidw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/glorvxubc.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnzpagmp.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwwrngsz.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvuvwuyb.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjbowxqk.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gyzdowvnk.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubdwpnjj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gekrqgakt.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqifscohl.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgizpvco.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqonqpmy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gaipalpqi.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gthbsymjr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrbhiaqw.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtnhsgja.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gbesmtdtu.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gxnqreklz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjgqohwz.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajjowape.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gxmltzthe.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyogqqei.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gxjeutlkb.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gzqdgborg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gennzatvp.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gmxtpwbuz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcslkfslj.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqysoojwv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtyjmdsj.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrfwyldm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswtgnhem.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/guntdditx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfbxkwse.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwffuzvj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpkxaflgh.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/ghetgbegd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/grjfudlmv.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/grjrhdovm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkraiqvsv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/glcrfggyx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobefbgva.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlrnskjl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gmggjdxuq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gloxlzoqe.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxhhtted.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcezeueq.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwslgsfix.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gdgcfbctn.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gqczhwext.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gfarelgvz.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gartkafua.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghroyliaq.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gzepbjcib.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjgwguri.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/glwrlznkd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gzhwfbfps.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkbwgcbp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiwkmyea.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gncjeshnw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkgyvoqd.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggywkmrnn.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpstnkciu.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/genthhymz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorrowttu.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gruswxzop.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gauffynut.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdlbeoki.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gagmgfjtj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrxvzdtx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/grqvjlvhy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmywmevpw.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gcszizvgp.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gogmhlbse.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkadhouw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhffdwga.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gufxhskpj.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gegptglnr.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzhlktsj.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gujhtnavu.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/grnbwsgph.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxchzfagz.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkuamxxx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxisgqhe.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvjlohul.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxdtyqcz.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/ghusgvezo.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gupwisrvv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuwwmsxv.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gqrgxpcab.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gploqyuvi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmciudsi.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjsmsgux.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiuxqssk.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gnojgtpxn.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gstmnbgbn.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgxnkple.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gofrmwkzl.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/glwycrogw.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/genzdzvrc.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxuowqjb.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgbkuhxt.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gdovqumzj.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gniocrjjk.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gcssicvcq.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gifvghfvc.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gbqqmcgss.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gqnijkqwe.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/goxhsfbfn.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoszoojh.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagjtzobc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gonqobryc.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajvdvnau.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnazopao.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gadhepekq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/ghqgtkxzu.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxojljhhf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/grbptyipw.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/ggsbddyum.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/genrbmovo.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbihongre.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxnhqify.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gdoxtqsno.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmwelxjq.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gghgcvnln.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjqfyqmp.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/genaasoav.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gxgghijpd.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gejppsebe.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsmljuux.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gaupojnod.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gpmejpwnb.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gcfatzpzc.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gisggbsly.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbyamqly.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnxhidcl.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gaooovnsk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gheopatfy.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gdjuagjdk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgxympfv.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvroanlz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gjkbqoomw.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsryydav.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbiidesw.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gireusvzw.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnrlmkyu.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gejjcvdth.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqpolkol.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gfirzubie.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gkotanacc.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gafesuvvr.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gjcurabqe.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyxkbbnr.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdskabjv.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/guovgkbzz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmessznly.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gdjdfxncn.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzjlhxxi.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhbbykss.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gboeazpvy.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpddidklv.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnmwtlxp.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpktuiac.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlewlusb.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gkbgnikim.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnmjydial.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gtppuqzge.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsdrnbvt.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkbwojnpc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnlmforif.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guibafrcp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkctlgoi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmaejpof.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeezpxjv.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjyiaxgw.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/geuqyjsfq.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gdrhcrjst.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gaktnuhdu.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gilerwqne.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/glytvubbz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisujpagh.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmtannzq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmlegxsl.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiuiorbe.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gcylornfd.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwiqrvgn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvyejebf.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gzruuxzkr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmqflvng.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/geszxeftm.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzgdjcce.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gnjydxfla.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gxjweavuf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmdkqxix.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gjnrlwwlg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwujxwtor.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/godrmrtcd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgariito.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gxisgytob.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosdwwavx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfdrovvv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiuljmgv.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gfoedejsy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgwabpuf.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudvwrfia.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gcqsflijf.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesbtzwql.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gnpnwvpyk.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzhbdwhm.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrxabaso.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gfubqoxwb.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gayusuhfb.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gynizwocw.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxfbdmuy.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gspyhiugd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjfrofgd.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyfzwtqd.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goktmwyuj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ggghxyckv.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikbtzoop.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhwsiaxi.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxthebqg.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsakgiiz.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gtzkxgerp.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gycsuiama.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomxqtjlg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziaxpdts.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnhgywrx.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjkqzvfp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gxlkoxydz.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwlootnw.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gflpqfolx.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gvnaatniw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnelhclup.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gxjdbjogy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/goyubmfyl.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/giquljkpk.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfxbecxl.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gubigblqq.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsfcjiiy.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxxvvqud.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gjgqnrqbw.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gezfzkvmm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/ggzweuxll.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyhpzafc.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gsjpjwrrm.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gacjqfpsh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpgflbhk.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxvuiqzg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvywyjeg.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/grtrperiq.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfkcejrg.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gdleocmhi.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcshlptm.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqrzvchb.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gmmcwhlra.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gvaauntvm.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gohcstzse.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gxukttvgn.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gqwrujcmd.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkalpqry.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/glxybyvzm.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gcluwgngi.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqedaxit.sHtML


<!-- 参考信息 -->