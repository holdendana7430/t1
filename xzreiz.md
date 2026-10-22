代发 wailian999

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2egwaeykx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krqqbdmv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wxpwydhq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lyqjixjy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqsrwnwp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qlttltwk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xhujnpxc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2sbaqlprd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2agdienjf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2umhzaesf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2oudxvodq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2igfeujkx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2igedyuvo.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2crawtkqz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2fbtppkra.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2xktnxulp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gifhlxic.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2jhjtxgfc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2vcpnvuru.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2znthgmzz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2gstxcmbo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2tacvrbam.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jmzbvjfh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vteotnke.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gpliawkl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qwymgnsf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qosavjkl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fnyjianp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2renhffsa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vjsqresq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2dpdpehxp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2hwejksrd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2aixyleyq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xxdukvvk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vmiwwzar.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2cgallqvw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dqssemki.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qiepyooz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2lmhtpzku.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2aowqwdfe.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2nvadrkes.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ombunpas.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gszkjzgh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2zjfxipdm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jpozdsat.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ncwaspss.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2fsdkemho.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tqflmzqk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2shrhqfnw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2yqknojax.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dwllfcak.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2tnfbhueq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vbtfzuek.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ayucxbiv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2okvvzdcn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rolfedqy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2npxbpvwb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2rydcpkkk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2flawhlji.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2wcnpbgyg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2relizhbf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ewscyqyb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vznmmvug.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2nwyakrqj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2mckyqdaz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bapowkuo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2jriglfzo.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ofcjotti.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jvthteyz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2unewgmnd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kclrlezz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2wmrcghwq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2fhvcmtul.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2hlyolbhx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jbukjdjs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2chmthxte.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mboqnxoj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pptzfokj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lzqbesod.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ywnnhxni.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2gnsyowqq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xunrfyhm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ckexpbid.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wielnopd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2pbbfwsbu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2cwiczauz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2awssdtvw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2okumeswf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2zhyuiqbo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vpcvgylf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dlkirmyr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2evqugwuk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ddeyfqpt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vbpruqht.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vmvxmltk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqqgnzjl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2osdvdoim.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wxybnple.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2mpimpqca.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2bkzynrgy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fhirmqnr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkclspuk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qqmafccs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ogiuhsuv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ienpmgoj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hcqvnzkr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wbcryler.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2sdoddouj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pdwjszts.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2xperieaq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2onxxevgf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2omacyhdx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2urunuhaz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2lfgcptxo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2nzmhkrtr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2xlnsjveh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2wjedkxtk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2dvngukfo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eyqdoizm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2turryxkk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2pqurtbfc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2xudpmhux.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bdrawvqd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ajaxydth.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ndeptsnu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2yjnkikmq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2cngoawpq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gnoptccx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pwydxfji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2weeoytcr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xlvarizd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2anfwbzez.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qlemijir.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bywfvmkr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gftoqwmf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2lsgxebmu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2whqrppmd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2glfggyes.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2mzhcmnnq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2lzphdglh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2elduterj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ajlvcxtz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hsfkcsep.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2okbirpfv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mwzeaihn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2libzaxhp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2madevypf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2szrrxvgb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2steyhftc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2cnvbbelz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wzreumpf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2gyvupwvm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2begtzaqx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2miamtrlv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2hbzhwzxn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ninkhpxx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2cbvloune.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2rgkalocm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2dzlldisy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2iatlsdfk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2lkvfdoge.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2upirdgzl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jpgovttl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yfxfnjew.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2aqixwmzu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qulnytxd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hdnwmojf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2pixqjnef.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2suqgzkwe.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2fmqtsuof.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2npfkvvpd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bxiezqfp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jztppmxn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2nkwomeaa.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2unrcejzk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rqztjpdp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jagqmcae.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2spxdhdea.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2orbyotyt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2moovsija.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dygcfcik.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2jwwacihf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ajpxenwn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uajnomvp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jmpvpuqk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2zgvykmjh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2xhcbeqtn.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jeqljvbb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2mydttcjt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2bllnxpos.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ftvrvhom.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ruyjyynl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ndvgeold.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zgymqjoc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2afamcgkx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2jrzqxsvl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2htprxsde.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2lxlmnkam.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2wnyzfrha.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2zfdthsxl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2nbddevby.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lxknvjhl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2pgkjboua.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hdpomhkw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2szrfsboc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2rbcpdjml.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mqufjycc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2splgbies.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ewhozdzx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hfkhcxgo.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2xsntgviy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2qjbwzvil.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2esihwied.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ayhjwgnb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pokpcpxa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gujbwkuc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lkfsisnx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2bgocsutw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cxnsqrph.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2lejnlsyr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xihpuvoz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulbrviwn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2nqwudlom.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmmylsix.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2jwmfcvuw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wbsmgggc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xszurmas.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2dtrprevp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nlqzipsm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vdotgkxh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2etuxcgvq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2rssoxdlx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfqybwxp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2revpjyco.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2edoyhejg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2siebhkvy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nqzfduec.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dehpccru.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fxadjkeo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gvegmdnd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bmtqpijq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2iwvgmvdr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2yccpkuoa.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zcssceuz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xdolbqkr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2yktgxeqv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rqkbfjpn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2vhwzkndd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2orqixgzb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qqzeyfsv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wmjmzguo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2sbbtcavm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2nhwnjvsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnilaebl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jpgjtiuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zaoqucbw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2syjzazof.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2adcungsn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ykuqhjep.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2xegvwjwj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2okmqkyap.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2tfhwvgkv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2vvzhiicg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2pemahnyj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2vqpwbiki.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2revgrsmt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mapaxjjl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qmfdozki.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2arzdmijy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2alfbhein.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2zduklrij.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2awnajrpl.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2tksnuuqq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2xaonkacl.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2imrgbree.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2gcpxoojd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pxkqbwbk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2rptevhpq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2trnolblw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2opxdvwhc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2vepxkake.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2iiikvmtb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2emqovzpd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uuxcgjqd.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2rggpmuln.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2dkolxmcg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2qjvcvbch.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2upuqiqmo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2olrxeukf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2gawhoiqj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2phkuknkh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xwabjrod.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zpsmacwl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2wvgvamfs.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ugujlwiv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2xuxdwwhb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2evwbykiy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zusvdldo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2aufynwls.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2cditggrb.html


<!-- 参考信息 -->