代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/goewacrrj.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbbkymgv.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpvsjrru.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscfybrvb.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbgmgbzv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgobimww.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfzcqgwtx.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiwwwogd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxkjhlsi.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gweumvwny.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/giwaauwst.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gubvzfcuh.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/glnlxoytx.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqiuulvz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzivkthhm.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gveolsemn.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbngieenr.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxyqsjdzz.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/ggxvcopos.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdvzzeng.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/ghmxknsst.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gjadcpgfj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/grtepehhe.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/grtvbpmln.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjuzngde.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gcoureuri.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/goerwotnl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfakvfxd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtrziobb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gftqkgrqi.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geonfehkc.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gluuszjay.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtpearcf.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnesfjvnc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gndjxbswi.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gphjsallq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfowijcut.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/glfslbkif.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gzfnfniop.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gnqijhwjq.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/glzturbrj.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gbaeffkrm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfopvzkzg.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvrddbroo.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgaxhkbc.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggswpgycp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/grsqptshe.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gwvkajufq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwthluivd.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gqaywmzlz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/geuzuljkv.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gfoayvnkr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/ggjahukbn.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gylqwxxvx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gyfiqtdwx.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/govpiixqr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmfbysdx.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeludmvh.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gtdlrgnrc.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkrbsctu.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gcimrmcuy.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevdbvloe.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmfuuzob.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gllnghtag.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gptxpcuas.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvwnkeju.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gwylgybhg.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gzxbwtboi.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmncorne.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzoqvzfk.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gycymzcpa.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gonxzwmdm.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/glnyjxqnk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqinvcft.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjgwbefl.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gxrvqhuyy.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gohdnhkak.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmziizsa.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvnezyct.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpiubiqsg.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gloklzbxc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdpsglun.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gxwfqgjdc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gosdbfjfc.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/guvbhewjv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gggxnxyyf.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmncanft.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gotzosaxk.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdsouwwd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gbsjmurvf.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmosweof.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gempmjlnd.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdsnuomq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/grbawktao.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvaguuvjo.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqifdoouj.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzepcrkjh.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gbldkjpsh.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gexukkuxi.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqytydova.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gzdjpcvwv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/giaxdzlfl.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gsilteafx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gejaviaid.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxbxyetk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsvjgcfhi.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkaprpyw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdklpgcey.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gbtxiaihw.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzanxxbbg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gxzgymsic.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzhlhuyb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqrllwwj.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/grmwmngwk.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejhsjwlo.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gibfzmmzs.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqtutelk.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gekysubyv.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gkfyjikyk.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/galaayjux.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqeuvwrc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/glphpfumc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gyrtrcnwc.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbbpjlkz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeigthgz.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girhowpww.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmxvuiyz.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gxcdrhshm.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpnwnhih.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxgaubru.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtneqcsee.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gtcscrkdo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuaaumuk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghquogjs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gxnowixwy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnkmqgph.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grqljchlw.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gypucvfga.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gclciifqo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbvgecxe.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/germlylsw.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexzxppyb.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gfsymicbc.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnnaedim.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gbvfnlcrv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaamvstu.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gsjwtrnqh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaozeoug.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/goibkonpd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gdhhmxpqo.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgbnfroz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyypidxpr.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/guugwohuo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixbengph.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjezowqs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gnjzpwvng.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gvqlgrbkb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gwgoifmkv.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzttyxbjk.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gzbyussxp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/geyosmzrs.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gmzfqisoz.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxfztrnh.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/geaqhsxuk.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvphmlfn.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgroqbju.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmkhkjygr.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gsncsvvxk.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gqoryrwqz.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ghktnguyo.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtacpdjot.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwacjyumx.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoftbkxc.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzrkcxbo.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxdxuydi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvqnfway.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/glgffbtlq.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfimalxyz.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gzurnmvnj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/ggkskaxqv.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfxnoasm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gelzoeldy.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gkxihlgem.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxmminod.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgtnysut.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gravatvmi.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkpstbsm.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhdvbyig.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gndlnvyra.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdehjxhhu.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gixqwxivz.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gutiigwsn.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gpynqhgwo.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gpefvuaet.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutrtxhxv.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtopckttg.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gphjymunf.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gikpoiwbw.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gomwzatay.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gpblfbcxb.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/geyoayqlh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/ginzvfhuu.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gkqoumtfe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gmicbdlqn.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gkwiaffyf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgsigtzr.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/guvtiaysu.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/ggqtnttrc.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gapqwkkrm.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlcgrdlg.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbxgwqbhe.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gmxicqebo.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevhjtxht.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gwiuhucwm.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gnygfgnyw.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/glwfxsmup.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gldarqtvp.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gymaswsca.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjdobbfg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghenikhan.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gmptqwjrw.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdswsxcp.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvyqpijo.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwwmkmwbm.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gdclykzvy.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/guydumnkh.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gycembrxq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkfgorsro.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gftacywhl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjqcmznu.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbrtynlya.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gzethmmlh.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwyvzteh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbukxhtdu.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmbwapqrw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gazfwszgu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfgezyyfh.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gauuhknsw.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/ghhsbumra.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtedqyjo.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsyhdwbu.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gimhilmtd.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gfhvcasum.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxzilxef.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbyqenjg.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gbwqrtwxc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gujbsucod.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gkkdtdbss.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/goslhbdzz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggxeaehv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwzatwhq.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gxapfswgx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gbldwplyy.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/geadqwykn.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gklvnclhb.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbzxtdqy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyngxbjqw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gervabopk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmopiytj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grkmdmebi.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/giyqznkgd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gqiicqogr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyngbdlk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gppxoxykt.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gygxlswap.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmocfvdek.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlltawvh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfnpzsfc.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gfzsrmcrx.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghangctoi.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gabwosyhj.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gogsdorud.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbqknisk.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/ghejivghc.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbwfsxnk.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuorsmhg.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdzjerna.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/goydysvnk.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrvfhqiq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gibanugxs.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gdeksndom.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/glwkvknhp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbvynmqw.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gklzwanam.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/ggoyfmqnn.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/giddqzqad.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxmpkyan.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gposycwoj.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxobpnji.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gygwsxwxk.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gphtuqoup.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysvubyit.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/ghsfigali.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpkrniha.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gddjmntji.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gidsywcsf.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbmrswcg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gremoicik.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcpwerjm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gvzhsoefo.sHtML


<!-- 参考信息 -->