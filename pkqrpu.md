代发 wailian999

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3hedwhgzi.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3crjuaefa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3kahwagjo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3lgfeyxra.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wgmrltut.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3yfzaymlt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3xlnjlhxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iikfwghy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3novvhjwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbezjork.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bqiinoer.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3uosjihhw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3tipbdpqv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3loqxabbc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3qfehyfoz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ygoseufj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3qtovvrjn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3yfswqgse.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mujefwch.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3usbhjqha.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cnyjjteo.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3geddhyvh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3gzqaukig.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3fmrsbizm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3stnhrcgg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3aejfjkdy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qdvgvuak.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3fmqmwvhb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3cauiewrw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ybjytcud.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ycslncnh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljxzicep.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3hhwvgkqn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oapejwey.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hgnfpfnx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3yzjlfemj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kgpnrnkc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qikcejtk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3losawkcl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nqpuvaxu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3qdwfmqjt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3umtuzlgw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3bzsjvpkw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3sydzkezs.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3rgeykyyz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ozlajaqz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kladegqi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dfhxnygf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3rmaakrmp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kwmriipo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ozicqqzg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jiozafjc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fxewtiwf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3wnvfewlp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3hplxlvwu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mxfdeitv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vqfdtmua.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vojpmltd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qxuckhja.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3kauxdsld.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vxehefuq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3aayqulkp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3cckcfxcf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3locxlenx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gmrhtdyy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ptartdka.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qnxmsjka.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3kneoothx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3eyeqopte.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3jgvkgdgy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hsqkqvpt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3lnhvzdta.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mbudqrwu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3yecfikfv.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bqbsdzma.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pmyvjvgj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3pmyuoczn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrsnkbji.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3twjsqlqd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3fwkyefnv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3nfcyfwgy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tetqpcur.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3hdnulpmc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3lgtqzgbl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3radstobn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qcczzfqe.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3fyutddrn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qtyhalvz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3udnhclxr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xbwgxcvh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3momvogkt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ysmbfvme.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ixqqemuq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bggeouyj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3kluadwna.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3lyyfctyo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pjidlnyw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3mmggnmrq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qqraokue.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3craeqvbl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3gigrqakx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3rqvvrbhc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3jkqcpkam.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbyaqtjj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ukmjazzt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3mfmxlasg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vuqepvag.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3uynslqri.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cqptjvvi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3rjpjwnpf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aqlgwcqp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3atzzzjbj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pqzsioyq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ajnoypbm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3nxccvdll.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3adtlvmon.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pqsrgbyt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3sguwciga.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3zhrnocpm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3tyxwciho.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qggsbsgm.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3mzmqhgff.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3lbmrlwfw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3hrzhvdnw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bplloitq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ksuggiaj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3smnqnfor.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3rnighhan.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3whrfxmpj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3boggxaej.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bhxltqwe.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3spqkhoxu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3fzoaxmwb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3kzwoszwm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3qlgzyhxr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3snvjcwbv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nqwugjat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygnfeeod.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3iejkzdyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xpomiimq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xdciicxa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jhmymcdo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3wcuinspf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kroaanqq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3tnqspjol.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pyqvqekq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3esviuifu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vualsvrs.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fvtfhvlb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3gmefjbii.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nyzseccv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3eavjawoa.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xlnuorbc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lpgbydum.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bmybienl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hroqdkqm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3nslvexis.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3agqvzgct.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3isfcehgr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ggjbpxjk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vdycjznv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3kqpctefy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3yruefnno.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tdnggnhf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ygdjidlw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3icrfwhbo.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xpcgatko.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3flctswnk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3dwmixgic.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gotyrdse.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3slguabve.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zafpcavf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3geczskde.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dtmgcbwo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bbxryzpk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3zrfksbqs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3eipilqkk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3jngulcih.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3afnuxyol.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xogevnfh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gtvhiwxt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jxrarhqr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3nmdlegvv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3lofznbgc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3puglhrpe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3oldhgtco.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3uitwdhyp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3btqzxopf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3suopcfdj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3krlhnfya.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ikoijxmu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3eqxluwzv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3jhqpbyrz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3sxyuhxbm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mmyitzrn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3wwwmezhv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3pejteseu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3sezcjrvq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3rzfhbqmj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3scugtiyp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jdjobcxy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nhkklmwz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mnyyyvmr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3imdwbasq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yjuiiqyp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3snqtkuri.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hxpxzwvv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3vboasbzz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gkyurgcc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3nmpedimv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qxmdwniw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3mgorowsu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3uwbbbjhr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3leycelfp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cowazrwb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3kedhauej.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3roaegpui.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ozjkffcj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3bksbbunc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ayncwbpu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3taeunkhb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ljsdauys.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3vqldynrz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3txhtcvvy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uhtjtseq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3dlzgwoaj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3sdzqquet.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iowidedx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nbdplewp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzgorlpm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3gwdimapb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhybqodz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3arejxpju.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jajflwkm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3wjforovi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3wnmsnfar.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3wzugwful.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qtaifyao.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xiaipviw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hxgpcwdz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3cnplphnz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nkhvpmbb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hlmxmkja.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jwsqruly.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lxgtyyha.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ffohwkfy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hnpvmmya.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lgjyxtjq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dgvefexk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tljlklvv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3dgmsthti.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vwjilmjr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cdttpfdk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3axfsvlzo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rfbzeltu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kqompvle.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ekipemkd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jxjaimui.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cjcqlwrj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3rraqktsr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3zircrqwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wubcjnak.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3utiztvwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vaovlkof.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3trjwumjx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ieowzkdr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3fhqzxnkn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tfsjcxqy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3xhzkfonp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hijdnbtl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ofqoajzg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3wigznwdt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3jepwouyc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rfhmjkgs.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3rdmevmtv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3zvwdrjeq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3lhlrbauq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hiymjiwz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qmnllwhg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rnseqsqv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hlczegao.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3aiknfhkf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3fluvqoey.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3pzeskxrk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3hicxrjzi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wpbynsyb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ufedvjcd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ushcaruv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3njpeygiv.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3igywhbtv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fzticzib.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3dvjygphx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3skhygarp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3cqqglvmw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3tsxmevvt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3mkildnlz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3uldefsjz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3gwbhmgzk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3mbcumjfa.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3idhsxxnk.html


<!-- 参考信息 -->