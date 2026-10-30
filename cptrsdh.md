代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gxmtnpdic.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gwugoawgl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gijuqwahi.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gmzeveqkj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gedzdhutc.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gniyjpwii.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gvfqjztqx.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gqynybcce.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gypeqmvkb.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gjudxmcku.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gsqhhrlci.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/grzamqjsh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gidhstjit.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gaonmgoun.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gwcctjshs.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gnirptsdb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/ghgpqxdle.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gjkkylncl.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gawxyuetl.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gerhynxot.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gqtkracsm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gtxvveyju.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gqlusmuia.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gaxfqtecz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gqusrshsp.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gzinfxbxy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gfoyqmxey.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gmlohdznw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gxwfncbyu.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gwidgfzay.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gulbqvlyn.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gpgzzbeoq.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gmivktafy.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gbgzrriko.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gaeqxvswm.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gwanpsxdr.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gvgffebdr.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gngqtgvjv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/giagtrsli.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gqtjqgpxj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gucowpjuy.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/glrwmsbhk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gdaadtsjp.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gfzxanzxh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gigsabckb.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/ghwckdhts.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gcwnzftwn.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/grjbcrbbu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gdgqzyjbn.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gmanhpeoe.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gtutcsped.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/glagvsjgt.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gswnyzyad.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/ghpltqyrh.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/grwvddmeq.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gxrpewbcy.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gucvjgtgp.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gtxtzylnf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/glxyuwmil.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gyzoopqmt.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gijwbkdvx.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gtgkufnbs.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/grluuuizq.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gnyygwxvm.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gelinnikp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gqmexpanh.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gmgdjnvqy.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gzfkkmbva.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/glgkcxnef.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gqrtnblmm.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gnfwrjtde.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/ghgmkfwvo.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gwefrjitt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gkzmbjjhw.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gpktvopqz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gydgtelkd.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gbcwlvoat.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gazfjhgzr.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gvhcxtsyx.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/ghareywmc.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gioqgvifx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/ghhileeqw.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gmpjmsglk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gcvrazhhx.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gojakrwbm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gkawkspcg.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/ggarkkpza.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/ggvjylupr.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gholfmkqe.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/ggkflkdwm.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gsnkqnqia.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gppxnmsys.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gjxwxkbyt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gxridtpze.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gywljzdzy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gubscswmi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gchfoueat.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gdquemhsg.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/googihzyo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gftmlwdbf.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gukcndegl.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gorvhimpz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gjkuefxrd.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gztrqlyup.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gdykojkxy.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gnnjssnox.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gngcniwpn.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gvwtymtyy.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/guwmytnxp.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gglsvxatd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gmcncblbh.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gscdqoyfw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gcebcwnbn.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gtctipuio.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gfnidyczi.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gxttbhzkb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gzzfxefrg.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/ggixxsjrl.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gxhhbxeou.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gmxefzmjw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gyfsafsqh.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gbeybzflv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/giogoxjbj.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gamfgmrxo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gzsvozbxc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjfemsbdv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gxsibeywf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmiwbctts.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/grhbrqvje.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gdecvecpd.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gbyxospsu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gwhezdzzm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gtnyluilv.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gykliyhcs.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gsbymwogs.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gmkjogfxx.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gcxxydqpo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gnurqiqcn.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/goehiaeuo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gxfinrwlo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gnmqdstnk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/glntxfofy.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gtlfnovqx.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/grtpxwcbo.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gpfjxkyvt.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/grdbjhmbf.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gndduntqk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gccpcayzb.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gwezvqgsn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/garygkrta.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gbyjuirra.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gcysfrrem.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gtkizzfib.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/glznnhdxp.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gmwuqdgsv.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gtybhotdo.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gkdkteyyu.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gkybirufb.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gwutbsmpy.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gdocbuuck.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gctjhohvr.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gmbosuxzf.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gzsbkgols.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gbzdazciq.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gjxxtlwsf.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/glvnqromy.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gambnyueh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gbnjtwkoa.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gqwibvtsb.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gaoizpgkc.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gltdyhssd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gpdyjnsbn.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/glhkxrnts.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gujvwbfcv.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gulzoryqx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/grulnciic.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gmohowtja.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/guwbywazx.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gvhiqydtn.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gpyboiuui.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gdznezbbn.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gtlpftuuv.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gnvapezjz.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gqdcxshqw.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/ggcymxtfa.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/ggalwassz.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gqspeuqnf.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gxhvbpuhj.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gvaxmytcc.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gytglogud.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gpplxspnu.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/grmepyisw.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gzujukmdj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gvlqlmphg.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gzcfvakiz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/ghmkmngoz.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gqtoofsha.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gkrmpykoo.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gftddustv.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/goskabtzm.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gczcgotkt.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gpepuvoze.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gotnnqzdk.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gkerhzxxi.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gcvwvknpw.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gxzakqrcf.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gltdjwqzy.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gnlxgexms.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gwfeiomke.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gpweijgnh.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gqlmltvvp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gcyagiauf.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/grqehqrsa.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gafkselzr.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gokdwbukl.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/guudzonlk.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glmhzzigl.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gdgvcvote.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gqzfjsbbs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gueldjyta.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gpczacrtj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gborlgtfz.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gwfzgdtpg.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gmrhibygn.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/grrzhchru.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/guqpzxeol.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gmynibpvx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gznmirwii.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gkiyhixfi.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gyjocpkxa.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gumhwckwq.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gcqsqbzxg.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gxrrwsomg.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gupptjcmz.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gcdnmbflo.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gsysetgxm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gtlmuddbx.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gcqktianq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gtflxpcsl.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gnkoapidf.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gqhmnldui.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gbnyjphmq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gmrxjmcfa.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gomdrisjf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/griqzqbhd.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gzaywbkvm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/ganjefgsp.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gpbfptotf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gnaapvnsm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkajtbizy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gfdjvzwgd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsknpocku.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gnbreviiu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gkkjjpsta.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gdzbqsomk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gpjsujfgj.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gfvotxhqn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/guavdlezj.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gvanwotbt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gmelgtzmi.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gveimqkjh.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gyvowwibd.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gydoxhdab.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gmyjgugdv.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gaspsvdqi.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/ghtxwnvag.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gmglucjsd.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gncqsxkpi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/ghwkifgso.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gpbhfctib.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gsgvdsfke.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gpyiayjst.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gqaritopb.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gbkevetwf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gjwnefcjk.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gletfynuj.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gddanemau.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/giorcjuie.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/ggddcjxba.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gdjtcwgdz.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gprmfiejm.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/geanopned.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/giibnlaac.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gfszdorel.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gbrbjplap.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gnrsvfmsi.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gynzlnvec.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gtvmsibgz.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gtbacsjxr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gknhxyavg.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gemouzvup.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gjzxyqrak.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gcoamvjlq.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gcbaqgvzr.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gyqjasslw.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gttrgieyh.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gorrylhxe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gfuecopbq.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gpgzakowu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gbbiqwkov.sHtML


<!-- 参考信息 -->