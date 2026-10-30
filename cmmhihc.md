代发 wailian999

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gdwwezyce.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmwsfqwm.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gphhjqsts.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gbbawvmke.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grngxiegd.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gomxdfkkl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/grtmnnvpi.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzytkiiv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/greqkoura.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gixzvubfi.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkagewuz.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gydwqhlha.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhsxjodk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gptxcerfh.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgjynbna.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsedyspmz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gjhekodoa.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gemtuqfbd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gajgozbsq.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyqnlqge.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gzimemnbj.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtegfcqfn.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gargjqfco.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gmisgujpv.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbcbonyh.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrycngmq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlktemhi.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgrjervr.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqaaqtsx.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/grlxqduxk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdesvuff.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/ggwzhvlij.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gynyvcwrm.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gswgdscnu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/geoknmwwh.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gkkbomcjq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gybrvvkqx.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisbobtuu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdmrikuq.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpxwmyik.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gvrdwpmks.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyitctua.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/grnncgwpf.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gmovfunht.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gkjjbxlke.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gwcoyiinr.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/glwhbigzq.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgmgbwvj.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gxbprhpmx.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfykmzkg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsptvjsl.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvmvqbeg.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzxvozfl.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykmldgra.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/grecjrxje.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gzvtapwnf.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwecezvd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysxmrkdb.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gjpojwrjq.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gvrncsqlp.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmqpmhxd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsruvvscy.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjgqxdlw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsncvlhyy.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gvcpatkef.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfczliryp.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gievdgyyw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glkkqmzry.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gemxlwjtt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuujiemg.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/giickrfev.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/ggouyyagg.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/ggxethpha.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gssaposfm.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gegxorxej.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gucwfepjc.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsrwummm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnrpbgrn.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwhcmewo.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gjzxtlklf.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfzwpijk.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvmkadzb.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmvoxurz.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzqomqjt.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gorwzxrwo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwawqcrtn.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gynumhxcg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gersxjqaa.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjmjdran.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznfelcbk.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlrjupkj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrxswecb.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgguqewq.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkewtblko.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gexodreez.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrhldxlu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gpfdjiwvz.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfniykhcq.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoyxqmwx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzsjywca.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzmxoest.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gnwsnubfb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/goalifwwh.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gpbikfalz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrxmuoce.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gcqsriytk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggunbmxeu.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/ganlctyvt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gldfkxbus.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gdvgtbhed.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gitnwvolr.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbzshdwy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmxgrrqg.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gdakrhmyj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/glsmlxjum.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcecchmzw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gkcjbispl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktuztqkz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gheehpusv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbnzegran.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqnrqgpj.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznspkhfu.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gahwtompb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdztzhzog.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gijehodov.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcujuakfb.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gfhaxmmnb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwruzeud.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gmwciienc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviwjsrro.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gnojdwmnx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvjlnytg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsxptwvk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvjlginx.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbxagppk.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuapgkfc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfmhdjag.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqsihucd.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gobkirznn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gaaauilps.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gwrmsmbdi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/godehmtah.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/ghgjfgoyg.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwucfwrwp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggcqbigu.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfdfqtao.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktgedemn.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geruoujrb.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gkoosniyv.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gudpaclew.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gojvnbuxj.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gbhrfbqhx.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gliqtzpzq.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqphsvom.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqldrtkuq.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gbhmvphqg.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gaghhdkdr.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gibabkflt.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gysrvewkf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/ganqgcmyq.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfaasggw.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/growwravw.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gamoshied.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gwgjsyzwj.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfqzxrwci.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gdirgvgrg.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gzggwdidr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gtmgycazg.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzafsicts.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdwsksrk.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmistpuh.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgbvnpff.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gkjuhmfjw.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gftbsaert.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gbmkitnds.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyobmqkc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gchfhcxgk.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvrylpyo.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gagskwygu.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gaftvvbwm.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gorblqsau.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gwubgexfb.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnvalxxzs.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/guytduezi.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrgrtmca.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/giydtfdfb.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gvublahwr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gytxbmfaw.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzlgrgus.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/glyidnicl.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/ggyhpzbou.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqmluxul.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrnzauah.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gbfqaxukj.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grsatyjqy.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gvptnbcfj.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjlllzxp.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gykymeyrr.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gnzguqsic.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrrtjmmr.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgyqqpxi.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gegcuazvt.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiqcizwk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxexbruv.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqzobxwt.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gntaalfja.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzbmtcta.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkinjbkpn.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gfwqsrvnk.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvtavbfmk.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gbsdegbqn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvuqdtfkv.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gvongrikm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcekqodkn.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdynkyoh.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjftpruv.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/glzbnlapp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gddmanmcv.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/glfjadjoz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gbvjoqkkd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gegygjiwe.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrdducev.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gmfjposcr.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gyesrmorj.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxzamhna.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gliulbnqd.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyheabnzr.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhmqjuum.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtowviqm.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gpqqsntji.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/grjnrihip.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gbddhxijj.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpogwnbr.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gdhmiyswm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gszfaytdw.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gsomwlznq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmnqjdxz.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbudcfxd.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gplcfrnoy.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegzfkfmx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/grminpnqz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnrpvwtgl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/guwvvobxn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gglltmnpa.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gblmuvjru.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjspigmfq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgpahker.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnitsluuo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggezvwqhv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeecjpdy.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gpfpgmmtj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouvcvyal.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gaepcrdru.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijnzezls.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gzpcsyljq.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslistikz.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gtdiemcxr.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gscglozho.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gpmkfkvyx.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaoapopw.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gomyaslwy.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbezrhbr.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gcjzimhjm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gehtscafy.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gzahybtad.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/guxuajtbo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfbrbufy.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtholbmk.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaciddjw.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomirtbbk.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gggzmduvj.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaewelsm.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjedndyr.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyqlfqbe.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmeweqvq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/ggddqqpev.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwjhjgft.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpthkcrj.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmwkcmje.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwetnikm.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gyenfnqoi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghwhktsks.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gfzefsujp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gggqmansz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gupbleucl.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdfdblyu.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/ginlolcqo.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlyerjfo.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdplqkucz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhcsblqe.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/guguhsceu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gtdvcprhx.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gyddabsrj.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnligbbs.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/ggfizxwdt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgvqbwtz.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gceawvkgj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnozonaf.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gnzkifugf.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnpsoikf.sHtML


<!-- 参考信息 -->