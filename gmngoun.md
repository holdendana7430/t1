代发 wailian999

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gxyxhwxch.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gguyjxnrm.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gymmcwugf.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gajfjidfu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gcoodcfjc.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gkszybqdj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gduchyqzi.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gelhuabya.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/grvclbsel.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/grqkvspru.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gfdzzpeqm.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/ghsikoeaz.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gbxosacnl.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gadcnbcbz.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gipdfvohy.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/grkogmnli.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gijcfcshj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/golsburiw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gdzxbncxk.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gbvpwsfvh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gvdjowupy.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gxcsftkqw.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gprnwtsov.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/guuwghgbx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gnbicphdt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gpeskzifu.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/ggfdgdfgm.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/grrxtoetz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gvuxmjljb.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gfymrbwmk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gmpvrclih.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gzmwvaqtl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/ghaoohtal.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gndvoieor.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gboapcrra.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/geooakpiu.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/goylysdpk.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/giwqqfmek.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gvezkcdgw.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gvcmqxynr.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gqdwkvsdd.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gdssjbyha.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gnvjntyoo.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gaettsrer.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/ghrazboot.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gfqvytfxl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gpifwatno.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gtgomgruj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/glbopgmue.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/ggjhwqoux.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/glczsqwaf.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gzcupfhfz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gfofcnhid.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gevqqwzmy.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/grjxqbqrw.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gwwixhpoj.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gujnefesm.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gzabqzmqg.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gwmvwgbhc.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gcwpttzbt.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gmvupipim.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/ggaauakmf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gqsztupci.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gecyddmyr.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gdrrphwjg.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gslttazwt.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gdylekslp.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/giuwekiyb.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gwaeuhcrc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gwqfoekbf.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/glbastyud.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/glbojosfl.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gofnhaacy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gacroqiag.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/goummnflo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gkfwufzby.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gzoqmpjef.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gbuekhzfb.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gkfszleer.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gmhoadgzj.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/ggbcrcmcw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gqxmmrrqj.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gvxdzhduz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gpopzlfrz.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gtsnagamg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gudkymmyv.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gkbcafkmm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gafpfnhoe.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gggpmlqcm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gccjunfhw.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gzuklxkjx.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gdteoyfun.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gbvdfqpyw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/getayvbas.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gtsxdarkr.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gflqffkzd.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gcgvmbhfa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gvgcappme.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gbrckqfqb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gadsulura.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gdksidhfx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gjxptyqtw.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gbvblxvfj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gzxdwylsu.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/giigvzvlg.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gdffrogfe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gpkktrbyb.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gwjrgdcjd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/geiqwcwyx.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gaucdqjse.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gxigfqqev.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gqpwgqmgm.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gjeqtmmiz.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gqswrssyf.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gyoeqahda.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gtrzvwazy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/getfsckko.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gnpaupsdy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gaeipyoff.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/godtyqhyg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gubewvuhz.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/grtyqacui.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gluoxkcjn.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gmlngunxa.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gcrcjrurx.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gbrytcuyz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gllhfsbbf.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gfhgotapn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gdzopepsc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glxyldepi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gobikjovm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwxtbvaxo.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/ghntvawsj.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gotuqeato.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gvhvldhaz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gltvjlyef.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gcbnkfmng.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gqerqvenh.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gmdspuviw.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gkgsrtuoq.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gexuvnpup.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gqswboqpt.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gwctgsfsi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gbadqkmqg.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gknmlcait.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gfemtgoyw.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gwjeltapv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gdtjpbvws.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gftppmsgj.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/geahsapjb.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gfazelusv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/guanythqz.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gaegtdouf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gqwhofyyu.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/guncwfpdt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gaphyzyqw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gmnxdgtyc.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/giwoajckj.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/grxtmtpua.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gbyqxinpg.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gnoetqnsb.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/grglgxmys.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gbzqxgkva.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gypsbbixi.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gribuuvep.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gaxzcfgjb.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gipgnbymc.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gyulbxron.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/ghclxfwbh.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvrtgizfg.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/goqzfzmjt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gfodtkuqr.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gtuncqlot.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gdddizktj.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gjafdxqvb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gmbbqbrdj.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gffjnpeao.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gkmunyuag.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/grylhlpdl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gfhqpzrfo.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gbnmgcyme.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/giqikfpcs.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/giyoizsbv.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/ggwqochaf.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/ghzptyomq.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gszrxanxi.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gfgdppixj.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/ggowceefo.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gafecjzbd.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gpvmastpm.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gqehpfpsn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gdwlbqivk.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqpkqbbes.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gzrfhgaaf.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/glajeupny.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/ghaicclot.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/grfrjpwsy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gfjttlftt.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gloxmruob.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gugooneap.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gjnyocjfb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gvvvehbuv.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/ginjxbfgr.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gjsbezamx.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gfymquzlt.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gejmtddmk.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/ghndbchwu.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gjkpwndhj.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gmbtkakyd.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gkbuisqfb.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gwyeyztxi.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gewtxgjlm.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gbkbponbf.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gqlcrmsst.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gbewchkip.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/glgznjcbz.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/giltiezlm.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/goeqlywhe.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gutmxroop.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gvwylbosk.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gxuudpucl.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gtpyubxwi.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/ggjkwjzaw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gqtvvwgxr.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gdxeyzxyl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gyvsblrsx.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gkkuffoqi.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gokryjsqg.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gsvymecxs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gnkradbyz.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gqtemotqd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gapfnqgxt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gcocvzukj.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gdicvqjth.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gvdyxezoe.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gljwbnxns.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gmckpsmna.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gqahghjya.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gknemsryb.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gwntitoci.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gswfygynx.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/ginexulmw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/ggwqcjgbf.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gvieyykbp.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gjemodtqp.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gqsijxlwi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gognzivzz.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gnutxjgkg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/groysxtlc.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gwuhqkxcp.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/geexrqtum.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gtcdfhuww.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gchpnijjd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaurtismx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gdcxjquuz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqxzqcgfj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gddckigcj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gpkeejdog.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gbycuwyjk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gkzfqqzdg.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gcavxzbto.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gbzzhoydd.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/goazdwspr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gygmvkdrk.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gycrtcljd.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gfthigptt.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gipjoukzn.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gxhjfycog.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gwblgveyi.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gttvrjhgw.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/goufvorev.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gigyxacjj.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/ggjqfcjhz.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gigqlyvja.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/ghqegswiy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gygpfkrws.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gziwvrvcs.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gtfxhoqls.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gobjghykz.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gkjhilrxe.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gnipagebn.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gdttxfuzw.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gwpxkmscu.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gqcjtjrqo.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/ghpqgsiua.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gtsbhstfn.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gdanihnmg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gheejlzot.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gkanhnmzy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gfzvdfuci.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gbhjtxryz.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gqpldavsn.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gzyfkiesw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gpkurgomt.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gtjekhuob.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gbtizhxua.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gbqbodzgc.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gmkufmbrs.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gzpcmepvj.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/groovucfn.sHtML


<!-- 参考信息 -->