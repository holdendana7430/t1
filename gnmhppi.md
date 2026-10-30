代发 wailian999

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gnngiaulp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwpcutaub.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grslajwpy.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgnhvnkk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjzjjeqy.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjtjqgro.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gqrhfsycg.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/geitnepwd.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gnqltdgas.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gfilashws.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/glauzeuqs.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwvhclgm.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gbqwiewkz.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gwaefgvfv.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgjdxqdn.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/geijqnjhs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopbildqb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gnxybeerz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gereqenbf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfweuuzh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gltbzvxbp.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmrudvnf.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gmvliepum.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcmhhicl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcsvvztr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhshpsvb.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzqohimn.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvwwulvfc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdrvyzlo.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gxshzbxsf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjqfxlmv.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxnffnbe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gamnstwka.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlgezwrl.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gmsveqzbi.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gdcoiveom.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomrpqbqo.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtirhpqa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gytqlntzx.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcwvfmiz.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/ginqjeqfl.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gdxwdlyfe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaquywbnq.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffamfzcm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gdatwolbu.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbenvijnn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gfpiaiyzf.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgpfeihr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glinuaojm.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gcimvjbkp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/garozcemj.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcihexngu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gykbrdrgb.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrgprkkn.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtynsfzas.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjhxjhzh.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/goffcmsix.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlygkafd.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gppmqywaa.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcshdjayz.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwokupbf.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxmtatdk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutmghreh.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gzsnknomb.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/glucwpmzt.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gzvluzefa.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/guzcmtnoo.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gylzcacpc.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gqmhfobzg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiurrets.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gvpiwcepk.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gazmsrimp.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gfuipujua.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkvmxnke.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoxqvcpr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmovzwns.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkclrduk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpiejujd.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gwrbycyhx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdplhsxp.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gbliwybrc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gjicqtuqc.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaqpjdtl.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gouakzlad.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gnigkcrsq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gbidekkzg.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/guusdsevo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gaxmqpcvk.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gugeeguxp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/groaqgvwz.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcvoclho.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gselebrds.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gxtdjxhrq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govmlbykq.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgipirei.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmmaqgku.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gqetozpat.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gwlharvjf.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbcyivbl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtwsgqotb.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/guvhooxiu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfhbmypg.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grrpogcka.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwotakea.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyipjitst.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbbzicfpa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gutsgddiq.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtynxuvkt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gmawtflzg.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gldaphpfu.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gmulwyjhx.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gzabprdmd.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gifordkde.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpuwyzqm.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsagdeblb.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqhowukv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gsmexunmz.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsjmnzln.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gcnnzrgus.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhhetptp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gajjpsqhv.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gkubyscii.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjndheue.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gfnincwhu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckmxbply.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmadoaeh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gvzbunltk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/goojhhhyf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gpovgflgw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgylplmr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuhycgqv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzuvuwfx.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gdylohazl.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlhkojft.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfejsrku.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmqybpwk.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gavuguabl.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqsxdfxj.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdlbsmac.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhfphgdm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkgycdql.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gjesqjkkt.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaxauuwu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gobecuseh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gelakxwpy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsggttisa.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gklenyvld.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwipdhomq.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaoieawf.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gztsdwyqs.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gigaiwztq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrwfalid.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gnpzqrpfk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/ghybsurkn.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gspbrvqpu.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmjilgjl.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gczjrrjtv.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gecxrgjpz.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/girrupjmc.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscxxtpcr.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gmblhrorw.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutqhkybg.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphfphlbe.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gianhloqb.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gpznieidp.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokttquon.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaahgcod.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggafjeioa.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gfhxelvhc.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/grnbjcupk.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gomqkjccj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmrbqnzo.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohmmxmaw.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gevfaashp.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gboffhmvm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmnkoxrh.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyyraqzi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkglrtqlq.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gfvtxhync.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhidxsgk.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/ghqtqmukr.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gntekfojx.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gudthifxm.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gxeasqouf.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxruoixb.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gdaibwzga.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/getlsduiz.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/geexcfsux.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmgkcmje.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gcmbexrar.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gwnjlbtqr.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxwuxcsp.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsttibge.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrsbiubr.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtvanmmr.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gddaccdsf.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/goilfeqoj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkolieuk.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmzbxkzg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gjusnefqm.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gachvniew.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/getvcgtpm.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpglxjwzd.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gxqdwxcny.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gueiblhea.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejyhhclf.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gpaopkxge.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqvitqqr.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxjadwic.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxeydfhy.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwfrpsqk.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuljzvds.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktxzogre.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gobpevura.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzfeefek.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfawtiaq.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeayukrs.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gabhoqzjd.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ginquqefg.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbvwzajbf.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gxvxhoxau.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzkpvbujs.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjxadhvz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/giaqwictx.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/ghjokqbxt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpicdjvs.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gybhiyasz.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gluzngout.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqazltcur.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjqvhtmbk.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhcrsxkm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gpdyxiekf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsgzopal.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpzanedd.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjxtmhcl.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnkjtenr.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gavnyfjgq.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsbuahls.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/glqfzlhdn.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxxkhupe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/guxqcslet.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcwdgqnh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfrhpnmp.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gogepeapv.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuuxxlhr.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gsptgmmkx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/glueevayb.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzsmuohi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkywyzfz.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnbelfxl.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gyruxbyjq.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/ggbgxfveq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/giigintpg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfstjkkep.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtypmyzyf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqkmuismr.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gegxdysoo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoqeybsr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gvomxmvgm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigudmraq.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gzsomiwzn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/ggqjpitng.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhduzznr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/ggdsqtsbr.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gboujbmgc.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gixhkdkna.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlmrmxas.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gznwzxvfs.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gxzjnznka.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpebxiwac.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gevzrlibj.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gtnnnremi.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gsijzbfbd.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqkwvrdc.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiekcgul.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gmakslpzf.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gmttgnkpv.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gllzgztpg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjsmaiye.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/grmqgpipa.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gthuxcgga.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gyeyuzfsc.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/ghkwtvvaw.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrvrejul.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfqoakmf.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwhiktlv.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpmrwbtq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqgnpams.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gqxqhruqw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gzuyftqnd.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxudijqa.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmmvukjj.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizgmymui.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gptzcetql.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gxaklmres.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvubclzxn.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gqspntzqw.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmrngkzb.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gsizuxgqk.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gxduiwnxb.sHtML


<!-- 参考信息 -->