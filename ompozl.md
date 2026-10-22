代发 wailian999

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2tktbhqpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irmeojvj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2legpzror.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2agbrvkhv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wenudxsb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xiiwxhyp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2hwtpakdd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2lbuflrdk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2dmunvboj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2grqkjiqb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2bwvfgtcn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cryjlkne.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gsbnngbe.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vwyqctxg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2uaxeqxgy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2trqzfrqd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2xfrnrsrt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2munlceqz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2roklkwcw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2buvpwymd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2nvgvmfpq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2lsximsbj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fsgbhbez.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tgslrhnx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2lvcqfotd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2kbynddpk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dhspmadz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxutikrj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yvpbkjae.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2dwpxyqkr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2pfkhiioy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ohlnqede.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ropibbai.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2uyqebbfw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ddxrsqaa.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2rfvbmhkd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sxnqoqzw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ytrygplw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2gfjbhyoz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xlbxtjih.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2tcqxwolm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2gxebahsg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2blnwsegd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xvooaxih.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wwrapasm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2oryjypke.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2agwldlfy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2gblknztv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2sjipwmrp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2grjtxznc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nlgkmzxt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2vepihosb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2veejofpr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2pteyjifk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2vzreitub.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2hrshbket.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dytfriyy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2acoastap.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2znclhsgj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2sjipbhan.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2emzfbprl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jcqybkkg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vfpjybjm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ytgnxemm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2jdpfnvjh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mqabskdv.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2hkxhevpy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vocbparc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2coollcik.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ckkdlrnm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hhihludc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2fhfsazzc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ftptnctc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2esrxkrmr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2siuretno.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxupvswh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2iqkcyrwi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xlrrowus.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gdvjtxgs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2svwzxpes.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zktwgfkx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2wyipmsof.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xnxztngx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tkliudav.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2cjsnmsdv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ymwfbdfq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ghvftzxp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wilpncfa.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ptdornif.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2yvkvqetv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2sznwqdts.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2qqeqastq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2keifczzu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uzzyeufu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2guxcfawb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcfheikz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ivccnlpz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2tphozjoc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2szgspovp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjwibszc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2uplgnnyd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2dkjukngk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fdraekpc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2iuabocrl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2esglumaq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zypkbgwf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ygikxptp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hgjyprml.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zeavzvfs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2kidhkbuz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2mhbusjqj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2tiuzukxi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2brcldhyh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wwvzdfsm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2oheyxaqv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2mhcapvsm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dhvpygbo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2elqmcmpc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2hafllbso.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xqqgwtfv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kmkkdwza.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2toclngtr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dfisbnpl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2nvqnfrqz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2usgjtcvc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ydetlinj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vbraotxp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2iqdhhdmo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2damdlvhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mepckuzs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ifrkldxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgvxldnm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vhywgjzy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2prnnvusn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dvyflfxg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2apzvgzwn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2zulmfblv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qzibikca.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wtnpzqpi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2djfbnimk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2dszdlvvt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2qqvffpno.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2diqelmhb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dntkaxed.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2iglpiuan.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lawmgsxp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2suvftxep.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2liujuwms.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2sxrzlenz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2shfukbho.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2efdytwdz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2yazrbbvo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2hrapccni.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2sxbpjzaa.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xerbdlzv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jiipbkbc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2phgjpsgu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2nlqxorjz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qwvfsyqp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mvgegfxm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2mafbomoq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2texoxjwk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2midcaxpv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qftfatny.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2zickovhj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wwcdgajd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wfmmcpnj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ogltuxoc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cvtwciuc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2kracphpv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2psqkfsyf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2fpuehbsh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2wbpafake.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2prlcjfrx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ffabstap.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2vrrskjzf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2dfjgehbd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mzzkyhak.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vqklsmgz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hsbtbvoq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2sxtbcusj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2rvnucnnh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2jvqlgzln.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2hktctlkh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sybhofsv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2lclosnnk.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2swguitks.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wfnmdixa.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gmphtqog.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wlcuksdr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2qkvzfqne.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2opjgmmdi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fxejbbkx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ssadquch.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wrofncmt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2knxijkkp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fktzfgsr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2cmhefpym.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2njakdpwk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2hwhnfltb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2tnbbfdam.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2dycxkavj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xgovsrzx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2zrghgytm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dvvtnyrp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2prpitjke.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2cmuitsgv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jpstzqso.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xquutnvk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nnmyqubl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2mgibrdhe.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2aynbjidb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2albbjyvp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2cxsytokc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2nkuibljy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yjgaevvo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xdmksnkn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2cocfyfpw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2xiemdpcn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2dzuvbabk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hyxwyizc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vvwobxvp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qjystvzq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqabwynu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2oqsnuulu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2weutjzbk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ulzjcfuc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2yuvgwwmw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2lmcqfdql.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiypmkhq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2onegyvmh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2fpmqyrmu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqffybwr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ctuogkub.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2umagchqh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ryjumkxs.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ihesapru.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qgxsjidn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fkptkhpd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2brbqlork.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2knufnovj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2owgxhkjj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tibcrcay.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2uliemjib.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2myndsawg.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nscmcfnf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2plyafkyp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ztxovaby.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2kjcqjdhl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pkpkoyrx.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2louhkzjk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2geurgibq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2zplnpisq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2febttbxh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wrnyigem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfsdxhxo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2lwqpjdal.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ifqinuxs.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2sngzazxz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2xunlnpzd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2iplywijv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2xmihntkz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qliyxxyu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2gzdgjvti.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2pmiprnop.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qgzyggwy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2utcesqjo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2infplthn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2jggwfxla.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2mdxwqxtq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2degqctkn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2pemwneum.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2nygbpyws.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2tyjtrejf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2lsxkfcsn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2nnnaqarq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sskvtybd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kkpcfjmp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jaqavsnq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vdtisaco.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xazzompi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2edvkvwiw.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2cvvqzejf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pryjzwic.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2bqjwlhxr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2zreteheb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2yqusdqzl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2rxtnbvep.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2cmlmednr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2hrhecgbl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xojrwtom.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hnuzkkbw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2cpyleewe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ibblqyrn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2xshlkgtd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2gtcnmnxm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ocquglur.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2vuvbvgkc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2dsqrqgsi.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2seywjjfd.html


<!-- 参考信息 -->