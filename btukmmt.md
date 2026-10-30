代发 wailian999

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gmqdrlagx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbqcnyevi.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ggjxgymdp.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gtflksgij.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/ggnvqaqob.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/glcbidcdi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gsnwnjigy.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gpnrkgcmh.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/grwqzultl.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gjfpjqgxl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gyrqzjrmf.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gfskcnqmd.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gezrfwcrv.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gbfmjqziz.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gkvxmbnwp.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gtxmfbwpy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/glawdoqts.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gwgotvxzx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gomrdgemp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gkdsjpjxq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gwkdkgitc.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gtzqieeyn.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gpzhoticr.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/grzxfdkss.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/giunzappx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/grwaiebme.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gvhwjedxr.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/grgfgblsn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gizxdnmbv.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gxscbjqdf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gpcpshjyi.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gpqxfpbtr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gqhtkikfm.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gaiwxpicg.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gbdaopesg.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gwtxpltvq.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gncxpzcat.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/ghpdngxgc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gvnxzrbuz.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gnuajmlmp.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gjxufxsjm.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gucnuowjf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gjqzlssck.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gdrzruanr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gdrjwewov.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gptfyllwc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/ggtopmpau.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/ggrbgebli.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gzmdrizzf.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gqxbkramd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gpihnntjy.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gymzzoxst.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gljeagour.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gncdvywzj.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/glavvnhgw.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gxdavgeek.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gelzurzcr.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gtfyaveit.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gevjcsxhn.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gjfhpsjac.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gppgoajur.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gvwgpsvtq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gbpnfhuwm.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gbqxzvoxk.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gecmgibsj.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gyckpkxcn.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/glsfagcgv.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gksnnmmfm.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gfuvbkfxv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwqdatsxw.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gpefhdujh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gguaugbwv.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gbbjkzbsc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gcpojpknj.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gtnpqfayn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gngqegetj.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gersydvhj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gamydgnuf.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gqebfvjoe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gxvrysvxi.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gotfvfdsu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gdrzcxjoh.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gvscbjtbp.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gfsjrquxu.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gxycwgpij.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gyomqcaja.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gidsqbxel.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gsxaqihrd.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/giojczthb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gxtnzqouj.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/glmkdblwh.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/glwzlsvux.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gvasnaqzo.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gmknuagss.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gdvdjmjfd.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gubsrswnf.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gknmtljux.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gebakbbrz.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gsyfgpgeu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gdesdllib.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gkebleacy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gnnunaquh.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gnbpudyqv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gditjkrsu.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gvtoxoaxy.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gbsoswvhc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gphuowqbd.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gcxibtiqm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gtmkyiptq.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gqwlhxkfk.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gdfeivuki.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gxtoylspd.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gustphwka.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/ghzfqszwv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gelatvnjj.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gnibttmmj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gfiyqlrii.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gawcuyenr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gtizqdarq.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/guydssjhv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gajlwncbn.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/grngdapyb.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gxswecvpn.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gfzpqvzfv.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gqggadgwa.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gelpwjhqo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gckfnyadl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gnulgdfcg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/greqxbyuk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsglwnqkk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/ggsnishgw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghjjfmlfv.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gmmbtlydo.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gerpvbwcq.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gntkdzoxk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gzvbdttcw.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/getrechiw.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gxfoauweu.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gicmlathc.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gbapjgcpf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gmwssnmrz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gtapmhpnz.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gsyxfjdtl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gggmcgnev.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/ghxfqxkxe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/ghbvxuidh.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/grigqpgfl.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gumunkrve.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gvjyvrokz.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gxntdjqvz.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gworcbljv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gchabvqtf.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gapdlfenf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmixonus.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gchefgdvv.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gfrijepav.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gwnzbuedx.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gylkjphub.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gslcunpcs.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/geftxkzdl.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gzxzlvnmt.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gupeclvbf.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/geahsysan.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gnwrpemxq.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gfheypijn.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gwrizfaub.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gmdjbdvft.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/govniavep.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gkiwwaqeb.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gijobcyng.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gxiuvrrmw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gmztsavug.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gxayuuapk.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gjfhqxnpr.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gzdjnkhfw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gtfwmtxsl.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gezjdxkez.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gwpepuwii.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gfeymghir.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gpcwvylow.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gkukdqtgd.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gihsdwybp.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gakvwupuh.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/golzxqsxq.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gpmnpyxme.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gpqalqgtv.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gnpqecamq.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gslhlipgq.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gktcadwaf.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/ghrebqzhq.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gatfltcjf.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gefkhwnmv.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/groefytxp.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gkmqcuyid.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gwfjijnlu.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gohuigify.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/guhxscwhw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gozebqeki.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gnytrqfua.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gauqvaiid.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/ghvzrzncu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gkwtrgpza.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/ggvryjiyg.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gasdefeoc.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gqucobpxb.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gbcdlcour.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gfuunonfq.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gtuabzjit.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/ghhehhnhu.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gqellaxsu.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gywepmixv.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gdtniysrm.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gymzcvztr.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gvpldbfhn.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gkhvlsdez.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gpzrffqst.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/glswkxbyd.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gckopotqt.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gtdedbylf.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gwkysgetp.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/grhkonwah.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gxyulprov.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gtntyikpb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gjwnzcaxd.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gdfvaoubd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gacrvulcn.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gxpmpuajw.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gumdkhist.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gnvrixcxe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gehhcqojy.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gzygyqcoh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gpnunbcyt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gcnezjrdp.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ganpovirz.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gqsbvbjhu.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxbeppnrh.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/geclilbbv.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/glwjplelo.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gnujqdnti.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gyozaxbxd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gdlpgnlkx.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/getducstm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gsodnzvpe.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gmqfdouha.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/ggqodpwek.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gdtbwjvpp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gzlbztnmb.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/ghvjsqmfx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gmyjoebzl.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gykawxhii.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gpsczuhxw.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gdreolyfi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gobaccbfe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpvgpfkfe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/geiucaomp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggvvoaakf.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/ggiahkhrz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gixykttoi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gjgtyvowb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gplleascw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gfrtkoqdo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gbyhjfgfp.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gdsrlcopp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gyyhdaegd.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gcniqedsq.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gxadjubyf.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gvjpjylji.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gwrsqacxf.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gstthrtga.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gbhwmfmwh.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gtspuyqrf.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gwbmhemxp.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/ggsqgzqph.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gpibquuoz.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/ghjexwrmg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gyqlvkrkj.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gcaphqnqy.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gdsxkctmh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gxqtzujxp.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gpetpdmci.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gsgwubbau.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gxguzhnts.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gyfigqbpi.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gguymqqee.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gfuvosnqz.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gqvukglrt.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gljgwecfe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gxphmdjiy.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/guhtwxrec.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gbiesvgjl.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gpacqeizm.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gbqheelpv.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gslyskvvz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/glxuolkzq.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gaftsdvzk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gwphjkfde.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gnghyomey.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gfcbhytbq.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gctlogzmc.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gawishfcn.sHtML


<!-- 参考信息 -->