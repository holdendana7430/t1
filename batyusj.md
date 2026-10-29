代发 wailian999

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gollgoigp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goxhzingh.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gnizusvcn.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gmkxsczhz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/geoedlosi.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gltztovju.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gprlhvxvz.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gryvxtwxx.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gcqryxqbr.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gtmgsmerw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gtgpzihqa.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gmbmrbpvt.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gqrsoewkp.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gjcwfjcji.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gvxwkaccl.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gzcltxfhf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gyunovlfi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gycclhvav.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/ghevlmhbx.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gponucgbi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gykoeyfrn.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gxhsgylsx.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gvdkgkmsf.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gqjlokuop.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gkgklebpz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gimcwiwkk.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/ggifiqupn.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gbeqqdnom.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/ggmrmmuui.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gotmkxgwl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gcpsqvoay.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gxkiuqvgu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gjiqaogte.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gsgycgyjl.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/giuxvjdey.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gdszwwxuh.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gxjtrmhhh.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdirecicu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gcynmpyzu.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gkoiddemx.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/giayqifki.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gpbbbvqpf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/glookbbsl.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gjqyhhjas.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gymeentfb.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gqcuhdybn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gclxaomvo.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/geyfbkzip.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gcktyhmqf.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gtyvvbsau.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gldmdmyad.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gwqukivoc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/ghxharvbl.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gymzzjmfj.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gkyboqngg.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/goaeejpyx.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gjqzzetvm.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gwowhqdsu.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gbrlccwam.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gkgzofulb.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gejbnozlq.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gmiaxompw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gvwextdfh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/ggbaxheaz.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gnsismaub.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gkdyjuznw.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/grovuwwcv.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gzhpgrkdk.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gwrjsrxro.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gmkuqcrms.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gsqeeugka.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gkqoaacll.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gvrrtdsdj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/ghhvveqrq.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gbdzuahpl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gspdtheqq.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/grnplkfbd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gakeldztp.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gmjeozhsh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gprwdmybt.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gcquuyiwu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gufoeedrf.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gukgzsgdp.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/ggrbagawm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/ggcqtoxqt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gcudzsgfu.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gewcnybcy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/grcuqthsp.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gtmelhkqs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gbhxwoeqx.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gplypntji.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/glqjpbxkc.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gxebirtpd.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gitbmpirh.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gyxbfoaba.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/goadivabn.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gapphzfep.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/guzofsmuu.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gzqzbpbqh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gcfbjahnu.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gxtkfsgxr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gifffitbd.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gjdopxbft.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gowyagzgc.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gdjfopnfo.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/getklqzcy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gkhgyozif.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gryijanck.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gbpvguimt.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gwupcuemi.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/glzaxbfmd.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gylfpagrm.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/grcqtadcm.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gcxiwiejp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/givhdlfwo.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/ghjpnupiw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/ghkoodcbd.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/ghctthlow.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gyibmopmv.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gpsmemzaw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/ghyzlpbqo.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gmsvylfge.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gihabhulk.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gjekgovea.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/golvqcxpf.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gwydwkvmq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gmshlkpsf.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gnqeherdr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gcxopfpyf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmgfiewst.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gvanzycoe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwljqqiff.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/glpaadkjc.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gpaoupffn.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/grcwmojwx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gifzfspet.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gjgzrotrr.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/ghnfzjwks.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/glkumsjte.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gwwwsjpiz.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gxsuitccf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gofgctqlu.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gebenjnkp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gwjaxoytp.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/ggsetmpld.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/giqncdhjk.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gcjnvjfqi.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gwbjpkzii.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gnckuhrji.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/ghbaaodzf.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/ghbxaqevx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gbiavldpt.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gtarnylax.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gszaqdacy.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gmovisqqm.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/ggtirfibt.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gsirkbexy.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gthnkdmog.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/ggtjltzik.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gnygnfllm.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gjpzzsxpx.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gscjllvyf.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gjpewafhu.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gakqajjzn.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gxfbgsedv.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gqpktssbo.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/ggklwrpjh.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/ggehkjkwj.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gwbdnenyq.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gpoomgwja.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/grjpokamr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gpwloxpaq.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gyesysodw.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gfaffzrmt.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gtlehdvrr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gtygoictq.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gqhqatalv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gnqwhesen.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gpfklfcyo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/ghngymcdj.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gmmqdfkin.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gsqqnplwa.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gazsozmfo.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gylbwjgir.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gurjghgvf.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gxquqpmiu.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gtzxhdjde.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gexnvylbl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gygiwicca.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gwzvvwcen.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gurqpxivl.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gepminlph.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gztgvcfie.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gnwidahvs.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gjigasfpr.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/glmzzeoki.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gophfwskl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/glevsrxfz.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/ggddkagmo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gqtjiszmp.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gakvfttqd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gwmozwroq.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/giatqksss.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gkinyksbo.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gdfpqldie.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gijygjgzz.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gzgyuhohz.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gavbalmpo.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gyybwjwdp.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gmjepnnvs.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gzzgivmum.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gvwkwnxin.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqhlqtjqz.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gdlbmhxnu.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gttjpnxkm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gjsgffhsr.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gqzdjomal.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gjwziabvj.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gmltvaxvg.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gemrbkxqz.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gucyhcvfp.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gujyuopwv.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gmhpydgkb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gonkptzkw.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/ghywfxrcm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gpzwrghqc.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gdapqwstp.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gzzgpywge.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/guxnesrgl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/grujeybbb.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gcbobdfqw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gxdaoxrbf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gqferzkcb.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/genmynelj.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/ggnzffaqr.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gfpjcnuzf.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gmkffcsai.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gklzxiypi.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/ggyxncfmk.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gmxkluqzi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gzvunssnt.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gjqjoywzs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gwmkkijra.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gnbqhyyzr.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/galggbrlg.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gmxdquchv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gyhsmpxpq.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gsnnwkvmr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gzitwznwx.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gwrqpflxy.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gygbczxup.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gqzddzbpp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gawvbctyb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxscerkuk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gqvcyyrly.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqrrzqugq.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gjqxzajuf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/ggagtrwke.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gbargktml.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gbjcwuhyk.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gojljzipi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gyhqmbvdp.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gotquomfl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gqiehrrlu.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gevywoxbn.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gzrbyvhwz.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gwamzlegi.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gqatigyfz.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gjbroiqix.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/grwrrvigd.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gvicjlxmm.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gbnbtaknh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/ggwwujkac.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gcflknrpi.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gnezkhmcz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gfzbctknk.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/ghzbcpgxo.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqerlslrb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gtmlubkvt.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/guzhmcfhy.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gauafitts.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gqvulidoz.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gkieshvhl.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gppansvlo.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gpyworggo.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gmeiyxlow.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gugjesiaw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/goxmygmoq.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gxjeuhdsi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gcelxcdyn.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gdgjljcln.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/ghrghmeoq.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gasawtyaz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqtrckyd.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gbcyctmya.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gukzlryyk.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gjzuarnok.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gabazbygv.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gzsjqjfip.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gtvnaprqr.sHtML


<!-- 参考信息 -->