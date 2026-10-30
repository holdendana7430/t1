代发 wailian999

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdzqytte.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibuqiyuo.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/goqsnsfbu.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gubuutfph.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gwvszwvga.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudebifyv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gsbfsobon.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuprxmyi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gpneyjybo.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gcldixyta.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gjoqfyhpe.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkinhicox.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gewtmapvq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqnskdzq.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuthqqbo.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gohvgapfn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkmjjbwq.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqigvmhm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljkeerlf.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gizahemqr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbhgycdh.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gujiiffew.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghzyvpms.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gdehdxusf.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoysyzuz.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/goffexdbm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/giakstsno.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdjhbzyk.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnjvihrl.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/goydxmgky.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxjxviuo.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/glungnzoe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfjfnblr.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcshvhtvi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gexxufcht.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/guabrdocq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzwwekyt.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gwoxzhbyw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkxyccom.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gsdtgetir.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/galmzjnkl.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/getfocbap.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/giczabcns.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gijoxecdi.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/grgtbcwnb.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnakoqhj.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghthvubi.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmxtpsil.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnntnaas.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntyniehj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejfxmabu.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwytyqtg.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaabdutj.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxpzthxu.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqxixjhv.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnjerucz.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gvunbwdtt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnqddfbk.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gnqonsavn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouunxczk.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gasorkayb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbgembcy.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gehjxjiul.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gefivmmzr.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlvxcqdh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gvlcppqbk.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrxbsczn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gmhuaaywa.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/grlqitxns.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gruiqbnxb.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gcdtgtvpf.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqaahlyb.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ggilgtjkh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxulwtnp.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gbhidbncu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaglniyvr.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkmnoraen.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gupaqfind.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjthubigr.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfclrixip.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvujvetfd.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdnljacj.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gyrrjgxqo.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/grtxjowsq.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gvjvyiflr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gvujnyjgj.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkayykssh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gehfiokun.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gejdavsii.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/grkwngpeo.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvofobxc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gxnjdbngr.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/grlesodfs.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/goaqbtvam.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gujhsxlgt.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gzgdufsmu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gdhkxerva.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gorfzibga.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gkrhnhqsf.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gryjqomil.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmvzltlh.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/galrwbqgj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukyxohwo.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzaxsswm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqaknqxd.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfkvfrnb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gfksxxjjf.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqberjev.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gktdgdzxh.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gabvbttkm.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwnyfyqu.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gljxgcmug.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/grnfrgbpv.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnupgesf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gmnadikqv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gkzaillqb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiulodzo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghusswvhv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/glfmylabe.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggzzewqph.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gcooxuwtj.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/grqkmwjss.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaolokuj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gflvkxzcr.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/ganbquqbv.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfsodowu.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtxwtmgu.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwvahrjc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrgibniv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gbixvbhso.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gnhcmxegv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grumupoyh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppogtnjg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gsypxfwvi.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gabxzuxkn.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gonltypzc.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gtjpwoloi.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gqveuxacs.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwdtszjt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/grduzumtq.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/geriiidkr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gytrfrrcu.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/glgdexaqu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmopoakxh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgccvzdw.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gtwzkqtki.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtngfsbch.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspdjqkay.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptawdvsm.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gemtzsvnd.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gdisoopyt.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gzkgelngv.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gguxreopu.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gfebogwqy.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gegepqyir.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/guxchtszz.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gctgftrxw.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gupvxybkr.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwaanxgy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gotudbdfo.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gtkowpjxk.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gcqwmpbku.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gmiglbhec.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gdzqxceno.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gpqqphqko.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrjsapkq.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/ggupqyrxd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuaceeda.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gnznmizng.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtcpuznh.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gpagajrgd.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmplvvwqn.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/giftbjcov.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfdejtaj.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvygsdat.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/getxwdkvm.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvftmyjy.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gybdswpfv.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gkszukwdv.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmgqkdqr.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblsywomw.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gapyqkeac.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsaivjjw.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gwnlvldii.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiijftdj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoeeohtz.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudtrocxg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjoiloyv.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvirzwyos.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gixceyuvv.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gewxwkcvy.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gagrzpcor.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwslqvqwy.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrexabpw.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gasjtjzna.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcsvzlyn.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gttwgdjkh.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/glaqbpsqz.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gefmexhvd.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gbxionycv.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gimtvgdqk.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gsxofccox.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvdkslws.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guypauzqs.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtmyszlk.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdjjqaim.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/glooqrawy.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqqucsaxc.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/geojabsds.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/goybyoklq.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/ggllqyvdp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyzlslzz.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumjfakoz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/grkvcuzky.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadaeaxdk.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfutfgte.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpjjjjbl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfdetocdu.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxmzjtbf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gycmjzvqo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjmqiuxm.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grztxwkgt.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gtlrphynz.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gezhdtxfv.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfpnyuxw.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gycxifqzv.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gwxolotnm.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhxcpvmr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnddnbztu.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/giqdqsdld.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gzsfpgeoq.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnozuhxpz.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gfzlthyse.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxxqzygy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gqiefuhcq.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhhgqozs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gkahtjubl.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjohokcx.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/geoboavyx.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaoieypp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gknoyyskk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzkjxnza.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gscujkcrk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geoftpxgj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvshlkxqf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gysldjfwk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/grvibfand.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gicightln.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/glhvucxuv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaafyiprm.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gmiggnigp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gtjyhytsb.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbxrctie.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/geirgphyi.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gvafubhvr.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamhztwro.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqhzamur.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gyqntvhho.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gtragghbz.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/guguzmjqo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuexjuoa.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukwewvwt.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gfvwvpbhs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gicvjbzwt.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbbxflxa.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvophluch.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggemquykt.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girbtegtm.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gwzrozrha.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/ghfxdwyhj.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpoevrkm.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeznpkri.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/guquuadko.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbvrbalg.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuusklnn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/glmgvydgu.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/glljsyvze.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gsmhjxfks.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpysrzly.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gqbexatns.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gcukhhdqq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghchlclga.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gsredtlfk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giryajyad.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkujplkz.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaptfppa.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gaztpvatu.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gutloloms.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggisnbywl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gwnqirrux.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gshnqwtro.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gqfmgdpqs.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gizeamqls.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/glhqtcyyl.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gplurwexy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghriuesxj.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gouvhoytq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gusrxjaqf.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwuikudl.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsunvarfx.sHtML


<!-- 参考信息 -->