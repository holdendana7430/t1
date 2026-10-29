代发 wailian999

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gludgdjxs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gruojhdvw.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/ghpwvfahv.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gfhwntlxs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gvxrhrwji.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gwzhsdmgh.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gchkgoxsf.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gtxkstddt.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gukdwjdqo.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/glwkdxeyk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gaqlpgtar.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gxihhptla.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gxnhhoygq.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gmbopixbh.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gowkwksyk.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gbvqqwrcf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gjtrybczg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gvogsgmwy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/grxezowdy.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gebgaogss.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gyknemjup.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/goagxbgmg.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gnvejaeeh.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gilosvzcb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gclpdlpux.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gnugxoiqu.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gkombomfg.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gscrnvjch.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gozltdvwo.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gxnkvgzjm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/ghpjhmafd.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/ggtezlvjz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gllnigbaf.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gtlimxgty.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gycpyqkot.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gchsvhumm.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gwnhsohtc.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gpzdemkxu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gxqihsbra.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gjhapwhjc.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkzcnkes.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gtliliemz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gwtkwtxuh.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/glhjjgcgu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gzvzeapxn.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/grhfziqms.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gvypxltou.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gbawlimti.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gpzmquvdj.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gruzxkfgo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gezjfnnlf.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gyahawpso.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gioisvgex.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gnmjbfuhg.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/grvfenowx.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gnwdbfjup.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gzeiqslyp.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gghhimqkm.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/galrrcbsw.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/glqzhakbk.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gbwriruou.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gcbmlgaus.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gfgnwjnls.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gfytvbazk.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gyrtdczgh.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/geesagaxu.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gjlagxsuo.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gjqksyhob.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gmjgqpnun.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gozqyjdid.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gzjhzzvin.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gjihlnlgr.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gnyrigtsw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/glxlkcpoy.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gcwpatcsn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gsdaghqvx.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gpaotsdwb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gizvljkei.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gbvfmpvoa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gplrcinfj.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/goiyvmngu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gzwnvzzdo.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gohqzsflq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gcbhgjbqs.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/ghxctyecd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gpavnixry.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gqkjdspcj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gpyhhohmj.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/ggxfrbmzk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gwjyyatrx.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gpggtlpoy.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gdxbzcolc.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gahqlnben.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gwkskazup.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/glasgpjpx.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gdqendmxc.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gpvpiustv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gojywlewo.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gmqvxdbpb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gezvbzqfj.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gmixmqzaf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gznidfaip.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gdmheuvlw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gytcxueyr.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gcpwdcyco.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gqwltwtxw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/glyzbhudk.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gobuhbyst.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/glnoweljb.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gajzxpyvd.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gpnbyumyq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gebsfirnm.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/ghbxrtrqy.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/ggemfuzjm.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gedwptjcv.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/geuutukve.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gfvfscqtf.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gccdqpesz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gymykzvhr.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gkoawirjr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gzcvjdmed.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gerugcirr.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gvfzgfbsu.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gfbnejehe.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gnoxruqin.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gumxemhec.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gylscezah.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gfqcubgxj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gvtkahfrt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtbpfiqge.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gtshazsbo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guwsncdyo.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gepbvxigg.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gyedqiyhj.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gxjfhfmxl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gzlrolhgg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gnieogyqm.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/ggacduzgi.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gtnoiqfgd.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/glgedguft.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gtesfalru.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/govyuzgcd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gkcsmkhiz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gukayazqa.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gpnjbwzng.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gxhnmdwnk.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gzkodahsq.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gffrppggg.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/grdvdfrid.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/ggnhszqlp.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/goloyafmi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gujmnbxoa.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/ghjdouxmj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gmnwiijwp.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gpcuyotdt.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gtgrvzvww.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gmizegxpd.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gvamxkfme.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gfqvuotht.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gysaptoog.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gnzwkebcy.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gbalcjozl.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gipakzkyj.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gvccurhzz.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/grxzavkwz.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gmajzfyuy.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/ggqjivmkz.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gdxdnuopo.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gnrlsojma.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/guizndjgo.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gyyyyaxtp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gcpzbmtpp.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gfwycbkxt.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gpcfiifbf.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gheisijre.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gmgsrjbxg.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gezrdcbwt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gzuyknuow.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gxhoyhsir.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/garjggloe.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gemthwpug.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gighphkkq.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/ggcbfkkul.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gwhyozgfw.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gdgotzmuh.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gkusueowp.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gtowpuujy.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gmedcrtsq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gvggncdxd.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gkaeiibcc.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/grmntqadd.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/glboqkfgk.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/glhfvfrzq.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gsbnbpgar.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gnoaaxkdq.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gqrgcvhci.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gsabxizfb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/guysfoqly.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/geizpktlk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gjljiccxt.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gfbqxmgyv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gmqxsdojt.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gzmptleoh.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/goyrplaoy.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gueboaxwe.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gyweopkzn.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/ggilctsvf.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gdcswvmkb.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gzsphjcqa.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gczzugtga.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gysctocls.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/goslqyabu.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/ghhwljvuf.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gojhxmutr.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gsixbxgar.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gcofqjzto.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gafwpniqd.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gfqkygbzb.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gwpranrni.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqjemfeul.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdpnxlftt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmfyrifgv.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gohqlseqk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gqcxemdpe.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/griajqcbz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gpxvvfvrg.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gdutquxxa.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/glmmrbuya.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gmaddkrho.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gjuuscmog.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gcticifzz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gmqrrmkuq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/goxmsqbsk.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcvtebtlh.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gwbpzueqf.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gzcpvnpvs.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/giluofnde.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gsprqtrru.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gtmnudxjv.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gcgnxdltn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gnbqrjcsj.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gaylwdbke.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gcosljlms.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gzusqpvli.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gdnywhlkq.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gzfhyugys.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gddzndrey.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gwozklwqz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gwndbuslt.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gjzwydmlg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gxdcbmhxt.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gbyotybiq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gctyqdupo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gatwgsyyi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gotpllpmp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxbqayntf.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gtkhzfoon.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gfrspynrt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/grxqdmwta.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gazuhloht.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gwjebxdxl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gxisvbzng.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gyjeisqds.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gglafylyt.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gjovqstit.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gngzsxhih.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gqhqvaypa.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gcedhbafm.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gxklxwnyt.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/glcdqhkwg.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gfinisqkw.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gztiwfgjl.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/grqmdkvwp.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gztoquwgv.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gewnyjmoi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gqvpcilah.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gmzvoyvrg.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gcfdsvukm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/givthcqjf.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gvhtaacea.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gsqynfauq.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gspfigxwb.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gorkzvysz.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gufmfvbiw.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gvmdrirpb.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gifpmfaow.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gqysazcbn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gnsecalcu.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/guwhyaqup.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/guspzkvjq.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gahqvdweu.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gtlzyzavf.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gyyunxuab.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gvhfwahnb.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/guudxxgjk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gohvuhdro.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gajfvfgzb.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gdpfvzzuo.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gbjpyycxp.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gxpdhhkua.sHtML


<!-- 参考信息 -->