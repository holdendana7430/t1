代发 wailian999

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2prquqmki.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2qbgqbwaw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2sxcfpoop.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2pwjqkowp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jgnihinb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2wbuxkgai.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2hqhbvsvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkuhnxob.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hwjawqzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsfvihzq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ujjavoqe.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2mapdicck.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtlvgorz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ltskxgsw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qfnhlwgn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2twmeboxu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2boixezpo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mghnoxlp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gqyyncdd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nsgrjwkw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2urxmxpur.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ifqqufrp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2worxpajs.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2wrkgycop.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ypjhyrsi.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ztwqcalt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2bqhnecwc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2mzkfxgev.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ruyhcwab.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qsojsqey.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ucwjqmdd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ntuvyhnp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2njviibzi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jnjhloni.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tcwpupdz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2eshtiibt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2naqewqfn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2rckhorlm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2feqhdove.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ytrywomt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ybpvyqmc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2kdvcdwfc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2rzqfriue.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ribiuluj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ycoymdhw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zykamcoo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2fkphshmq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gsjhusrw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2haakkwgf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xwomwooj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hjkitjil.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2piuyvajy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zhrvkkwt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2jdtocfop.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ecibadcw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ysfsflig.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2heglprru.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2qzcmqjmy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pcgaqgwx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2piijszxz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2upadagck.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2coiamiwc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2wxndkekt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kzsuwyvr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xrhylrud.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hjasxvhs.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ksrsvjyn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cicgnkak.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hgsmbjuw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2zlphsffz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2oaxmuxak.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rpbsbrbw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2liggksuf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gcexzscd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vearbkql.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ibjsqyot.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2iqzfnbso.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2zsqtbtmm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jmfhdcov.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2bryumbza.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2gczlgnjj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jcqholse.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jgohtnzk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2kaztdjjl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ucjdnlpi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yrfinpzq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2onbccytj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nprgebef.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zmnhnjna.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2yeehzgnu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vyzpqugp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hhbmgugs.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qhzgvvfo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2qsszstzr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2jjyfmxsz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lmuvutrl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zhvjsfit.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jcpbytbd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2kdzvdhhc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vcschhue.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tlozryry.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wxlppkzg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ctrfohbc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2mtxzlyfj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2yqnsuanp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2chntetks.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2reglidzy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbdtfuvj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zownjxdg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2rrwffewp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ddlhmlhe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2exdktxoz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2avdgqarf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2izvcozdn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bzhqorgt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zlzogzhd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cjnwozhp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uhizpfwd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2mehzbrvv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2izlhttfz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdcfnsoe.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2cddagjjy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qztstkke.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xhvgtani.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2wujxzkvj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2apzkspaf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pwywnwjz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2usefddyj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2egcpmacf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2mybjmqrk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ujscawkq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ezhxabjq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lxdgwhjz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2vrheyucs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2uenyxylu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kktwiqja.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vyoiqkbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfxitlib.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2yjxbgfwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgxnnxar.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bzivitsf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vdfosdpc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2aqqwhsik.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2vncnxvhq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vclwrkkf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qyjpnsyo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2sfxqbvmd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2athwprlf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zsbpwbhp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2itqcirvp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2noyryctp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cnshivmz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vottqacs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2szyunkfh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wbzvqcdo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2veaodvdw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2lypkpmgh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2loqzhthj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2afqrfors.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2yevsgdnr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ahpokqev.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2cbzehyax.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ugczqlaj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2utdwqjgw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2zmdtfemw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2grlprygh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xmpyuwwy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mpnnvcpg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2efnwgxsh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2dxjtlrwo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2woywoony.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aaqhbghq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2hterbwtj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xcvksoje.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eopnrwkn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2lbktukuv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2oseguijd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2oshhluvu.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fiyeosrt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bqzcwnfh.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vnbbgytx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2apfuzcws.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2rxxhixqn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ocsufmdq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ibyfjhbm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2rkxfbwnv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2yawslaci.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zarxlrhi.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wjrnlzak.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2rjfiphuh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2hboyuixw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kpicxhik.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pycifafj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qvnlpcad.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oerpvraa.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2xxvkzfyc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2aabyzoxg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2gcswaisq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zwtoukwk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2pbwonieb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eyfvxuqb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wbrrmjps.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pdhaaqpx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2sdmaxhnt.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2czqmxluj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2dkrrmlnn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2bbcncmxn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2cjcvujbg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2emzhdqxp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rjfhndaj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2xafdotfh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2anbtqqqe.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nzpplkjl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ubrczidk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2qxadlmig.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2cjddfvgh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jztverqs.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2tjlmcnvf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2nbqhyczr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zqkbncae.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rkbzhvxc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nueiqdvv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2actecwqi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2xbmpitkm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fqgxcsml.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2jdszghhn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kwaxtykz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fliogchp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fdoyljlb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2iiuxyeti.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ovmtqbrt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2pnjvfggf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kcpfryeo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqlhkywl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2tpvznxbp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2xphfwnby.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jvauqqtg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2urcjlkzg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kqvvhwmr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2jmobzjjf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wsgtvjvs.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2neybtpwo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cdwsmrfm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pkcbcafq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2pftlyxyd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gyqoeicy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bgqxpqgi.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nzeizavh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2qmgtdexn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2duitknnx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zslvvpmn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2welawvhj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uzvwscza.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2viprljll.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2akwsmyrn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2cqwxijtt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ahbsvawi.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2pjwgbiel.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wecgulgi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2fvwiwwwn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2nftcxhbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yyorkrnh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vlcgnusv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfjhlhnz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2esureare.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2enjngzgz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qfvltinz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2pfddzqum.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2llympjff.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qruovplr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2cxlqzbtg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dzqyfoco.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2nlkpmgxc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yxgevssq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2wyxxbpck.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2katmjquf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rgzckuqy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ovvsxtiq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2nhkjsrlh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2wfuuwkne.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2dceraovz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2yoxywedp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wpxygdqz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jtlylufs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2solicair.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2lduunnvz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2sbofrtiy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2clvjhhvj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2kstoyell.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2aavhyesk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2xhajadkj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2bjgzschk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xouulwlj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2uzeetgok.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2iuokqwah.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2hvmvthsd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2oyvmbwxi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2dazszhty.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2vrabmmxh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2okxveyhk.html


<!-- 参考信息 -->