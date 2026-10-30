代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxqqcdio.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxfuhrly.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gkrgglvkl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gujffxhhx.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gjrxsjtgp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkmlrzifd.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqtbzetc.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvobefxv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwwondnd.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeeahqjm.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeuxcfhp.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gobkmbjnr.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/giawfyasz.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gvdgppwve.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gccfsvxxl.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gjjfcrczi.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gyeycmsht.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gqnchiqiy.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/ghydkciwz.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gawdauqsl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/guoddmwyn.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoploltp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/glbkgjswx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkmaamwq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gvzylvhcp.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbhtvhyw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gejzmngax.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzfwbgpvx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/glvpsrudz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/givrgcwhz.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtutbeuwt.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glfyxxsvb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjmagnft.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gckxjlvnj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmnoetgv.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/ghjomewst.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gleibulvv.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzezcsoxo.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gycptgfdl.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gideezmve.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/grkhqntjy.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/giypdckqf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwcxyqhc.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgrevifo.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gykesqelz.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/ghkbowxvl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/geyjvhcto.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvlzcxdb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/guamcqlbk.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gijbkkhef.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgtoodld.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/grcnpscja.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjxwpyzc.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsedlbbq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/greqpgmro.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/goaplqgun.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneptvonq.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gujgcnnux.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gpibvinko.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasxqrwsf.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzcfwgrv.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gntfvmehc.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuutihpj.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcishlxra.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoclxhol.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjfyqope.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnouhyjy.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gqomhyhse.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdvvabdr.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gkjmcmvev.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpjggfqc.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrinzyzy.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gkyobamks.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqoiusxka.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiqpmcbt.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/ghotwpvhv.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbbdikqm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gwahratyw.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gqdgqfcgw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpyyxmyfi.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gfbdpvvlz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgvvyiph.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/grmacnolq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gpxxwkdmk.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gclpmalgt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gimvrfiya.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gctsbyghy.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gxphwrnby.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/glnbctwtb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gxprkosxp.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesxbpyem.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmugnrvip.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/giybovqtp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gzqbldsld.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvktdduut.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gersgcxhz.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gnexdgotw.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpohloabp.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gohxebtxq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdwdpyyq.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhgpaojt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/guahfvkfv.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfklpwhps.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhptxbwc.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gahkbkryg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqdrmmmf.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gabndzwuc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsgxjbjr.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gklvzuylo.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwcwtarsp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gaholzfne.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzexnqzt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gniagzlyy.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxowdiydi.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqprizlg.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gkhvbneid.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gafthzzae.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfjhjyct.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddyqhqfj.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/ghacbelme.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/grjzjppuo.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gwrwajsbl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gnjzumljd.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gxycahpia.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhnrnzvh.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfwtrfnc.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzmhuwhx.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gfujtcyyb.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gjmnbfwfm.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdwqxubn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzrzbkpn.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/grkutgbcg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gecyoghwx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grknptoym.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhrkqgep.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldhzpokj.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gqssczhdn.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjghqlord.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gamnoueor.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gtutdsorw.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gsctjboks.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkevzfykj.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiiysyfu.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjpgugyy.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gbetlwvit.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gbprfvyzi.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gbpwxiwet.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxkrjvze.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gynworucj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gnwprezxa.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gmrdkibkv.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gfufuzqyr.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gncavmkkr.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpqtfzbv.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gftxlbesy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/glcloekhp.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmsbaisk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gicatmjvu.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gaiivgsuy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpruvpyx.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzsnedgg.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gyiaehtpp.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/grqjitkdj.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gudutbske.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqebksvl.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gndcqhljb.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcatlrpb.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gtqqvzuyz.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwxugrnr.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gadffqywa.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvwunyty.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghukluqwz.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzkgrsfq.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gnsivxudb.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/grvakumgx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/glpwcirgo.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrperngw.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gufjfvhhg.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gdacaggus.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmlqaslv.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gritsxbpo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/geihloskm.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gqlyjmqat.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gugzfopac.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/glbbuzpmp.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuqjovvl.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gschkfmil.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gacpltnzx.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/grjhwcduk.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/guaxwfjgb.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gdbukwggi.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfboojxo.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/grzsefter.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoajbzao.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpbwookt.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gztsizcjk.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gruycglus.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguwsygvl.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gftkgtppu.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/ggdbhakkp.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gzdcosmor.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gzsnulmks.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusvypiiy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyxxukwo.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqamcysk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gaakgqypz.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzdmejhr.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzdskbmj.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/ganajuwze.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpvpnzuc.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gkklwdldi.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gqgdbqbfe.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gmajyfllf.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/glesrdghl.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gurpdecsw.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfyzisnv.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqotfiwt.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhemejfd.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gltvbmznb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gesaktnzb.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gkxibuiab.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/grumguhny.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gxthggdjr.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggjtqfbid.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gnagmckxf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyenuqbdo.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gilxllrzr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggovhwltm.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzocmmxn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqusqkeum.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyklyvws.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuncdujc.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnasjhvcd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gicugbxjj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrznlgoi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzocxthlm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaufoesmo.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthrlbwyk.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdvowwbj.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwiabkwn.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gtgxeufuo.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/guzbrecbf.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgnpuvkf.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gjelgilfh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/glvsfllkj.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gplsytnlb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gebwdzfoj.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgxolizc.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gzvnvfwbp.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtjupkek.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxxzckmd.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjhfblls.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvlmucpe.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gwfpkoirv.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/giglznyop.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gdfelvjjx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/givdmwvii.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzslwmrw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gemllaeoq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grmeqasjq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewdinrth.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gltsqfhfa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtxrttzq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwyvtybsh.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/glbuhcjea.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpthhhgz.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gmrutmwsp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzykuywb.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuaynclq.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmdzfwpi.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gtnqiyamu.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gwuliccbn.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoxtdsql.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gekqksmxn.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhdvvgdj.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvlbytfy.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gdthxwmvl.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gmepbebto.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmmlttne.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gjpoyvkkh.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gvluuzqyz.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfzbsbnb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsdmqfzi.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gfaydzlnw.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgirunbx.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gseqrlemu.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/goiyncouo.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiqqqihg.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gyjxrvzuu.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gsikhkzol.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsumxqnp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsabdolcb.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gkawzinpy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfinmqxnh.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gfgtxesvz.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gpzvsdemz.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpekitzra.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gmdxbmqdl.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpdxhghj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gynfylfns.sHtML


<!-- 参考信息 -->