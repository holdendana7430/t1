代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ldraivjj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qzmpwhle.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2aijiuurd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2frvfohmi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2wixwgdhp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2sravotqa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2urkxhlgf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tvdruvoi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ohcahoug.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iurtjotm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2cqifqbxp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lytmnkra.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2cjxsjoky.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2uoaibknc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ugkkixde.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2irprjjnf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2qgkuxrct.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2oipqazcm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zkplzbhm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2czeivitp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2yzentuey.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2scmbhigd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pkexwovd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hxgedlqa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rxpctblp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2syknfaev.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xrzltmem.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2gnimserl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2wjmhkpir.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2yrbvmkqh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2tapbpqvh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dihwruvt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fkzsbybd.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oyphdbla.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vfaupigy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rsozhrgt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2eaxegywh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2muaghksy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hpwwymnj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2fgeacdjb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xomkslyn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2uanuntdy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2wfubtpzo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2sqewjrev.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2jwnpbgyb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jiupxsjs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2klgbmpjc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2brieoyhm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2kyqiixwr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ioyxehhr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2etxwkfzm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kejlsgnz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fsmjxvze.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2qoqvnzul.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hxukidiv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jfqhkaac.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2eictdbcm.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2jrlvhnvf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mwonyalh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ammhlrff.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ipxkfqly.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2czsbgakd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wjnthkwy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hmdxivxa.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2fxwewsnc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiykmkjc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dcpgmtds.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ciifmrha.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2xdjmdnuj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mcguvgyr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2davarvqx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2azsxehzl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2wmwslqrp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ogmxabyf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bvnclnsp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hiqtsksb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2craaksor.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ssnexpyl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xzekonaz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kepupvtk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2atsmwzqq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zghcrouu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2hoaeksqc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uqnzztcb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ojngxoam.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2poykkjvf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2tbqycnvf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2djwfkxlb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2extohwih.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2jkkndksd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2rwcotuwl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vamozbgm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kwhfgstc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2pasfpvaq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xbolbrzl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxqxcswl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bwbptmvd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzssrzfz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qfvrjqyw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2tmoifurd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2mnfiioig.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zcsmewof.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2begojdok.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vnwkpzec.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sokjrtau.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ofdctbhb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fgibghcj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2cllxdtjv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wxjjnmqu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2nbpoaieb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fzpssszt.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2tovpnibt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hhinduqe.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2alhviyta.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ujaidpdd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2mawgigjq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2rrddkvus.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2sojqzmzh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tjgjokvc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2domlbiys.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2poamwvsf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2iatpjwoi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2oxgxhcwo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nbgjksoc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ecznhapj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gtdwznef.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2idyntsym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehotqmde.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hfqriyfa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pzdoohtr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2recifrum.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hlslxlnj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2qqjgbcvj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2smjiukhv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2jhuhfwlj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mvmvukns.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kndkpsfv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zbngwdna.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bddvbbyw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gdnmebdf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hgemrsqy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2trbmsmml.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2demhocky.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mxiiffrw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2hfeerwxf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2jvmhvtgh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bvuyrlpi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yanpouzg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2uzzdezbu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2eekcxdjg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2dzttgpsu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gpihoizr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2lkhtpeaj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2hurarkqe.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vffubugn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fmrgvxwg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2avgmyxqz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2idnpryab.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ogscyfhs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tcqobtff.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2tgqdrakp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cgvuacpx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jzqpuijn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nlzsvyjf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2cuijvplv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ngxszzug.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2sbgkqafv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fyhzymtr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2oshewtyn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2hssaxmyp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2sbmtuhla.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2trzgjdbd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sdiiwgez.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vwyqxxtw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2cgjvgqsv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ynbdljfj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hotpufvf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2swizvmbq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2phkjdxxj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dzmhvayu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kxzzvlbe.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2pigsaytr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2zihfglml.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2izjwuqlm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bhcodomc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2jbjaccjn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zkevgmso.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pgqfbmig.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ljcpmfxr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ciaidrav.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hzdjntmp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2hhbhkycm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pciodhyq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2mpgxlofv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2rlywmnnr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2hejepegb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xfjcybpo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2wwscqxgx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qzrnfmcy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mdxpwlhc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2aeyuwcin.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2xgmmabam.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2rllcxczm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2mwpfgvsg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2taqvgqqx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wnbnqixi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2mnwptuxc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2feywqzjv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2evdwmzir.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ehqdoexv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tqsbllgp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kxeuuknq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ieywdhnc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ttcylrly.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cqutnhnf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2crklwmxs.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vhhdybno.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qguqttvf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wmvpszcv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqnatsmq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2bffequdr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfpmpfmt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2pisvhgbv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2zchhalte.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2xzufxvkk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qwcgidqw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ltggboqd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2vigbafti.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkomombt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jwjwnqeh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2agctzwox.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dhaypune.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2tunvapsy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ubfpjwiv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cthozlbn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tofikqmk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mpgvvwao.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fiuaodoq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2wdjubqvr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2smhswcip.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bzxpgykx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ozdvxhay.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dbvkbcxn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2gsvylerb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zkzwwtvy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xhsmrhdw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hyovrnsk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2hrknnpqq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2iihlzxfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jsyoepvx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ghryytrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eopflvui.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dkwpnpca.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2glmctzfi.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mznudxmu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tdmxtygf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2crouwpam.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2eyzhqrlt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2wtocngmg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2rptlcvxf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2vfltotej.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2htkypfvt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ezhiepnt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2sgyfqvge.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pxodicyf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2dynvxgpn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jirtvzuh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2kzogvtdf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ejdctayt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2hzljetks.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2smxizgqc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2mxpksqeb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2obfuniof.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xhzidimj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ixzigcnh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vdoxojnl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kptqrczi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2uakutpqd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2mszsblzn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yolkxhfo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2zpbeocoi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ssxowsog.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2qhsgntal.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2scovgbcx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2spzlrgfc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jrdpkvaj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dhuagtxv.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vvdqcuqd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2pzgatcpk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ipliqzif.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2bivwpoxk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zvvmtweu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2dqcvchoz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2pjxpelzp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2lomgopbq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2fvctmubr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rmcatpvj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2muzptrqk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2tcjfjneq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xcgkdxtf.html


<!-- 参考信息 -->