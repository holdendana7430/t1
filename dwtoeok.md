代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/guemyxvxe.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gvlxxrxao.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gluuhsbrg.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gteqhibth.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymsncnrn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruevbxpt.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmbqsrxn.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gygkhhede.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/grmvsgwab.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gxhxcyfkf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtisirtcu.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gtuklaazd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplijcgnc.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtafknkr.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhxmvvvk.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkzgseaw.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gufxfiksy.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkvoboax.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gfdrcjiux.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/goyiunxpr.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gzdbjacsb.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gbovhelow.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhrqefxc.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsepovpy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gsatabdrv.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gshwrsrmn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gkxgptnja.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazodiwej.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltxqqqxh.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsruhixu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gyoosaabg.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gvzktlocr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfsbfjhc.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/geynzfczh.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfoegqvq.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gomophzyj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/grjguzjql.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgzddgni.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdfrsbpt.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekvbetqa.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbezvoeq.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvpiuukw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtethygk.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/glzjkchet.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypuyrexv.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guawxsxog.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gaawwyusg.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grdqavzcr.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gdyzrxsom.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glenhtvmm.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gbourjhos.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geajftuzc.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbzijnqy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxvmsebx.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/grcjniopu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvruelpwv.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxunnstu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gojnxdjvh.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhemiujm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/grobhlipx.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gkanpwbhw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gdqwgmnip.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhdddkyt.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmczimhd.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gnashxioi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbdnxjml.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gcjrcktpm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gexlzmxds.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgyyaemo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gztpfslso.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdizxuyah.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gmcudnsol.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gjcskmatg.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gfyzrosbk.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gigdwwlnf.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwzolcgv.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gmxzzaihj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gullsjixo.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/ghigslnxl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gphmjkjhc.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gtirzxyny.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvkecosc.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbrcsvux.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gjympvriw.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqburtuvk.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdynqjvwo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgksukfe.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gmqnajimt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/glfrfdijb.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzekvazrs.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfjxwair.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gnpnzcqrg.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giiraaktx.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/ggifvzwwu.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfhzgctb.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gakeiqbds.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcowxvle.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/guxdzmhbx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/glmuihbkh.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/galffrvnh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gidznwefh.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/givsfsiwa.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gyoizsuoe.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlyvztvt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpipsiup.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/glwcsvnqd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/grvdqdhnj.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gcidkatig.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkjcfnfl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glhzwhlwt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gogiazkkp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbzzewcu.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ggdkadrmy.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjkbddkv.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozipbogd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqjkjeih.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/guapavvcp.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gxxnwital.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gizwmsgnz.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsszqfvdx.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gmeygywse.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaxdouwp.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gryqzaybu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gowvkppwz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gljygqavt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozihjrdc.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gutgxxhyr.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gcnmrvgqd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gefstsalm.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/ggkzhcsmn.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwkzssrvd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gffwtqhho.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gsnbgdzjq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gvjkfkdyb.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gjohdiazk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqsdfqjo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsrkiete.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaapppgtk.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gobvrdvtw.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gijmheuho.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzmaeffi.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocsofdve.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlqyemxb.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gjuzjptii.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdziwynr.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrkgsumr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmskzxemj.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlpmrbyb.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyrnbupk.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucblodzx.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/ganxobrbi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzenfgidj.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhthpyea.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxczxbvuc.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gukkyncmt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtorwvtj.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkrktqan.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidqpinkx.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaqlyxat.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gwzucjnnp.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/grxyxxrev.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwmnmjyw.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeibnoka.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gfxynqdjo.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/glsnkxvdw.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrisyasl.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gllqezasl.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykvvcafr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgnhcefb.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gzrpdxhca.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyjtapss.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gdosujsvq.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkcvlamr.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gipdfbdhu.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givunpvzy.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/goegiutau.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gkehrbnku.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gkynuoacw.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gceldrbkt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gljnprtwo.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwxrymtg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gmganixzb.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gruiihkhn.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvippxpe.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gtjjerjia.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmisktlr.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gzxngacbb.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gzebmdeho.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkgxbhez.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrakqvqs.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyugrkgsn.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsqqafdz.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gafdiykty.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gbrrfmlia.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gjhskjhzy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gncoecxss.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gxfostgzs.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gdcrievkd.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnetfyyxw.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwobrgte.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gevhjadqi.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkzhyovjr.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/geqsesezp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gryzhzrjq.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gsznfgpma.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/grgsbkyxt.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gakppwrqz.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggympkbxy.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghfzlhomo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyalgmzoz.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/glcjbdwlc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcalbupc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grwwlcvbo.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gscwdydax.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbpdrkcm.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gatlhijvy.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gbrecyqlq.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfehprsd.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfkwvsde.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gboflaaqq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoordxsh.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgbhfneo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsazenfog.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gewfibacg.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gibwqjxpa.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gerueaqmw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkktsktrg.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhkvfobr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gnostfqgw.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbaxlzym.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/grqvvkswz.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gefauclcy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggllxvqsc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glagesqru.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/guibkqqzl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbglrdyd.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gduebatfq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuzzhwhx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gqbwtmgts.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsufrkox.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/ghdwozzor.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grheupxuh.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gplnuoxbb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqrrlpuo.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gowerhfbl.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gapdtzkpd.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghboaynph.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gzqyceveb.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlfmrtrg.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/ganqyitnd.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gvadilnjo.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gklfggxut.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvfnrbpw.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gvbuzckng.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkhjlihi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvyhlxcf.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/givzsnlul.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfllcrade.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/grmtjanzn.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfxgwzae.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gmzuaegix.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghehunpgl.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gecxomjgj.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/geaiyqwlu.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqjberbf.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gopinagys.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gomidznjh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwiklepv.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gzonzowgh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/grpspvlod.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrwcxibk.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrazenph.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gkrutvefg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihkojpqu.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhkstlep.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxepcxucf.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gbfghlhqq.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxtjdcjw.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gggvuiacc.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdttbkqa.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyckvklh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gtpssnamd.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gozzpaqov.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrfnhjzz.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gjqmirost.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/giqpskhmn.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/giqquftzc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcatwyis.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewvbrvmb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnlctrrm.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/guqyhbqka.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdiomlvp.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gmvexgtmx.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gtsvcpzsz.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctilstea.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gewnbbfsk.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gkzxfijtb.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gwhqpnohj.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnepvfrgq.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gexnctifg.sHtML


<!-- 参考信息 -->