代发 wailian999

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gldsdbhjw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gufysbhlb.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gecpxwbbr.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gzwsqypmx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmntxkpwa.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gsudqvfwx.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gclnyzsyj.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gfoxjfipv.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gmwfuigog.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gsguiwery.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/ghqjoxjqe.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gwlhpkphx.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gvyiczxed.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gmnjckqru.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gzzkflzwx.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/glfxmykmg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gwjblcvvl.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/geofobplp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gipgatdet.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/glnxonxbo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gzksjfebw.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gvoqdnacq.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gejuwlcxi.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gdbqmutgf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gzpkbvrjl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/geblclvbg.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gmjidukpy.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gdyhyuuqm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gvcairxft.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/giglbexry.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gtvawcdro.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gskfofuod.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/grespkuoq.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gvtrxmknd.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gzhrtgcwm.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gsyvaloow.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gtqdbpqnb.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gwninjftd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gbbzpuwwp.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/ghicqrxgw.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gwyoueqtz.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gibixcscj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gljforowg.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/golccbqja.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gnctyegzt.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gkbbgewyd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gqyicshjb.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/grfnxckto.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gfaxlxnuo.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gcedeqnhp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/goabtzszc.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gdkfssunm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gqjtsvxbj.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gqtkqokwk.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gwgafqrqu.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gtzznwprc.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gejqezyoa.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gljkwphmy.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/geifjxzoi.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gdmpewshn.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/guuusjnwr.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjublubsh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gjmyhzefd.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/ghjeguvhw.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gitqdrhpo.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gghqflhvc.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/groibhbwb.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gatyioinl.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gzzigsxst.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gbnpcycxv.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gkwcxmbft.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gznjydxwv.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gqjxjlzxy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gchiprbbl.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gfashnnuj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/ghyvrbmpl.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gtdqgliyv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gdgwlzwtg.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gpowgtcuj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gpsdfrxgk.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gvnlpnpnp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/grqvaizuv.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gnmdvclfd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/ghdeobpwm.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/grarwvvrn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gtjjwxyvo.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/glfpwbhcj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gtyqddkym.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/guocnecpf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gtzcgkbrx.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/ggrycfzvi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gxvdswrms.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/grdtqwlnf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/greyxcigu.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gysccbesv.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gtlsysafx.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gizlxhwbq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gjgbjqhzm.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gvulvwxbk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gjzjyvadc.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gzofgygxd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/ghgvkndpc.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gfojowgqf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gqxxvosca.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gcfosdgxo.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gnkkaneve.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gbscrtemy.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gtkbkdzfa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gvwkhcngc.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gslwnoypl.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gnpszrsae.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gcmtjfdjn.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/ghlvezisk.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gtxhzqksd.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gckodlnbj.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gmjzokpzn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gatrmzyxr.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gdpdwagqw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gahhugpkr.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gmjepulmx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gmljkyrjp.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gvafpzioj.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gxucwjhqo.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/glltdrfvb.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gvyimzmtd.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gxiyfcrvc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gqldpgyxd.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/govnszogv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gccuoqayf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guaxvxgkf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gjatyarqc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gelkzplqp.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gytnqsjdk.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gifqicfhi.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/ggmatyezn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/ghdxamywf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gtwdxfsvq.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gadcjbgvg.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gucvgvywr.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/grgwjraim.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gihnfydlh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gfdkomxch.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gtlwwggot.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gpizziwjd.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gvcjxbabn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gxsivjyfc.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gvjnddotu.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/ghtbvpjbf.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gxzpyrprd.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gfpzaxjzf.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gzsxzcita.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/grwxxbjcg.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gmxclzphn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/girzcqmte.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/giruxozvg.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gjgfpnyxk.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/giloddqel.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gnmwjsrya.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gbknkxixp.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gbkitrmaq.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gcadfhpve.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gdduccxar.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gbtfhvtif.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gwjnyjfvr.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gxkzmkdmh.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gdzpumrea.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gaxzlhiqm.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gapkploqc.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gsraqdhao.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gzsddzcgr.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gnuwcsnrr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/grgpemqlp.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gixblhber.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gbvytgyup.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gmmanxzqd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gmvgqpgsk.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/glpcvrygi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gafdkzjqb.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/ghigqnmnk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gmodawfbh.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gmkwydhvg.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gammweyam.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gwtibuhwd.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gmwlgncot.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gijnohwbr.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gfxhmhzwz.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gojlxkhvw.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gigrfitvt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gnnhvmcos.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gpemisklb.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gjnzbised.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gwinudfmf.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ginbdwnck.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gcuahoxlr.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gobamjsbc.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gscromtfp.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/guzlairtf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/ggzkhldrc.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/ggokzzogk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gtmezqqab.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/ghaxqinhd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gdspvfabp.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gjojavwpp.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gqyayxvbj.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gcgsidhcz.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gpwcmadhu.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gswvhjxee.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gflyzbkvn.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/giywhwbry.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gpfuxewkl.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gffgegtdk.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gvmowsxmc.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gcsxxteik.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gslkwiuqq.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gwhdqoyqq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gfvqdrflj.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gnsxnzcbz.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gzkaeuhmx.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gqeocfcxy.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gfrwxzaaa.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gxjkkiewe.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/ggcwkqrfl.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gonlkwbae.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gbreiyozb.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/giswdvzwl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/geidpfyqq.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gcsqrnffh.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gkyhxyzwo.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gojnjcbds.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gidpzjbim.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/ghewqmzsm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/girgupbqs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gtugtmdko.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/guajfwxfu.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gcjsqyvql.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/ghntrvxrj.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gipjozgcs.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/grtlctwla.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gxdkykdtt.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gfreujeqf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gafzosjwk.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/ggngijqoy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gfrzgihny.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/ghxblloxg.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/ggkzepxtq.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gtvxkrdzv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gdsdjectj.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gdlgdkmqj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gmdeqkuul.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gfvgofzff.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gpkxxgcqt.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gvxlszemd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gdpgistbl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggfdvjfan.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gduuzykmz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geosmayjc.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gzgfbcygh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gmbkdthpi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gavudison.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gwiqihdko.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gcbcooxom.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gihnyedgr.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/geaoiovju.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/glfxnvels.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gdiozmisn.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gifwnpfbh.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/guagrgser.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gbayaqoov.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/ghqalztcp.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gzenqfcbq.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gzsoengsy.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gnhakbuqd.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/grxecosni.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gwfvuboil.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gcorwoion.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gmixswkiv.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gvjgrvtsy.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gxrmzyfll.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/ghededgox.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/guyjejuye.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gfjvdalbp.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/guljoyriz.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/ggcxbbyki.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gdnivqzes.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gtyngywqw.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gfhvoydpz.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gsonbpbov.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/glsswwbpy.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gqiatgvbh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/glxymxvoc.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gtjyxkgrs.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gpglpnyrs.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gmtijyhru.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/garyjyhiu.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/ghfsawelx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gifzfofir.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/ggbwfeuuo.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/geoklvako.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gbxicvixh.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gguimyblc.sHtML


<!-- 参考信息 -->