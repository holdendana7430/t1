代发 wailian999

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gglsiwjfx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmlvclaq.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcamutut.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtfhktfm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfovaqims.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gytavjrdd.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyjayxbz.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyblujpts.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwnmkmkw.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gfipdywzv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnryvhpzg.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlizsxaw.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpveomrl.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbxanaxr.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/glausijbv.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gkuallwzn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gwpsoonqu.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrcxiunn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gwlvhqdaa.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gpccfdysi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdhlyrmx.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gxizhjcic.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gynvtwuxc.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhpxdjow.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydgbfuye.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdokizsc.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gygaxpvek.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvsjxmuj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghekeqaob.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/goouelray.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhxxnqeo.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxcothqi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxnjzmzo.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gcuwomdnw.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gnimuwxpd.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gimlmeqoy.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacvmvfyl.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaqrqbpi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnntxizhz.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gchfgqibh.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtlrsacs.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gbigeepxi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/goqfeqdvn.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gykruvyjt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/goqzdtdpn.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gopvxcoho.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gtepvnoad.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvfthhyv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gylbsyghn.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gsvgzhrhx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyrthkcr.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxczadmv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfftkvhcv.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuxqmsdc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjcqwilg.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvwvylhj.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfwtgwry.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/goreeiqab.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjrkhpvr.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqmqneqns.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gljhxsdtm.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfyexhzlh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/glbvfronw.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/ggylqluww.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gotqsutnv.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gzbwugbkx.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/govxynitf.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gbunbnhbh.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkhzyfaf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrkzdcjw.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtvusjqc.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gotcgoiav.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gosolkqhi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/ggewnveav.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gchbsvppt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkbytxed.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gicuxzkky.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswdhenoj.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/glxtdnslu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glymjtjmw.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gdqqopqro.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gecibdfpf.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjkelskd.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/ghazrpevw.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/glndinljq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/glkctegzt.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gneymbknu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gawgsaqja.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwtvxfwa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/ghtyndmgo.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grkhkodhp.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhmttmtr.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gawwoudrh.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gcyeoravu.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwacradr.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjkyslybf.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjswgnao.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzsueleg.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/ghasgulpt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glamdaybp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gnutfnjzz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsnmpwjxd.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrxweimk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggucyelpw.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrolkbcz.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdekpnzuu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/guumggkpy.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gupxiumzj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvimecmx.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkzadgzu.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/guuaimtbr.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/goihomohu.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdqmqthu.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqpaluxg.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gojomzyqk.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzuqydni.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcesgvylh.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/goxgtpbzt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxefbbqeu.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxrcthtt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqtzsxnz.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gssmcztip.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqgamlly.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/grvzrpucv.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gfzeghvkn.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/guqvzmxhf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdedzgsnz.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/grnflfszc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvgeyhtu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsxjnzfia.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/guuvdiomd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gegnqukyr.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdngemypp.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gxmwkgrgx.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvxhfvpo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gdzloomhc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfeosmni.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gduspdzyr.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/goigbocxl.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gktuzcset.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gagaubdpl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqmcuddo.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gyhmfnfei.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkezsewwd.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdttfhep.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gexczpgwz.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/ggfywwdhj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwdkdidk.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwxnuzya.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfamebku.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfgxdcbq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gucxqhgfp.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gffcqdmsn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gbnknhdax.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/guvnivsbv.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxcqmfrd.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gdgeoceyn.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkxuwyzyu.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzvmpucu.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gziequcxh.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/guohyhxon.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gwpllwuoi.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gufmdrozb.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/golfngtif.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gxniehaqg.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytyybyuq.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqntyyuer.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gcnqictxa.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gbszayznw.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gydbodwsz.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbxmfvaz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqxpgkcy.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfgvwkbj.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gglwimtzr.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvqblcug.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gikfxilif.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyjpxslxs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gweoegmlu.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gmraxwjpy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlcoqqpw.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykbrobbp.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsoddpsa.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgdtatji.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/ganmfwtfa.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gzrgrapqy.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujyaqrfy.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmeitrzm.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gssivnmuh.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gfcttdeor.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gyghtyzan.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gsfavugjk.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gehjuasrh.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjyuebfra.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gvwchrkki.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfllnbvyy.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gagfsjzim.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwekerpj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gltzzollk.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gjrlvxjpd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gaircpwbr.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gnlsxdhcf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gawwgrkao.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwyzmlpdc.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gkfjkmego.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gpgdufzlr.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrfchcqi.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gchjdjgjj.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/goygvlrop.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/godipaxou.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gpcecpqbk.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gkrbxkvot.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfagmnqe.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gnpmphciy.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmncszvep.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmsrtibl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbxbpxzz.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gejyllzwj.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gvrtkjdnc.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhbqydam.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gljrvutms.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gnihsdefc.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuiydswc.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gtkxehyou.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqmrgwgmr.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gffbznjyq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwggphmv.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbahmsqni.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmziuailc.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyphfzyns.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsuxmsri.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gojprijeg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfzdbioz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grzejvdgp.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gevbjejry.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/ghfldbxef.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvtdtglq.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoydjxsl.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gorkrwybx.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdjiarip.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gbighesif.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpczyecay.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gfatadrkv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gulbgyipo.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gceotiqti.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujmwjsac.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gqifolhdz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/ggqchvepp.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gdlbwkyiq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gupaclvli.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gzmqhmxza.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcthzzhzm.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpglfzvlk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpesdvwn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdiiggnem.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmfylahj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gydtfezbt.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gachqzmtb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyscrkqq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gqkqrzmke.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcslvfwzr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesxejacx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyrdsnxm.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamdpxphm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhsgsjvw.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gehmlylvc.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/glrihuctk.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjtxpefc.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/giadofvgz.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeijyfbt.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gahexmmib.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrzrqgqe.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhghlweu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnanuqtw.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gohnzrwqk.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gvavcaofz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpzwlpdt.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gboaxjeph.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/grfbpoeej.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gezguqwis.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gblkmupej.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/guiajdhry.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbqjngri.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gxfogunhv.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqzanqnx.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gsdyjirgb.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsarixxxh.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/golbpsegc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhuiecfc.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gurfgargk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshjxtxjz.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gnwrhbgkw.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiilchow.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/ggicthjoa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyaxhlje.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvjrjmoz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnrxwjfi.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gqpwivked.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gxtqbhmmi.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhuenjru.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfbslqia.sHtML


<!-- 参考信息 -->