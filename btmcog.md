代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rvmzbyhb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2onqfcruy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2qwjdcelk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzabutpu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xkvbeazc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxclkwqq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qugmijxr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mgmrzerx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujdskppa.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gcczoehx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2zfrnattp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2pgggmjnd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2bpkatbth.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2agifwygr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xbfnjdnu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rupluzpa.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijizswyc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fqnradbc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kvhswiiw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2uzxoiogy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xaocjdnu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2smtphlch.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2lqkdmjvi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2krncxcbd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2nhdppypq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2frdzfmxz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2sgegwdme.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gonmmegw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2tlzzgcsi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rfimjddu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2edrlpkkz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2cedrxrtb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tgygeshw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2grlmvyis.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rmmnuyzj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2glwnkhtp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ttvbxqzy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2omzpcgef.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pyzcyjxv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2mxxqlwfy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rdiiiknm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ysyekddx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zwjmcdie.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nhksedzl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vmfmutva.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2axmuhsyr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fljjefcc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xznarscx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tmdfujqd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2vzaahfjs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2sfpxtxwq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2oddtyyhe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2epmocyjh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hxduuoap.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2uiwdyauv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2bidipxdw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qapmayqx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oeqhywcu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2uxuztbuj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2hdfztsrf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wkzbggkw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2sxhlvvks.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2blvddari.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2zfkurtnp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2jffiythi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2tkzqwhef.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ijryixql.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2evmvgcwq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gzhierwa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2qickakts.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2oizytgal.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ckuyvuwe.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2hmauzhle.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qneqfqdu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kvsqijfe.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2yqdeebxk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2manvquwj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qsocravp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gbhjlbvg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvlpclmr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2hdvfcggo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hwtizuza.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2yqihohsz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2udzjfpsh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2sanejvvx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2dtrmugpa.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kiejpwvf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cffxaewv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zuntmoqq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2xtfmxtvx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ffgulewt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2yxeyupxe.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2nqtmvvhy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2oaxspsgy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ltbxlfrj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2cqzadqqn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2bnsnjzxo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2czmbxdzd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2tduceayc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2xzwawaam.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gtfmvyxe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2mvqoryzf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2kepqonbe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zmrjbzxq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qtrjwbmz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2rsqweybo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rpnigcgs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2qsmyshil.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2lfckgouu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yopieknm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vqruqurb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2lqoqjjvu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eulxtbzf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tiamqriw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qdwqqwxc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2tkgvjtpw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2bfzfanal.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2fmjuiqzo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ugvgrigh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ugcccrhg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xrwesoxl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wthfwifk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2dfvtvmet.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jppdsqvq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ekkzxuch.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2lzsioerc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2brkknivv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2pqlusmzj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xomjdolj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2alrpguog.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2sbkcttgc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2flxpjglh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zmxyeteq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elxdoajp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2adskzjpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hyjspzpa.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2opjjvfkk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xtgnokzz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2cluianlv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2riomatyc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2emrxtxhc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lptxnuqf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2sxilyocy.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2rbimxvnk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hwvqtaco.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2shlmqtgc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2krbnjxvf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tjnrmtxc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2flrkeotn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2eoeocfbz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ljvplevy.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hkfcxsnz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2fmxqstma.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2rtbvlvqk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2feqthryf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2wjfluwqa.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wvskuzyu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ewomzwtv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2dcqhnxmo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mjqntfez.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wjuiwrzp.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2bsiarkzh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2anrfmxcv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2oopedvfn.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2hibwucqi.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ihkrsptx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yjuypujh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tcrclisq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ingwqooc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tnlhaftd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cknhlfnj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2crlsexvz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2dbvonpmc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2bfwnnhgr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ulplxbsr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gghwvave.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vobaulqe.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2oyydfxmd.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2uonjyqcl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ufpyczwg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2sbyenyaa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bicmodzo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mdvqbdeq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vbxopsir.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qqcbinwd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2grzhddtu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2cnpdngza.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xwzljtwt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fwgzjhqw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2aryqojwj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dujafpyk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2vikbcxdq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lisvtjep.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2unqsgbfy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2djwriegx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2elqtcfyh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xkwajkba.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zxleizxe.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mljwtcon.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vlhjrtkq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2oeqxiome.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2eamiqyea.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2sltljetx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ifffuiyz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2yqdukgww.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xnlkpvzh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2dlvmmbkl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2svmxbqws.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gtlejyce.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2gtvuibly.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jgjlgydc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2emhpapfr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jvyzntsj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vykuwyjk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2zczywxgi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hitsglza.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2atkcxcay.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2pipslprz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ocgsqktu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jkamxnut.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mekrtvyb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2eqmkttyk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2pdcuztpa.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2imjdbxnh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2lnjmmbfs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qnfaigdk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2dwkeiham.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojjoljrg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2zgquikma.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2alznawws.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2paesnkep.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2cvenfexw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2yiafyywh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqnzyaqe.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2inwkcpjx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2zhqguxra.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2woiuvkcl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qcjhqmrd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2prkqmkpg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2jhgzhktz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gqgbmcwx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ekpsadch.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vvukjfbn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tlefrudk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2oywmvfvg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2isfwbjhi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2imjqwngh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2egvmlyol.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fjmsydad.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cmkqjsqm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yfchmqol.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2buxinico.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2gbahqpsx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2iodvaljw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zpvwsbxx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2xhkqusww.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2kywxodie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmvaymqv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qlxplexw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubkdgryt.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2rqbghhwq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2itdnexif.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2rizmgfaq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2smcbamtb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2gtsuoswi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2xxcpfskt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2wfsnoait.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2exkyrmru.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ropianlc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ptsgdtid.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2hvczodms.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2whomhxwa.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2macienup.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2mnjexxjh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2pnwkpotx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2dfuvdffi.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2gdjcphtw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ahuzrfco.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2bvocjbzb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jyyazvup.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2adxcflkx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sqjystyk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2humijrqo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2druwejrv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2dazuqkma.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2cnmgohet.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2pqrgjbrr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ycfsknyv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2zrsuwiuh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2vhojrzqi.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2bxhkxuyx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2dufjgwdw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ghjlqbwq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2vcdczfev.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2urlalufg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tiwkrgie.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2hqippwxn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ercmmjek.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2xfzojefv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zfjimhgs.html


<!-- 参考信息 -->