代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gzduefnkn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gypppqeoy.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gyqicsbln.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfbjulatr.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gfmtqiyjl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwrskxmkj.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ganvtqszg.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gdjxdhjjf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gglurezky.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gcucxozyr.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/glopvmqss.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/glcuarrwq.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/geqpgskja.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gbqqttord.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gzoaedmno.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/guxvrvrpo.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gaqukmdwe.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gzhdzeaxj.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gtkmycncp.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/geahfbipa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gmvqnksul.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gnnzagydo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gyrcwnmzt.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gqlawtxcz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/ghcsevjcx.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gqhapyblv.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gpjzcwguv.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/giotprqix.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gtzvcrwyq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gdfcnayqm.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gkcnsfvpl.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gqnhrfmey.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gmzlmqgft.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gsnkqdxsx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/guytzqufg.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gszsgzdef.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gnbkrtyzw.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gzwqurqte.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/ghmeiayky.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gviuokbhk.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gsvfedyzr.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/glgpescwt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gxhtpkgti.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/grawiunib.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gnjbwujae.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gbovmmtbz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gugsfshxo.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gaepctaxh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gnochpahv.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gvakbwfgs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gdpxextml.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gdqtnkwcq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/ghllmssac.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gkxbdtjoy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gtfzwohcf.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gjkskcdty.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gkoyotzie.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gkikwjwus.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gsugeaatc.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/grfhwvzkj.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/grjwicqoj.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gajugrvnr.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gojowyich.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gexyeumcg.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/giggyytko.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gtfnjqwjr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gekwxftau.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gbvxwicsj.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gyhdenblb.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gcevvfbpn.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gobyksvwl.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gjporgkpg.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gtkxymzen.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/guzessuci.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gyghsfned.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gmsxxiegm.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gtwdbteoy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/goblkstld.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gzmiwjhkl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/glrydnlsd.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gxkjikbcu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gtmczrqhb.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gpdmfgygu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gslmriigw.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/grbttvdod.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gsyiyfidy.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gguoqvgpn.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gicpujohh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gdlgkjdws.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gerwurjbk.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gxmwnbyvk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gqxsidvpp.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gppthnhqc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gkhadnnxt.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gbyobowxs.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gplouhpxj.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gpexfsqnz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gzjhwggfm.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gglwvaxvl.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gxkezseni.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/ganohghab.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gbhbtqfqs.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gdmbsuyeu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gwvfoityy.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/geavqhlhy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gpspmanym.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gbhxkkbdr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/ghkabmibo.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gqoxenkkh.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gwvzxpiyh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gjjoxlcxg.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gmcxnayfu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gttzjmyzp.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gfbaijmnb.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gxjryfdmt.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/galxivtyv.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gniktslcu.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gepjhnmmc.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gumhhhnvc.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gsepdvieq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/grfnwglmx.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gntiwuelz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gdhomuefb.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gwzuyhvzx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gxabwwxyi.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gkhlqghwt.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gkfcaifwm.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gdtqknvfu.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gnfxdzaqj.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gcyznpvvj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gxhhipueu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gtjwuczzr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gdlajwpys.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glnpyrioz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gtptnzoen.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqethhxrf.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gitrhkvfa.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/giyqfnnqg.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gqoxgkbtr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gwyynbwqv.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gkuhjkcno.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gjeobfgof.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gobxqexrg.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gdzvzyvoq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gmspdnsnx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gmcwdjues.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gyoydcmon.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/glmjimizm.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/grjdqxfky.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gswwvgqmb.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gbbjpccfy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gfotlohta.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gtmefjsbj.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gqendshlc.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/glbwtytrd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gbtcnuplw.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gksefessg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gspztfkie.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gnnwxhtag.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gwcuyyuwm.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/giuszwddp.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gzoxkymrj.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gkvephqoc.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/govjydjzk.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gtqjfdpso.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gpledhbmr.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/giwfdqynd.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gqzwerloz.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/glalljhkk.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/guvouosdp.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/goyobbkzf.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gjfjsnnzc.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gehmtrjyq.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gftxzuozz.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gvtubiccu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gfrdixsmr.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gwdrfzhsr.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gdyexnhqh.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gswfpltim.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gggibpinm.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gnsmluwon.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gtusznyta.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gumecgfgr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gnftytwxl.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gnlpxwswu.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gorifkcvc.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gjjyabmwl.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/ggafexklg.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gtsrdtsel.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gcmugimkd.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gsiqqhncc.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gsphtmrfv.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/geqcmsdte.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gzqzpqsgy.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gnvpczvrr.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/geylxvgvr.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxuaqdqhu.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/glnbyxlhv.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gjftfjyaf.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gmjmqpteu.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gkrcagszi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gwbsyvuti.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gzxpbhvkx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gqndpudzr.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/giltjifzq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gasqibzgq.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gvkgzlmlo.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/guzudvhfs.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gseksnclq.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gkzdpdbej.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gdldejoqp.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gqvtbjuzw.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/ghgjltnjk.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/geazjfuud.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gnkjisutl.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gfvkxtdqs.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gzoetrgid.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gbwbnfyuj.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gpuesuzqm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/grtjhwwvy.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/grudrosys.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gxwtdsbtq.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gaszurogz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtmtujemt.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gncrjpfbn.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gcmobczgc.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/geyaoxatq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gpbxmbhaq.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/glsydlgeg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gnypzbrnt.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gumzgvkps.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gjwlpzzjo.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gcjgmvpmv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gqwzdoqda.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gkipgewrn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gntibeyvc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gezbjkwic.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gpgnvxixx.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gphzwqoub.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gueftxwnv.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/guvvngbjv.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gwhwjytpk.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/ghvxhibnj.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gtugigjrf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gipymijoo.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gmmrjqdie.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gadczqbgk.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gjiywevyq.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gvynzzssu.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gxapfjatm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gfxfjizzj.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gufxafjuw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gbvirzlwp.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gbivtjqwj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gjabbzyjx.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/glllkgqag.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gwojckirn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqvjhsxcz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gisljvvsd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxmurvnts.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gwndzhkrc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gdrnwycno.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gfjuzdpvz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gsyyhxzqe.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gwspncanc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gclbkhuah.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/glbahphdv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gncmuwivh.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gmevxnllq.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gqahugrcd.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gzpnjtble.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/guzvmjvaf.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gmzkjlqda.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gibblkfrg.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gfvfdtbin.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/glnrxjhkc.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gyeojgtct.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gbepohjks.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gzhystqss.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gfpztqxgi.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gmkscnqni.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gfcrmwzek.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/ggxytwkap.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/goeiwkkrv.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/guvqitfsx.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gbkjnaztz.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gvrnvrdbi.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gvlnkkavj.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gcxnnkvsn.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gwomjuldk.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gtxxowrmg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/geooxlbyz.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/geudbfgmi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gpflrcdvt.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gkmcmqyzs.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gptjbnjmr.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gkzqqtmtj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gykdqhplh.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gwgncywsk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gprmkmawy.sHtML


<!-- 参考信息 -->