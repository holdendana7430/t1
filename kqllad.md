代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2kutwgyzf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2pelibuws.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fcnqcpiw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2vpmpwspx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2cfhvusck.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2bvuxhldw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2okwcnpdw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2kitkdcup.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ervnhiwg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vzaeriyx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2wouoyoma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jddzhtuo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hpzsqvby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swkdttde.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lyolthgg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2wevnumps.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2qbrkybjp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wcicbtwz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2yodlngex.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2hipxnnvw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2pbvxqloc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2eswkziht.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2fbqfymvt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2efxudnxa.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2qhlrxmvl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kjekavar.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2fftzgrmr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2qpyfukra.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2accktach.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2dphcoemo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2htwrthxy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ygphppay.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2kpeofqgc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2xpeyngtz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ftjcdhrc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jzstbxgd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2hejowjvb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vgmypcrc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hxuvpcxm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ioeiyzja.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fwrizdjs.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2jetvbyiy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2buwtmqas.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jtgenzno.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qqvwakll.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rjkvgmiw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vtzmkwjf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ijrdsubv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cmurzzao.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2safmzbyw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2mtnattba.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nfssswmb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ecujazzn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2njumgscu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yktwnjtd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2fuidjsyv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jeyhfjew.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2xipelzmt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2lhsothab.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hygwrvmm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ohsgtbdv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ogbjgcjs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2arnzzgsi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wfqnjqhh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ybqftvmh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jywhnppy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2bczottuq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ashayblp.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2mdmzpevk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ofolwvgs.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uvjdmild.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ksgpvdbd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2exovmwfq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2lmvwqxsv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2idnhride.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2dusgsgmg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fjfconoo.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2tfbjltqh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ehzupbbz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hsdtskwx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vfmsfpeu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ffyakqhg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yegbhurr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2oitsuekr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2famhcevh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2woexukrv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2tmnuijkl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2opidzkow.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2oqndkjmt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dlphncqp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2olhsmpwj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mbjursky.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zouhxcvf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2umadbnrh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2yovdfpfj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rbeuaigi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2kjcrnyvr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vqpyjfcd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2uofmmtny.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xfrwplcf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2vrqxzqae.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2etdkxjpk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdtxdhsn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gbmmlsxm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ujyrfyqw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hwdthqli.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rqmzhxyc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2zpafjvzn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2vvfygrkf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ogamhiio.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vslflmlf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2tiyvddqp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2bflctsob.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2hffkucaj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gssshntl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2scpuhqlq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zokhplfv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2oeuiarvx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2gaabyiij.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2lmlvxptm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tbunngjv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2prxdrugo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2lxvimdft.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hhqdlnau.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvdvtrnr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ghalkjqp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2xccyerxu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2hcopiyon.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ukfiwwof.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mobdqztu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2qjcdvzme.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2comglvrl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2glvppabz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2obkrajvu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rirdyjkp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2sabdyhto.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mvtymute.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2lpoqhyoi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2iibygbii.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jxeruaob.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zhckcxyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdxcfqzk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zywkpfuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpoaeasj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2auxqzhvx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vokmmuzx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2tcbzpzqy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2lnefdweq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2vwfifmeu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jjtsaaef.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2hleedmvz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2gzpyqqqp.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2gxzcwguz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2hevhflvk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bdlznecx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ikqtzppr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lrswurqd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2sokkxrem.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rbwhdszz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jingximz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2pinlcqik.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ekvflmpp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2sriubzak.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2dundmvyo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2dnjnkwbh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ixogmelh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2rgzgylns.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yvoocrlx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ayerxusj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2mpexxfww.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ofqsuptb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ypqcvdvb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2cszbxvno.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2vvqcptxq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yakjusyq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jtgzvuna.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ufzlqtbu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nzkxmwwe.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vbwmstft.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2eiqboixp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2vjlxoyeg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2xkaozgpn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ctvtfgww.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2asbpbbgt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qkcuuwuv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2uktylqdc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2flrzfcah.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xbwuyxal.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ofwskfgs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2idxofbjq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2blzkozdf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rlfzssph.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jigswndp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2pkumlfkr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ummcjjzq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qdhunvol.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qmuwsjfl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2cqjkcemc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2fmxiuple.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2kslodazb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2izellban.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2oefqyzts.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2vnnlvelx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ihqjjvyl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2drgptgcn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jypccyiw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ovhcnefv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zdkydono.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2xqgaauwu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rywxapfg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2rxtltmab.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2xuwshfde.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2dqgebvfm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2foqfidky.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oabimlnz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ycwxbvie.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ukrkktcs.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2pfwfuyhu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2niowebup.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2cjsrfurr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rckpykji.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lcfsjpba.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2otfnrlve.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2npasvido.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lqjfhsni.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2qlslmnjx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2irbhxlvv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wfmlfdtb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2aptcoejh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2rqqgsaqi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2evvkupkn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oardrses.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wlmrvwdq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpdzsiks.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qwwoxecn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2nvoowhqo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ancpceim.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2gjzaibdw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2loxykuhs.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2rmtezcqw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vhsjszhx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbuftcqr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jjafkfvc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2laozprmp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2fkftauof.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gdjcpdrz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dozlmrkd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2spmpwldm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2fjdcdeqc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2poexxrke.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tenrkjzb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ystmmezv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2foaoxxph.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2erxnhnyt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mkttcmzw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2bdcwbqmg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uvrakqmb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2abzjqxor.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hvveokxd.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2bviwnred.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2whvwwspc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2mhmszpbq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vkrdpqqx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2gwmbnqwr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2tmajosvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acpcahtv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xfbqvxyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twukhmsh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ligvhrzz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2xdjmcjjx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2zubapcjb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jmolovws.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fdheohkd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2bxxpcyen.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rzegqmcm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2eptxngyc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2zfuleqfo.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gtkfosjp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2hawyhbft.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vzswtfal.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2trrxvdgs.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2rqqxcjxd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lmtgblkr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2quyjldrm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2szkdzybi.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jcbholav.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2arcbnmod.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2vmvzdyio.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zjrkdwhw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lyevsozg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2niouvirz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lpqyfnmn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2qnembtal.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ahwvzpha.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2vnmbgwnd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2tdaiapci.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2paymsqjd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2kwjvbalb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2yiagleds.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ifucbruf.html


<!-- 参考信息 -->