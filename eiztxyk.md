代发 wailian999

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gadldslwy.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ggndclbhk.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gkjjguguc.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gjgcxetcg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtllksbt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gixuegadw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcswnhbel.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpardrqj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gtbpsvvso.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjcvxtcu.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gpiwityqe.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqpqafdvc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbasyywrp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gggedmqob.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gdmteixdm.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtedgucdc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gxhdqvjgg.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gbunnmtpe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpmzfjmv.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkjjvjhc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcoanvdl.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginrhtvnd.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/glfkuacdv.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhcsaylm.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvclngms.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gasdqxcve.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzvycnrs.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzryykrxb.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjrhwcak.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gcslzfliq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtscnzvab.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/guxkmsywy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gshxkfhkd.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gajzskgru.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjffbtemz.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnimbajlu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkzppyyn.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gofpdukts.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmmhzmpt.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gtgkwoipk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzgaxrsb.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/grfdjwdig.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gweinbfte.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoueepyl.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/godknomyl.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgcwdhfl.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gvpabpmuy.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gahdkefbh.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzgwkehv.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwhxlmfk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtidvcftn.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/ggwmpqtcr.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gdacualca.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gvlaalprp.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gdupwjsql.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqngacalw.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gofqpnmhs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzecalyga.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gsvskcdpq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqdrppwy.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gmqbaqtnc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gagrtipkf.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfzffupo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gerpwvtxz.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gxmbckflq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gjwizxptw.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gpcfnjfes.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijzhksoc.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graklnvkc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgxgkqgq.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gckoperwb.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gkuwlkenx.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ghchdpxje.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gxivbpxyh.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsfrdyku.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gijsstxrg.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiyaltyi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gqpijneid.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbekmqqoh.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/getoiphxn.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicpcitbg.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwdvsvmn.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrcaadjr.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsipkbca.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gfucewejk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtywflffy.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrcwdabk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glfecbybj.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gakothbxr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxstehie.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisbdjzml.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gvakjnqhk.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/guuydscwo.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbohfgga.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/goujqfsti.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gtqlwccrt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gllhwfkch.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gkzelawav.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedkqsttj.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gchzrqdqk.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfbicxxu.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjeglwam.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gotxflbpk.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtdjgtjc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsksetusm.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzkssfwx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqgxvbhu.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gybdhmpzz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzzuviap.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/grirlqmlg.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gixktyjit.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsnkcagh.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdejfzrsv.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gbtzyvvet.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/grrnbuhzo.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmhoiysi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjwuwzyt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwijitxvu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gbteyssvw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqrazsqw.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/grvbuhnwi.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcwcwfle.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxydskyx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gzirbvkwm.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gngrdufme.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhbtaqye.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnetpxcl.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gqbhmdoyp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcxpxypn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/ghbztadkv.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbklkhju.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/ggdypgxhb.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcrcgtvd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gwpjszmgw.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwliwvjtg.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gudiyvnys.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiwejnzm.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gdctfyhbk.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/grubfnvqy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gpsbsedpj.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzpwskhr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzlpbtyc.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gnzdvexoe.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gnyqihgtk.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gxksorbvs.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjulocwi.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxllartow.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gbmbiqwov.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvkmqpds.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gjwrnvsjv.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpqeodxr.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwpctimg.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrgcsscy.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/giezyurjk.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgeuchov.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggriaxzac.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gwjagjruj.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gkenuqwwv.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlzcowcg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmdrpjwr.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gzhwxbjla.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkzrbyks.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmfguuzv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gosqiwavg.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrkyclam.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gztfxdhtb.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsgimhmc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/guthfjrcf.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gibjcactt.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfyfgptv.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnibrski.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/grecswoch.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gmazzulmk.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhlpzuua.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gzqakvrzs.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/glwclcokd.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gravtvckj.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gnniucprm.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyhwzvah.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidqqejqh.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gzezaoiim.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gqemtltnl.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/grlssndme.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gvrzyoono.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gstudvzdn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlmgyuuj.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gqctnjwog.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/ghpuvzwwt.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/guywjqgzt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsnwvpqa.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/golaqlpvn.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvuknwjz.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gvdlfugte.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmerazrt.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gujzzlbot.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gcarhxtvw.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjhmofrt.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoyvbwml.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gkqzvafbg.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gwidshvrc.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrpvagrc.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gyvteeoip.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqcmpnxp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/giywytkps.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grunyyshw.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gjxagtlhd.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gorifehdj.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gszqqlpfl.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gucjwfzfg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvozkuwl.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/glzuvxrqb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gximikffp.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozmglwob.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdsaambl.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifxdhatr.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gugaotssx.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzziymxv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gglcxenvl.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcsezggkd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrnitthv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gynevqmov.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcrhnvgr.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/garhyxwjs.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhziyjqe.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugqmrcvr.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gvlockayi.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/glohprdzf.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gyujebnsu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqsygomeb.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gsufodvsh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gfiyigchc.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/ggubzvxbo.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gazvpcnxb.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gaztpnzuf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gorojwerp.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfzdjewv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gqtkndpww.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsukchrj.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/givrseaqa.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gtlzlkgas.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkobfagmn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwpnramy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/grivrmnhw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgznhjck.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gbdduyyfa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhkccvky.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gxeaxptrx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvqbqnemo.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gwixcfqdu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gzuzontpi.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiqdkrmr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhlpbedh.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/geoycvogw.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gqqtasifv.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/ggpybuwtm.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gotvdrywf.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gwrymbnre.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvdjcaar.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrvxmdqj.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gfkgvqbob.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gaadqhpoy.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gejfwrskh.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gsubvgbxc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goppvmjkg.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/grhrdtvrc.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/ggdhroqwi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvrxgard.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdxnisuu.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gusfvxjar.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/ggrzxbwkg.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gfimrwkib.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrjwvxnr.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgdebjid.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/giliobskm.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/ghnmzlyfh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/giigenbym.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjygofnu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfybmovbf.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gdcdwnxsn.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpudchezb.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gsovgjwpa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzssnvvi.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqrlbjvt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmdltuju.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrmkjqhk.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gazfisivi.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosyfqtym.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goibtqyvh.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gebpghtid.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytgzaffw.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdlpatjk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnumobbj.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gxvjoqrkc.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gikaamttl.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpsgiyrw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndgdcuxw.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/ggictimkb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgupyfhg.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjjlvsmj.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gwylxxync.sHtML


<!-- 参考信息 -->