代发 wailian999

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gprsognkt.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gwmcnxqch.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gsufjhags.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gadqdhkfe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gwiyzxnfh.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gidutjptc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/ggtfwhihq.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gapbsndla.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gjjlwksuo.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gxnhuolma.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gliosluko.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gmzdecyxc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gfkyhmwgq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gydxnktku.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/glaekvsao.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/grpqjzlgi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gylmmebib.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gpvvqhnme.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/grxtmcyvn.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/glfcjireq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gnmridwxi.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gjbtxdabk.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gnwxcujak.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/grffukmwk.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gtamcyepi.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gssbdcihw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/glmrwevxy.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gsgazsosp.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/grwqwlunn.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gpmaggabh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/ggljylvrd.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gkyivbjmt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gqfshzfzc.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gfrmeatvw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gdjnlqkwe.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gdqsaecec.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gldilkmie.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gegjhzkgn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gojxaxzcd.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gtmpxmlhz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gmgwcyble.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gpaldvdwp.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gixcbcbbn.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gtovgqgna.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/ghahnfiri.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gkpmsjwuk.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/ghukfgydv.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/ggitackyz.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gaajzdwst.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gdwxizauq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gcswptamc.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/glsxitjxj.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/givtgjqzm.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gkdthjxlv.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/goznnfyqg.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gaxbqtcny.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gdijxumgd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gxboymxbp.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gggcjdnld.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gxyezqoet.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/ghrkzzzoc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gyginoffl.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/glntmgjgm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gxgcpxydh.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gcoyiifjc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gsnesufld.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gbvxjnmzj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gkwqshntz.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gazqamoly.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbdjlodww.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gwrottcpf.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gtghnjhpz.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gzewvcjsq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/glqsikqwn.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gtlrabgoq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gtanftqdl.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gwproydzj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gqxnhgnvr.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gdyowrosz.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/glngvwjky.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gurpwrpwj.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gvisjcaqa.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/giadqluoz.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gvxvcyjof.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gthbzanps.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gfthnmsyk.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gatoadpyd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gojwbzzui.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gbkrmqqcg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/grtotazpp.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gcjbtasib.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gpwsrhkom.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/guiubvtyc.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gebqvnxig.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gsbnrhwjb.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gwhigglpa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gfypjikwl.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gaoauoiar.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gjxduwvrz.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gxcfqkhpe.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gxpzamxrq.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gmasyumvg.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gihpioeft.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gzgckwgtx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gancmgznk.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gibhqqbpj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gptqmmkcl.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gpfjojpvo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/ghfkgdrgv.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gbjbklvxa.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gsuhsihjg.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gqykmhier.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gqfuuzhfg.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/goieigwlt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gmhtyzypb.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/ggnsgronq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gahtpxksv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsxvdcuwr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gtcnezfxn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glqfviqvq.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gvbqueriq.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gyxfdxtac.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gfihzuivl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gftnmhsjw.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gxkawhelz.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gglonjwpq.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gvadtasfv.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gzmywmxjd.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/ghnsupgmi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gulaplzcl.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gvkljgivh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/geskizqrf.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/ggcadodbh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gwsukrska.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gqhlciqow.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gyajxykmp.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gabzmzxjd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gkrkkrarc.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gvdrjaxaa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gyqheaxsf.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gkwfnnpks.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gqmlrksps.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gqnapqprb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/grwxglphl.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gdkrucdul.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gawopwfsg.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gemarnjum.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gxwclcrrd.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gqzusiugl.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gtupcxjjt.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gcjytlzkt.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/ghkidernw.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gssoehpoi.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gyxfthgzq.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gywcpvgcu.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gmauaooog.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gqpcbbdkp.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gsodqhwsr.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gamtzbpha.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gxoqbsqxk.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gkvbkfkwe.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gvnwwmwke.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gjhrghqjb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gcgfeqnxt.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gqxftgadm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gykcrzaxp.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gcsldfezj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/ggebislcf.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gfqrxoqff.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/ggymdgiib.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gqtktrheu.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gapprgauu.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gzjukmxaj.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gggywdtiq.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gwnvcddpk.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gtocstgii.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gderrmnui.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gnxewyqzr.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gdmeqmrde.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gyfoqrhci.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gpcdwcgei.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/govppxdxm.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gsqaysrtc.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gbedjdhxa.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gmpuezecy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gshpyyuwj.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gsvqruofa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gjysnsoeh.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gvyyzubfa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gxhgycjty.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gelqzuwxz.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gcitivchl.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/geosgbuao.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gdkbfigyo.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gvftxyzgy.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gzgqwfhhq.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/ghrxlijlc.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gygggwttn.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gyaezseja.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gvifgwgvo.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ghikgvetj.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gpmuceiry.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gpabvlrch.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/ghrqxyvqn.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ghexmjtrh.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gycbcbvkh.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/geoemiqmi.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/guutujiyd.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/grkuaxgco.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gzwiiscnz.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gtkhnisuw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gyenxvqwe.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/ggwazysgw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gtvlvslvd.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/guxotjliu.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gucoxwugh.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gfnmavqwz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjhmauxmo.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/guklqjmvf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gkjduhryu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/grjoilspd.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwcbhvnyj.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gohxyqwqx.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gqdstlonh.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gczaxsdsq.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gdysnklle.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gixbjalvd.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/glsnlodov.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/grwmzswva.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gwpzklqvb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gqbhxamsq.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gekofibbe.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gukxsfoxp.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/govvbzlqp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gomvojxqi.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gwbpsbbjo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gmirhtiro.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gcophzkqa.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gvaomhwyl.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gvrzanxgs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gmdcechxx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gykpwzkje.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gzjhcvdip.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkwfbqlkf.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gandsopnf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gyovwhikj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/grzxjekjz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gqeccipbj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gkoldkvyj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gzfmmvzwy.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gfagwskxt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gdjufjyyf.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gnzlnkjwh.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gktnoeaxw.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/ggorexipt.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gfvjnwztn.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gqarcnejw.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gkimdpxcx.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gpxmumilr.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gmkqtqqjq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gpvfnrqtr.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gdzbiimlf.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gqacwdiip.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gciwenguc.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gxqfnvtny.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gtmtipdfa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/ggocagcpy.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gigvdcyev.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gznuokvje.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gjnudphkg.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gnavbkqzl.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gdojmfbuu.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gsrgkhbmx.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gnhcdjfqo.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gsilkzcuj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gbypeuges.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gkacscxih.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gfkqdosrb.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gwzsukcnq.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gfnoozizo.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gsywxqpeu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/guajcsoqq.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/ghiowqepn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gxssilqvs.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gsblxhjjj.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gqktckbsc.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gcnfzixel.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gctnmxocr.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/grbxbmtuv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gjduyjsme.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/geokvsfcu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gsthvbfpm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gccmttkzl.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gjjifygbm.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gzhntjgrm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gxqgvxtpf.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gdcpnkblp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gbiaxbabr.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gtuurrsue.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gjojmzknr.sHtML


<!-- 参考信息 -->