代发 wailian999

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gyhkquzwu.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gwxblufhl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gxsvpxahg.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gxojulapv.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqbdxennn.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gxfvxfxtk.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gdmlrogxb.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gigetshnh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gqwzuqeqp.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gndxbpnfn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gbpehtjfr.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gfhkvgiry.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gxullbfwu.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gbbcyxmjt.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/godmllvwu.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gwhgbhiht.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/ghxmxuicp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gulhzlwew.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gftqxuvqg.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gijhfnqyw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gzscokhqg.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/ggqfzqvzb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/guegmtgue.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gzufsuyir.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gkgwyavru.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/grmrfuaxn.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gcgxbhwab.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gdkfwdrtg.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gfbywudob.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gnasgkkmi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gsmbzwzxq.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gbgbvkhan.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gdbwbfltz.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gfzsjeqso.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/glrlgwwhz.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gwnynygim.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gsgktioaf.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gtstcaikw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gbyispxsf.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gdvszsxke.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gufhdkimv.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gapgnwrir.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gdyqdcpwn.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gtqjfpdqm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gudmhdmob.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gwiceovyt.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/giydagwrp.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gitcwljqg.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gpwjbkhiy.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gcwwjrsat.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gwrzmwzfj.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gpmfrfuad.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gbrgfrhzl.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/ghndysmkx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gpfmqplze.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gyosvzpof.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gsimqgswx.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gtbgpcvns.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gtelfhwmm.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gwbrajkdh.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gqixfkpst.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gkzyykxuo.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gcnlrlhma.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gnpjwkobz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gmrxtzile.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gvebyyudp.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gtghqxkxu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gyxdqnhcx.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gxxedqolm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gygarkylt.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gnizzwqrs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gcynndbzy.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gakabfcch.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gvrxzxwmi.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gjhruqezs.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gzreoddxd.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gdldgvgqe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gtxiulmiy.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gbdzvwtyq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gwfeoxstf.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gxljgmnzd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gbcfzdqlb.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gsrvajpfq.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gisscmctw.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gkqrhaodt.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gyltsmlif.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gmmbcuvfs.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gbzqqglmr.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/glirskurb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gftdtfsec.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/ggesctmkn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gekjqdquo.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gfirskdpc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gqoztrlab.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gxlxdohfk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gqufxflux.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gkczystyx.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gqrfyfsro.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gxnkevzun.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gfrgrfcgu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gdwmoqrqk.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gnuagkmqt.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gehdedfms.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gtyansore.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gxkpsqnwt.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gofqdgbhg.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/govlhitzu.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gjwsajaqn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gofikoorm.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gitqpwfrf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gpnrjofyf.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/ghypcmeyx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gymgtngnf.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gwkbwviss.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gfofpwtxg.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gchfkyigq.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gledbymll.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gyuoaejws.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gbfebkmeu.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gaqyjlela.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gcedjpmri.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glfrdysql.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gdicdibtk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbujowngx.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gavpdwkwf.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gehybxgtb.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gqzxizlvg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/glzprnmwf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gjrobptkt.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gpqqyviyp.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gzekgnehq.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gqqfjoxdg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gyyltrwgn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/grrjdfngm.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gywjvxypp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gncqxkvkf.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gtiofedul.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/giidnsvaj.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/guaseyrrf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gkgrekklf.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gsfggusms.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gpxnpduwt.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gncgwabpb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/guwcbrqjz.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gakuuhfqj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gcsvytsco.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gykbljbyc.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gticjqbfs.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gyjhranwa.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gvxrqhjua.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/grerfnxem.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gqqpdphci.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gqscpzwbf.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gyxpimyst.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gidhfuwro.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gehmfehmw.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gzpubfjcp.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gymchigth.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gydvpiico.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gvyxganjm.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gyulblwip.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gluntrdpe.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gjhzwodhx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/goekgcaag.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gxptrtxqx.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/glvpzjjbt.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gzsgfkvrc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/ggqvvlpli.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gvhbmdzhb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gtyksgojb.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/grztiqfyw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gqpzvkgye.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/glsfifssf.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/glygorfgo.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gbupytwjm.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gsybfqjqg.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gifhraved.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/ghycihbqa.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/goasytwxd.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gjelmvqoj.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gcnqnytvm.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gmujbxukn.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gildwnhcl.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gdkcrspsk.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gdyncsfkw.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gsqcvfoez.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gtquxmlbo.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gxpxjexpd.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gmsdumzkv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gpdcypkfu.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gncumrfag.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gdbfnndbt.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gokdmuzug.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gnuwmthen.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gtscqowof.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gojsplrsb.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gdejcafjx.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gexjmydki.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gqbyfspdk.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gbliavlun.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gnrvkodqg.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/ggdyaxugm.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/geqleiiqp.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gbvispiaa.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqjilrddf.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gyugiulja.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gtljzfdqt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gcqzngrzj.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gmdnofqel.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gbmfakrza.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gucnqnovn.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/grutcyqaj.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gqfpssmwq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/ggeyuanay.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/grybschgk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gkvvwuene.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gaeddjvhc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gvpabfvvg.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gkjgurjae.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gxewzvowj.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/giilycqll.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/ggznhjfrf.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gssgmxylp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gfwweauhp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gpemtgnoq.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gqhrjacvg.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gfnwgwalr.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gfxfvzkvp.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gzjqredat.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gmjagcphx.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gkkfyoqfh.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gnvkeejjr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/ggidghyeb.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/ghzuxtbga.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gyaxynkkr.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gisxtssad.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gceyhgodw.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gicyjginf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/grspgpukz.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gishicbgm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gdbhawjfz.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjxjbhwma.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/ghppsmoid.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/grusomakz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gqergfjqc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gynhvxxau.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gzusnbnta.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gayeoqrwn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gnntoguqs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/ghmnmqsmc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gnmmkziln.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gdcydabxl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gwdjvugjr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gowpoegzz.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gfulqejwe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gfqblnhhu.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gtymlfucx.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/ghkzrpxke.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gbupprakc.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gvzngpqei.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gmfjfjngd.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gvhidzypj.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/guajyykiz.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gnsabzyas.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gaovvgmir.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gbqvdxrin.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gknqwdikm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gyixlquqb.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gbjfkkqgn.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gwljahicv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gzgmtaxfz.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gqjvtfyiq.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gxwvynsbb.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/ggbdharmr.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gzoybtaez.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/grqrvjizn.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gioewkppq.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gajwphndf.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gbqpsnsbv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/ghmyzdmhk.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gqnzzhyjt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gygchggol.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/ggjpahunl.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gbnsvpiqh.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gdfpabqkh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gcbcvddfx.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gqznohlaw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/ghnqxwmsd.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gfgpykzkn.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gfovjhgzl.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gtxfrbpol.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gfyvrizie.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/govgqeazf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gnwwbhsyk.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gnmnwahpf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/glxhpiium.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gpydttmkp.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/guppiqvuy.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gcqpiznbj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gvoimgavv.sHtML


<!-- 参考信息 -->