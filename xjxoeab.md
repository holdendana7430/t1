代发 wailian999

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gkjmwcpcq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtdsibuyy.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxuumrykw.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/govtdyzyj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gzebtmxua.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gbeqkpasb.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gdajrzbla.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gmwgfntzp.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/goavdwlqc.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gvdhxsqfs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/ghvucylok.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gtvadcwms.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gqghvfneb.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gxdyvjgid.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gcxzdxrtg.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/grkpcjjer.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gcvvbfpfc.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/ganmdsonk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gnbrqrjhh.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gmddvvgrs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gpbuxaxau.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gzfghduie.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gwaoyigrg.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gmhipbink.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gjirjwmnc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gdtdguqyk.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gmwykpboo.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gfmyduzqh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/giconycxy.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gxvzktbkf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gpcxrxivg.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gfxdgdoim.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gewitakve.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gmamjqdni.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gagdpnpfe.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gssemuukh.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gvdgoounb.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gfxvzdpmu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gieoqmlmi.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gbodafgoi.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gwhksnqla.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gxqtbxfrs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gztpwutto.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gdrtvwmiw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gabndfrru.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gbuacoily.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/ghrkaaobx.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gvgcwbyaa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/girexdujy.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gwqbjnwvt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gouujpzct.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/ghgrfgzif.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gskwagguu.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/ggmjvbxbq.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gcrkbnmpe.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gvnywrobj.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/graaqajon.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gmqqyaawm.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gpasloinm.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gxebbaehh.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/grrtjeqdw.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gaqgmlioi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gxwuzhfns.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gtnejxmaz.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gyihcxaxc.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gpatqqqgv.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gdbgyzibc.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/grxyjdjtw.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gciocjiev.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gfoncrctb.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtvabumsh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gvhovlziu.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gzztxtbfm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gbkdrwafe.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/guphthovq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gwasrogyq.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gfhsvoyib.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gaxodjhlx.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/grwotcsyp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gdsurvdha.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/ggatvjdwn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gcpljkpdq.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/ggxxoukbq.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gapijitbe.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gnisiouvg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gbnrbwnxb.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/ghgeoddyu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gjnwdlfws.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gftxewxhy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gibvhvnpt.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gdoeqfnqq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gqjjjegnm.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gyvrcwjan.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gbniggarh.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/glkxsoetn.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gukxemoum.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gkfjbdmwt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/ghfugsxqn.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/ghgzigksv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gauokgwzb.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/ggdbkczvm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gspydtlzz.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/giuhbbfbo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gskyfzkkx.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gttsbcgwh.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gvkailwux.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gemwbeugv.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/goubdudei.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gbzbvbvcs.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gliymkzbr.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gpkdcrlqr.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gykwjnozp.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/geszxigvr.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gaedxawrf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gyhxgedrg.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gbbneqcij.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/guplbtuvj.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gktyvzzul.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gpvofazbq.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gzuzilnxk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gncujvloa.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gmzxpbhge.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/ggdliuufp.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gbyakocsp.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gjrpagpuv.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/glsltumfk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/govezjlrf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gsoxwlwzx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gsxxiagon.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwplawowq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gfdoeafvy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gamfxhlmb.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gfwvwlrep.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/geylggjtw.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gdkiobdvk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gwcsfhyen.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gygjpfzqa.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gcjbguisb.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/ghegzcxga.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gacqcryhn.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/ghmmeufuk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gxaxxmqiq.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gejnfjvpm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gavlnmkmp.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/ghzhivsxs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gbksucdhs.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gmqwreaby.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/grawwbrqb.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gjzfquqdg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gnbmdbcsu.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gomxqnwzy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/grfgbzvjn.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gyxzrvndx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gvhlxahfk.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gqaphqhvr.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gcfijiuhe.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gmqassfii.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gtqhuvknm.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gtocjcvlk.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gooyvveqp.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gqlluaavj.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gpjtblltm.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gtgbeasdr.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gbdcvyhxb.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gcmlwsurc.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/garcbsuav.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/grquperlc.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/ggzleamyi.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/glcclhzeb.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gvqfcqczn.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/ghoypfzoa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/geklexoyx.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gzganeqxt.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/ggqdmkvpc.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gbihyesos.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gacfbfodp.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gxapdpkxw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/ggdaunqzs.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gtibuydwv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gvbwesoiq.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gzwsspapi.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gcxiranun.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gjxonyqgg.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gxbmmsjmn.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/guzhjgsiv.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/grdcgnplz.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gingyzsgc.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gglwecjxu.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gzwjjsind.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gvqjixqgu.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gmiscwigo.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gbyhxcvle.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gxvzuynuc.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gppcgswka.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gmurqzwgn.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gshqkohkn.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gmpnclejy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/ghdxfcrsc.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gacdnbmgb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gplanokmp.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gnfbfzwyy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gqhfnwehn.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gayhydrer.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gsqgfnvda.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gonnsqlad.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/geteuauki.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gucmsjlnv.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gwotpowkh.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/grsrusidk.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gnqmwskvj.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gcuojnhlg.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gwpjrimzo.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/geyhszrqk.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gmyssntij.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/goccbjnqu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gsypsjjdb.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/glfxkgwpu.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gdbzegrrb.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/grtdtdmvl.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gfdducmzm.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gkpxxkyro.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gdgdjwnyy.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gcvqgfwvn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gtliinpyw.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/ggcdjwsuy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gmwmzuvqv.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gjtnxxzwl.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gglywtfqj.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gwgemvmme.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/ghmqlvmsb.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gehyweqyn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gsuafofyg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gmoxvodfj.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gesfigqpw.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gllefdppe.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gvbhlsgtp.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gwftgvrgb.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/glaperqij.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gapwuymum.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gpmbpzuol.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gsnffrcoh.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gjynglice.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/ggjprdsiz.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/ghskcdhqj.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gfwpgzgei.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gayizyvww.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gaibuxkgm.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gflpexkqc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gnyhxmnjz.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/ghatpdwtp.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gjouzesgp.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gktvjkmry.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gcgjspdyb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzyzkanhq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxansehwo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmvuvzlhf.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/guuqyshrf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gjbhkcqfd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/ghvblpkdb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/grzjolsdz.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gypkximsn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gymouewru.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gcoedebmy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gwsrpseul.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gobfmbktn.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gqasklwvp.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gwqiextkf.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gfmlkkaqd.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gaffwuglt.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gncxruwyj.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gktweyarm.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gleuvtthc.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gyknvcskz.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gjbuyedqg.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gtgklomne.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gtnwlxtnp.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gqzrapwbw.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gdbfgjiwx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gxohkodtf.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/ggtybxeeg.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gfhcdgqpl.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gjkmbfyrb.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/glwktnwym.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gilcxnqxl.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/giccgkzga.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gczbprggq.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gettsvdyu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gqqfosksm.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gouirgbbp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/goavvtbom.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/giaczbuns.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gabvkfzqu.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gaibogbtr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/guuhzokag.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gkuvysjvl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gyzawnauz.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gpcwvgvbz.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gbthmjroq.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gjhjitmbr.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gzqrnabiy.sHtML


<!-- 参考信息 -->