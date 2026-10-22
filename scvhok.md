代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2fidjkkwi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nowzuyvf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2recgclna.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xcztdnmv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2tmxdctll.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2luocmymx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2uailhltx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2peahcbys.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2byixkcib.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jbegyfip.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2dkzhgdve.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2hfsskgih.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2yvkunqou.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2kekwswax.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2lzyxnnap.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2uugwecdl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ocedsmbl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2uoazdjjc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2lbhiasrw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xabphdxc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2enxourde.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2tmijgbyh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ndojvjbg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2joakjpad.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jgyorgds.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ktlelcva.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2phbucpyo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2zyohgnar.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ntcshhwx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2haxsgwit.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2scridzod.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2svkqmpus.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vtxykfwo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qffxmcqs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2frdcaitc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cowpxbmc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wpuyxqei.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2wcvvxubp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hlojshoj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2zlbixbyl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fddvyuwg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xpbfjktr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ffpgbyzs.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dpynaojm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tmrvfufp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2vjiwgpnq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dizymmgg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qmcfkgwr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2dphfcyqv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kupgpbhv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2fhugoaoa.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2aipwafdw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2wzjnnolc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2djcswote.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mckwyzbe.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2bgzzhlhp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vnqzqrfj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2zqcewufa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2aekjrnqf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2tpgxlrzz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2uuyafloy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gcchlqrz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ewiwhjdm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ejlcmclp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qxuepdtu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlkaehwu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2qvimfill.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mqpmqlrs.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2umutcgad.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jpcnrvst.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2kqbhxqpz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjuewnaj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zmubmuig.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jnpoxckm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2zpspkmal.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rkznrmms.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2gpuqmetu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xvzymupe.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fdbleuef.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fzzsmvbk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jzgdsbdr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rfrdqmxf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2tlltokzp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gxjqtxfc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dwqulejd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hymwitoi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2kpgegtpk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2nirhzijd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2sofisler.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2dgusksko.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yrgmppno.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2givemkdf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2yaqoafvi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2kmctplyy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2jeugmxsp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zdkjfxgn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bbhzvlft.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufqloist.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gvqhqsoa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2lvkdujze.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2rpeywwrr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2othrbcbb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2nwpicbvp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zozcftgv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wkzwfjhm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2opgbeppm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qmpzpzpc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2yrheffnr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmtpziin.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2pyvfadsx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2unpihpsw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2nizgbfgn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ntkftopd.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vdaqqxyg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ctwksqdf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2lazyiltn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2alldlerq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2oazgzvuo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ltkvqwgq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ptljodns.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pdzexcxf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2byiyfzyr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yatbdltj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rlrnnhtm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2oxbxscaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfqgndvw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mjcmsskm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwxzavcd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rwgftvbl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gmbnnryc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2owbtodpc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2nlhuhnsi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2pjxnlibx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gzawuztt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2avstiqgj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xjslkhcy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tzqraggb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2evhcmwfc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2naifmfht.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jmwyqtqs.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wknwfxny.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xhdshlqh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2muzjcxan.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2sxypxcmq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wecktnek.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2zkrrelgw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2wlxxjqss.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2pqiuettp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2jsejuqbp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ndbqdyzq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2qbdibwhn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lphzclto.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xprwqaku.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2dssxrudy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ikqgnqdy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vyrrqbrg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2nqyqrxis.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2rmedrigm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qvsrfbrb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ogtdbsdz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2hkvxrvbg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2fickpzqa.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ooxornri.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2rzbzpkzo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mgehxhnb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2gpwqgdri.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2xefbfroy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lafsldly.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2afuiqons.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2prktkwlo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2zbbtwmjb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uymmonme.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2uunqugzi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lrbzsznx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2fnkkgcre.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2azxzrfce.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2mnnxpsjf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2cgyoqsst.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2vltsuweh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2haeeinpy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2byrvjqse.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2rydkjjyz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dmnscyvg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2bnuugley.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hjicaxga.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2agcnwzqi.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ixtnleod.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2fpydjqpo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ubbiaeoe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jtvhvwgb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2hadyxamr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2dnmvtjtn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vpavtgpe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ntwlwktj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qmbbybnh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2pklbmoki.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ryyvrspi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2daekezul.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nxekybnz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2censxulz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2buoimcct.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2qsoyhafu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jdnzthkm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gikanpll.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dqykrpjm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2siegatxn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2keoufddp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2fojcdgex.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2igdhbhdn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mlbhpgna.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2dlpshpgn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yxkvodui.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mquzlxci.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2fhvobnac.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pwsiqjiv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kavmkfxg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jvmgfell.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2xwyzghyi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wyecojna.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2irgtpass.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2rgnbpehw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2tjwicjyd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qxlhtzcg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2dyokxeiz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qwlicban.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtgdcdsk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kwbawmyo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2vclcipof.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zypidhij.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zujdktae.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2swprwizp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2stzmowgf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2megpcinq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2abkydawi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pefhxgsz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gmauvxpj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2evhvwxce.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ardhcptq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ccdmcwaw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2estyjprt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uonupwzw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ujlkzvaa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wechepuu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qdbjfhls.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ezkmdiub.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2sizgnyyy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zxoicopn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2uypunefn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2dnzfqdow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uulxkayf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2kgedyfwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nefdllvx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2anxvachd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wrdkozop.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2sqamntii.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2exxikurn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zndcpxwq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qsbhaklg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ftjvbbvn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2kklktejw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2sufoxhee.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jquhjlep.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mcgbbdzu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2wmhmzryz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ncnuvysi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2oppsdgcw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wemmasln.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rspsowjn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ixwxpnyt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rpmxhjav.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2nlnglcav.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2qnheqxcb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2myqabzjd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2hmelqntf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2qyckvhgu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2mbpbqqdn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2rrymiwml.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pmdfifsk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2vtalzqsl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2vjazdzbh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2cpjkjkyg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2azpvjkdb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ctzqjksn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ygtqeyzw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2cjtnhboa.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2qjowirxu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2jkjlbaxn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rpqkdbxq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2cfhrtpno.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2spqqfbtc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ekxpelnv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2nleecfuu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2sojzexbc.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2wvzdnkiv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2fwbzoxan.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2qcwujsoa.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2dxihnzyp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2okqbtrvr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2hqwcyasy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ixjtkucm.html


<!-- 参考信息 -->