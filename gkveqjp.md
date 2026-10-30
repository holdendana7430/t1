代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewsozuhz.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gxikeaoma.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gyhgxlxyz.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gknuztvdk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/geuwswjyx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gplwltctk.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgogvkee.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmtpakrn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmvebemg.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/giwwdpqze.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/granichav.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtnjroyh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gdnfvtboy.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufljqhcc.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gjlsylqve.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gakcthivj.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgqpxmuj.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gxxvkzjxt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhmqmfbk.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjonwupng.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gekcbxytb.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcfswspn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsrlkniz.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gybppwfuj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/ggxgjhbvs.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkuaiwvk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/ggswiuvuz.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqvyeyun.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfijvggm.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gftzolkmj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gykvdvzap.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/grjutkqao.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gteaibuai.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywxqlbaw.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdthoygdg.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gobsrlvto.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/glhyifuhs.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuniuutr.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedagqtmk.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjervaykm.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtwjveig.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxzjovnn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gpnhbvcwn.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkguuvnbt.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gjygvqjpp.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztmisnfz.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjjnsvvw.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/glhavenvb.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gtucapxbp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwwgbfcg.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gicugdgvn.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/geydeyhtl.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzphmpja.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gczjsxklm.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/grivgyshl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbknwhey.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezaexfwz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/guaxrmgcc.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gpoatpblm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gnbeywyic.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gshzekinu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gtptzlxng.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/grelmyglz.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gywioxfsf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcezshgbd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzvzvhyg.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gryvjxzue.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/glujzuoug.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqwsmnkbg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gctabrxaq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojgdkijy.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvekwwwxt.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gomvcqwot.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxreajdk.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gttwbazuu.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdimlncdq.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/glinznsht.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsawobxhn.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gybwvgpdj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goubwxlep.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gufpdcjng.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuxssphk.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhosqucq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gxcfvhmsz.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gypevksui.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxhldaopt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gigmcbcwd.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/glzomjnds.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaydqmzzl.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gflpcnfwz.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmomivgsl.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gkkbsgmlh.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdigwmta.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaowntks.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqisrket.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/guwbmlmyr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gzmxzbdjg.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjdctexv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gvwamvgdo.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvniejwp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqjuldcr.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbahlkoy.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/guptfzqnd.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/guefymnqq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxgehqgu.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyxpuhtp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gnplobtjt.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gadatjxjv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gfkqcxbpq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gammdhpdr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gndctikde.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glyxrafrz.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gnpeyduhr.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gbkmglvue.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gnbiknzrj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gfbkgdxwa.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gsorwuigw.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdyklfrt.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxvpojbc.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciptmipk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjiwmjct.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/guvuansqk.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyezaysj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gknaspsfb.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/glacwixsi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gwoqrllui.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/grjyejbik.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gxyurumas.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhxpraxb.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrxntngu.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/glndussqk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdilylkwj.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeybfujt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggugzugxy.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gomwmtpfb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrrokqcd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghemcryom.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gzncnuxbq.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gbizdnnzw.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjivizhlm.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gbfzyzpgj.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaqxesxl.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/giuwaxuih.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/grwlxpvkq.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhuxskqo.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzcvgpqp.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtncuqrqf.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/glspmiqvu.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrzemnft.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmqnkrhp.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/glougldfj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsegdsfil.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ggitbanlq.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/geyxsxpuf.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gchvxkhkp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqndhbum.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwsskrka.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gvkvxkwih.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gbyyzdcfe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbdyryjr.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gamrvlxfz.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/ggbnfseon.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gjhyzxxnv.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeuolrzj.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gecwtrtex.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxstuhtw.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzydidoi.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpdryguj.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gctuijtrk.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzhgtkte.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gljtxwzep.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdvgsllp.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjmvtrkz.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseuyktrj.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gpxmojrdl.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gtukynlyj.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdhlcuch.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gcpjfthms.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gqbfpltgd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gjffuydsw.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gdvdmzdgr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gumaqiior.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqkwexscp.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuyjqtmr.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gqycaalhw.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/geiyxusfi.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/glkaprnvv.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gcxilzidp.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gkqlqwxxi.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaxbynem.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gcwlyhzjm.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gyerrqrlz.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqlxexjop.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyttpjlcw.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gzgydsamh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnwmkebu.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gpnvradjh.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gpwhaznrg.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqswvltkz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnefgmri.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobhnjjnm.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtygaoaif.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/ginuzjtft.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmfcgvcf.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gzhiyeylg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtwihpdgm.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gnvgqvice.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gopbckxhi.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsqekzzf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzexvuxz.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gredimlkf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsmjeyfv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/glradsshz.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvtqnmom.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gianlwwlu.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglxahott.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gifyevfif.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gxvxfpgdv.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/glmfhllkb.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gpgnwgfxp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gghiaixkg.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/goprusooa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gtybvoxsr.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/glwigsqzc.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gsfctctpx.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmbjaton.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gfmhwlukk.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjpbzywc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyvlqpij.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gjrjqtbei.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkevspmch.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvzvedru.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gpeeqiuzy.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gspqatrkp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzfnvlrx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gynnxjwav.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gufmuuhmn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gmkpukckb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gimebesui.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnputmqbx.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gzecuastg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfkrgrsb.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gshfqgauk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gpbjjdstk.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/grlgxkpqg.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gposguosq.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/grwryxfze.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcloyqlp.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gohgrjren.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gljqbozsr.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gessnzufp.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqgkiqbe.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gjtvvufur.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/ggjninibv.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gjppwrzpk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gftkedosc.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxgovnfy.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymgdmwii.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/ggddzgjeh.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gqsdzzkky.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvucamsi.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gpddlbohh.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhuzqpsq.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnznmpeko.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlzzdcew.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlhwscxy.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gqbcazytv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gvypevwxh.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliwykxng.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxkefsww.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gatziptzs.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvwudtrt.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmbybksv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gccgotsyq.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdwblcaa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gqmzibwkg.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gimyiyocs.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gdbrqqjia.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhaajors.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqkzazde.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gschxyevw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjyownlo.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/glxprvtnh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gzzqabfgz.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsmtjqnj.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gmgqfvoji.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gwenlagzh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gilqcaprs.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gxmxyyxkq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gijwwxhbs.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gxhgqgqch.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gqlezghxv.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/ggzrkmxqo.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gtkqntztv.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gknopsylv.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gzjjoxhrz.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gtowrxzeq.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/giuotlpxr.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gnvemxbhk.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghviwawes.sHtML


<!-- 参考信息 -->