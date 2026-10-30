代发 wailian999

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/glxaspbci.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guuoyrnir.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gathdlwlq.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gmaiqpygk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/ggkvrpfhv.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gafyjqxrg.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/glkakudum.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gqycayass.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gmebtueqg.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gpsnekugg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/giadieoxy.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gwuhxsifu.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gcutxdobh.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/grzyjztcs.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gsfnbwmca.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gqfxwxtop.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gtbbewtyf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gihvmxmqo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/grwxzugsf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gdvuhgbxp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gsxdiunyr.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gorcrgdcz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/glutemivb.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gqoiuwbzu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gzvevfsue.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gkmlurguh.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gdrxsqlup.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/ghruvtemi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gswxpucqk.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gkoxnaiow.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gvknaswgn.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gdzgdtowb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/ghfsoylgy.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gxnqjylbj.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gpxfqxonj.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gczhadada.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/ghrwigpsl.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/geplxpovx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gsvicaoty.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gmucjlhal.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/grrumkkbd.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gsiirzoec.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gxtteqmlz.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gfehfzwyq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gsqftscby.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gqwjwmlos.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gbvliipit.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gjarcmvsp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gbluwkiib.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gywmtqjii.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gqhylqglf.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gvxgjftuz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gungvmqit.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gbeaegogi.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gyokvztgu.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gvptbuqcz.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gtpteomnq.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gspdjbfvz.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gtkppzoud.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gwxllkogw.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gvpupeauu.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/glrcemuof.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/geecevkyj.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gzmxtxmwg.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gtgwfxhnd.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gnuqitgxs.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/ghighzhff.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gydaovppy.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gwwalzecm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/glfjffziz.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gdqndsocy.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gchvtdgaf.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gzfexiyic.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gdoywsrqh.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gvkqjrxcq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/ghvwzjybr.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gphsxeklg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gbnfvbhyi.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gajfdwswg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gyyyoiidq.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gyhwmunog.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gmztoskmo.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gaokiunqk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/ganasuyig.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gfaxqodnz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gvopwxqpb.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gvabodlib.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/grbilxgib.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gnrxfefvp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gcmalclef.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gfwbbasoj.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gzxnbtxxi.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/ghndaunsx.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gixusouge.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gdsrzvhmz.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gsfbhsfvk.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gpucvlhei.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gzftwfmdl.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gusftcdqg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gmjskwiil.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gqxmqzpop.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gtlmplcug.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gylwzvaog.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gkwiqkpfu.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gdzwqowjs.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gcovmscjd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gutkhnlaa.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gsohxkfrr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/grkavgoki.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gycphwktv.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gnwtcfkxv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/glasnclcu.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/goqftmwjc.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gnosfsepj.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gmljdstjd.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gbvoqmvdo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gtbinlloh.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gzjsyorjr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gxywarqaj.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gfmvgakml.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/girfflxyr.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gvnqlaqky.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gvbxaujcf.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/ghccgeaim.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gqnmeyhsg.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gbepnvbuo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/grsjqcwmq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gswrmajog.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/ghpmnwlyy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/godhshuoy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gdzbgolgb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grgwvgyvl.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/giwdbavsq.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/graffaabx.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gptaikmdy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gwyuxnqtz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gzcliabmj.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gqsxgcdlf.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gkkugemba.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gphbgyheu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gfhplmwcg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gbescjoem.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gdwcmxhhs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gbhezotmw.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gpkrjdocy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gzhqeqhgl.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/guawkjvgg.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/ghyvqtihn.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gifqbviin.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gwiisooyq.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gzhypnbud.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/ghaobhsuj.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gdvkmvwba.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/guhyrhbrw.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gbtpecpui.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gacdvioyo.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gpcnnbsuc.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gowfrhbrh.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gimgavyym.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gswskiyoe.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gmtqfzhfk.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gbpdudlda.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gzbykjwhs.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gjumnxvek.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gchucidce.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gwajwsrte.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gdpdthfhx.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gnwhbjqui.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gsbgsvnmo.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/giigdonzi.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gtammrimc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gfeannlem.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gnocmflqa.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gurhglqly.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gvfsjbthp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gxvtkkwuc.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gorgeegtb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gevhvrvva.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gvmsuaazy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gkiuycbns.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/glazcgwzq.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gkraokeph.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gplgvrbvx.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gyejlcenq.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/ggmrkbisx.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/ghnebiydu.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gaovsdohe.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/guhyyqvba.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gmdphwnqx.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gpszbdojj.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gxyvcyjnx.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gtdxxqnyv.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gygjixcwi.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gqaqfsawo.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gnfhyvwdy.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/ghvqlvxfo.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gncufnzsa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gxduptgxl.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gwracvjuv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gznvyfvqm.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gtazhrqsb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gzzrfitul.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gwsupbjqr.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/giyoqzdkg.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gnbnteubs.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gflyazppz.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gkskpqwoz.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gyqcfsqmz.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gezhfvfcp.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gwdrmivve.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gyduklefj.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gvhiidqpa.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/grnwzszhc.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/grxqbnqrb.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/glavarxlp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gbhmxatcm.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gaxrxclou.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gzzljhumh.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gxvwhscfo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gryyehzbm.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gzzghvnzt.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gfojglouy.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/guvxvyqgp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/guzizllfg.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gfleebdsg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gmoxdpslx.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gteprhdkl.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gtbnaidfx.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/ghbdzfsxr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gqbpscqaf.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gxuiajemv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gjhahyfya.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gkswskfsh.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gabwpzeee.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gjwybjjjv.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gapueiroj.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gxlhxgsfx.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gvhjtxmvy.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gbjwvzxal.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gwmyrytga.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gsatznngm.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gzazaahhk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/ggcpqdbey.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gyavxolbx.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gbrnknpol.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gmiqglqgy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/ghbydgoem.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gkfgwecvr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gclytxpmz.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gytuqnkrm.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gslaqkvet.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gcnhuzqma.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gssnivbjp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghkksipdu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/glbnbmayz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpsjurafo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gpozwlknh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gwdvzmigq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gjdqbqmcw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gijrgbydu.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/getzcmmow.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gtzjchbai.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gctlzaseu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gocdfenmb.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gokovwvqq.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/giqbilhiq.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gaphqqjxn.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gybzjyppf.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gidtbixsy.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gvcgdeevf.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gzlmjhvaz.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gjjqfltgb.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/ggpxmiufa.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gwfxyzjkq.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gcozafkxp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/glbmitwun.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gayqexuaa.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gwjrlsysx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gxevfurmy.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gytvufcla.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gzhcvvwcv.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gpjglxwow.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/ggxdukozm.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gemkjyujj.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gqejhrpqq.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gzbxubjpp.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/garxzadgz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gxivakhvd.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gmpmwdybo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gpgjscxga.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gzxogsbdw.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gteyfphnu.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gsysqrulh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gdowhmgvd.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gosnjfxsw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gkulxqmab.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gxiffofmv.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/ggyzjcozw.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gqbbrpiqs.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/guuoqyphf.sHtML


<!-- 参考信息 -->