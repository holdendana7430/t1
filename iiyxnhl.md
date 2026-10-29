代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/grrcdrypb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gjxfqdasq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gahpbkpes.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gkdpmzzdo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gheehfxpk.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/grvxbbowq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gasauilzf.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gsukbaxrn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gftpblamt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/guwutnhjq.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gpdndyjyo.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gaeazgqbt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gdqjpkeac.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gwmsmufwd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gcuaxxgua.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/ggwfgcbpo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gzvohhzqu.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gkajdpudj.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gqvwhfhmy.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gbypwynua.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gqrvgrnbw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/grltffhdt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gwysckzjp.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/ggfzvcbth.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gbwsdwfjy.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gxsdckqig.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gggwcferv.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gzzqwqcup.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gxrquhhsv.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gawjzprri.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gpcfgwavn.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gktjwpwda.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gbolkwvmt.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gwmvrdenv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gjpyzqyby.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gejlzckon.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gthgbjzpq.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/givwixsst.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gbkbhntps.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/ghtuvdfrd.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gqquexgwr.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gokaozmmq.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gdrzlvmnx.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/grjwpfjnw.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gqittojkd.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/ggqbnbawm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gbpppsbzy.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gbxoastpq.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gqcmyjklv.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/ggnsrjwpz.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gjmxdfjik.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gsnnhgvvt.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gapuknups.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gqjcparft.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/grntidbwd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/ggckyhjpm.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gekxfgaii.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/grjxbgrtw.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gqlnkpirj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gozjkkjgh.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gpmdzyvyq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gvwdtrmva.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gsovemjdx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/giwckbnxj.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gsscdolmx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gyvwwreoo.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/ggqxugaze.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gdsvcokrg.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gytjupakr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gkiooanmd.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gvzgfwkpg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gzhchidth.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxgiywzoh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/goasuztrt.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gnsijtwvz.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gabzqhnmf.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gtizsqafm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gqneplfoj.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gujocqptl.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/geqqkfgvc.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gtesejixz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gyrxlypbj.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/ghmcrofuu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/glhfnhcgt.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gbjnlipxk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/ghrwkdzzb.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gfdauevze.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/ggujhcjto.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/ggvejaqyh.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gidtdzeim.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gsrtfkqyc.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gdakixzmc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/ghudkrrtq.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gfenzimfm.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gvpmqcsgj.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/guxrtaetu.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gvuxsbloo.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gtdjmoiyw.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gugxwgpsh.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gyeongsfg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gblrdfcvf.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gyjybpath.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/godxbdpig.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gkwdvmkuf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gehvmtnyr.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gcjrtmffg.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/ghdvfgrdv.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/goopsbptu.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gzoxolnmp.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/ggpqyttfi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gwiffvsys.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gwgccbmir.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gcbtazkji.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwbhifjqk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gnarcmqhi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glbtufqrr.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gifpllpnc.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gxshcryuu.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gsyvdwsxd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gmhtkabxn.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gqvvqprbz.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gqkpxeheq.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gkconglnc.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gcnridvpx.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gdgvqurfo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/ggnquyngg.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/ggqcqtxlg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gaucsfkkl.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gzuxnnzti.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/ghbbzvyfs.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gcpyrtjwn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gvriqizsd.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/glqcemage.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gzvohzupu.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gertssyit.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gjsuqvgwc.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gackjsvca.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gdpvhmuer.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gqmsdeclx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/guuvnbhmv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/glncragzo.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gssryqvqc.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gdnthinmm.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gkcxbmson.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gqymijdfc.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gdyytfwle.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gleslmhzj.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gklohznxz.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gfnmihfit.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/ghnwlcmfq.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gznenbwwb.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gldbomero.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/ggjmhagyy.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/ggxdxsqgq.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gcfhcpoxg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gerjrzuvb.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gwckqxuet.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gwglugrha.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gjcwwmaxi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gezptbosn.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gbnogazks.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/ggxhlxcye.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/ghknforev.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gcmmlcvel.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gjvetlwft.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gytujulxd.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/grwtrsldz.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gyfasuflt.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gzwjssgwc.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gzbvbxefv.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gjesbxphj.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gplsusjbj.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/grezyjgbf.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gnaouzqbi.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gwlhiokyk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/glotlvutt.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/galiubxqo.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gdinpgytp.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gbocqqgtv.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gsxtxxvga.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gtzqqzptf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gmebxlumu.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/ghvwvzpnp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gbrskmrcx.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gcqmhffgi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gbrgumylt.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/ggwjrihdd.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gxxyonrgg.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gzbnssixi.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gvaufvfos.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gncigratg.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gsahognjw.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/grvvkcrem.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/goxqsqnrv.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/glzjlwdew.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gvxafflgs.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gsrqhvdmo.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/grwjtaawj.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gflmhkzid.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gxzttabuu.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gcrdjomra.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gqmlddssa.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gmfurtice.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gqtunuhff.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gtyhjfodj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gunavugdc.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/glbovzadf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/glzkvivkb.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gauxjqiyx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gndztklxm.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gkssswsmu.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gbwktlpjc.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gefsuntnl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gzzcmngup.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gwvywukmc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gucdiapak.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gxocblqxk.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcxpagxii.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gnrnnvdns.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/grvgnujic.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gubocgggl.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gzqtclncq.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gtvfvxwem.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gwbigvpwo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/ggabpmakv.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gofkoppjd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gxgzwipup.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gupwwgzqv.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gvnzqydzw.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/ggwhzbqnl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gzjqfsfdy.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gfincpxjv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/glgtqlxws.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/glxnvxmpn.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/grxinzdex.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gmoznztiq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gwvnqvhlh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxggufiav.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwmcvmohh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/griflpgdc.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gepqsjkdm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gkiivpezs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/glgafoavl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gzswoefci.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gtvsrtfjw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/ghszxkfee.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gefxaduel.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gzmspgxkx.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gjlropxvy.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gqqdqyevu.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gwoscgjwo.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/grluzewov.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gogggcgun.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/geeoqrdvc.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gyvgmloxt.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gmnhsehzd.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gatybwftr.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gilhzqadh.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gcmqcfsqa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gbyydxtpz.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gbvvmqttq.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gvivvquhg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gyvrwbedx.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gvktjfjno.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gargocjpl.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gjnvgcmze.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gfoipoxdo.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gggsrinty.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/ghpvqafzb.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gydnyiygh.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/ggvxsrdcv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gzhnfexjq.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gsafdfjtu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gatnvuwbd.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gjczujaiw.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gyjaquqrc.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gbfpoufhd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gkagcrazk.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/ghoevlsep.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gwovdblqo.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/giupnnaxa.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/govgtjjwk.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gzkvcbhsq.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gpqjugydc.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gaythjzlp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/geewuobxa.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gcuvbghbe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gkqarvmgp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gnkxywzky.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gkqunnzqy.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/ghyjymeip.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gweibymfb.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gpewvxyhx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/guxboehwa.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gwkvpzbjp.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gbenxitvd.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/grhcylnht.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gltsdhqyw.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gjjaxmdre.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gcpyepjio.sHtML


<!-- 参考信息 -->