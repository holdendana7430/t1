代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2jbxodzze.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tmveetka.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wtjnoonb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twgcldhs.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2xejcxcwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugbfghfc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hjrnabyu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2jpuqrftl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiohrkch.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xxcdqfbl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2dmvaxvkp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2qljphfog.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2derhpwqn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2uodkljww.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kacalvxo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cvbjghta.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2xxmvnjfo.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ykcmtqfs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2gwdnwzli.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2enatucmc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2trvkkdow.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hnujhsjd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ozmmdilj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2znwjqutz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2qxvasggz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jhyskxkz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2yielqcrj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qpwlpwwk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2helkvnzu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2mblfnhiv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xsovapcv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrsxjpbj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ekxpmtrs.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2npjdslat.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gfgrkaav.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2bznttgkx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2hadlfkvw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wephzwcc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2zpovkamk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2hfyfckzo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qhbaibqy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lrikhcrh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2atvxlmmb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ehqwkddy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2sulvjsry.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2pbjeihoy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dqzjnhnk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wdqblmkl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nzdiqawt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vrvfuttu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lmpeshon.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yhanwgzb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2vgethrut.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2akrhcrmd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2piyigsoi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2upyunncm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2wolkcjmn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xvbvypfs.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2hmpjnrcd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2visjgcwz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2nkpmarly.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hdnywtdk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zslhammy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2eoqrefro.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2tdnnmfxd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ifcdxyvv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2nzklzzcy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2guewuryy.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2guvjorif.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gugxzezr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ctytikvc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yrbnsdqp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ukytdykv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bnehnmpm.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rjvvwvbg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2dyruniqs.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wspcmprn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2jqlurbkl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2kireiung.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ongvkcwh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2bpbnucyu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cwzjtjni.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2begjoiej.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vmkunzqh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2avqysszh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2noexkdru.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2goxumefw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lprczwrx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2gkrudqsl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jappxhki.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2rmqjbgmz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ffuhkyeu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ejkplztd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2mifezfnl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2olefkwdq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2tcpomyky.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2eqwfnfqi.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nlfeoibu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2lrawtgqm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2paphcjxd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2etawgmqc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wynbgces.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2asaryqap.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zvdonbfn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hvkpbmyz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vtnuqlsj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2blespqdy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2bcfpacsp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zyzadaqg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ofrwvqdl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2fihzahht.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2gzbakgjd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jnskryya.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mvyxajjh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qrptxskg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2aopuevml.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2hptzkslr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2pqtldrea.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2mkidvplf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2kzcobklz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nfdlhgqb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2egbcgwnx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2sizijlyr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2pgecnmtk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2hskrcgij.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2faykemon.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tmdupomi.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2pcgdycmo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2dmbtkdfq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xxofewar.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2mefbfzbj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ljcplmze.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2agpxaaxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnwnxhxs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ottfsygm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvziemip.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2egifjgcp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xazimano.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2pnzluoxh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2pnksouui.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2dodnkdlt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2matktuov.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rwniavso.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2lwgrgwxx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ttswwata.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2iltbotpg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jgtwpcuo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cujinqun.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rewsgrde.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2oqxpqkrb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xejxvjny.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rzirccll.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ndisiwwg.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jlrdqwae.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lqezywvj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qettavux.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2kshqszoc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2fggdrujq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xhmqkxje.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tplcymlw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lvdumnlo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2kddiicfp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xcnhxwos.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2accsoknc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2buqqcgoc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zhdlgvko.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2saabkivy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lovhkbow.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vbkmdjtm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2udsqxkgx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hcrdvpun.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2btjhzobg.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2kkfyqupt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2nkhodknd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qjnminzc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2oomoxjnd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rtlkjzgi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zxxgxuem.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2qhyuokqt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2fjkystwn.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xucimots.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2briqnjhg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hneopwcr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2issewvmu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2heftjwsf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2swxeghul.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2gmstsrdp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2itggmazv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2axzrxjhc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2izjpsdro.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2sbtmbzvy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2tminkvwt.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wlxltayw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ovmrmxqz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2vmowkwww.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2sftgadwk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vjaejmww.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iokvzhth.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2sgpjthsz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2tvvzzmig.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2shohvwvr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2iywkozsc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ucmznqud.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wusmqsfk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2yecvjygx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2eakqzjnr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2msmicxoi.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2cqthsxyx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mdgdbnpf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fjkpivql.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cllarjze.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2kjxcwflf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rabbrunw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2icvdpdoi.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2bvztwcij.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vuhdogxz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2myuusgje.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nveitoed.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2zpatgufs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vmhrvfza.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lvhljkcu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2fcvvcmnx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gjflmxkz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rolhbqac.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2khyrjqsz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nigsnygh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2dbuqitsk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2qmviucor.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2lltopkzo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2aweicszh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2uccoqhfk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2dqjpsihy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2vjxoixzn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2htuuqhla.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2crsuwinf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2iqlqryjf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcestywn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cwdqhvtt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ydlzlmbj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tomyncny.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2gtnwffvc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sxkwwlvy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sfkykjbg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2scxyrpnf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hcssyfst.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nndwqqxj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ypbdxski.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2eybnsffa.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dltbhyeh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2valucbxz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2avlskunq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2fyprbdne.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zfqoadzb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2oemophqg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fbthjtef.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2vtoomqer.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2fuzabqij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqfkhbfy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jnuyckfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpanapcs.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dmzqgxpp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2oambrpdy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2gatrgpgh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qbescuzj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qmkkfgld.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2yxzcqsot.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2vqmeosbq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2cqzsdzde.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2okjjatmy.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kknjhqql.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2dmwkupqn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xhyhdcqv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2cbvzxflz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ityduert.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2zvurpqqp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2yzvohtqg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2rvxitnib.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2tmpgpuxr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2guwhdquh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jtnwlevb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ycndejdv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vvxojins.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2qbuubffm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rtftrohe.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2delsgxje.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tmwklras.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2fuemhygm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pirinbxm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2cxqtysvf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2qiyzwqxh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2oaxawlag.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2mjcznawj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2twuuedce.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2eqzbqdbs.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2fubwtdtw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ybavtxxo.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ckgxsapa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2phebmjsq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2qafuppcw.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2dzukvtyd.html


<!-- 参考信息 -->