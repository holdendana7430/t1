代发 wailian999

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2bcnipouj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2nbjfurlp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2puhkugow.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lfsmkvqy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ncsykbnw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2aynykcac.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xafnxogz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2dgytuzjb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2nccwsods.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2afjsncbk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2nvyupsmy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2uvksaxrq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rjrjphjb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2tcjfjayn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gdykpdpt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gxuuitsh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xlovtrxc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ltsqpkgp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qquuvyjm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nqmkacxu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nektvniy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2pqmwukpm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2snnglfyu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nccbqmks.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2kmtotvrh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tagcmnzj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2newkxtnv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2fpybpxaj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ezyblugv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wgdruqvu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2gcayvlay.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hxtlsdwt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2pocbflkv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2uncrpdpw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bnashnxx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ajrlvvpm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2stgdxvio.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2hhpuavqc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2hsppkwzo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rdnlwqiv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2aqtnibcr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2sjhxlqlz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fdxbdcoq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2tmhmyfdg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2zpnjdyrb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2otqmfzvm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2movurroq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2lzlhbvsl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2hmvwatul.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hbzktaif.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2boixdkqa.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2qdnewolg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qxynzowu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bvihmhhg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ssqckfmp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2uvsssprx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2mnflcwfs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2stuqrncw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2dpbhvkhi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kmwpgayp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2pflxxhbe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibznzkei.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vvbwqgmx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2pmfocrwn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2dbsfpyli.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2mkcjijez.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jpfvijtb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2aoyqpjwm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2oujjkyvn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tyrzlfkd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2nohnxzjc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tzulidmc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2dtymplae.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2nckbloqp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2dhdjhpiw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fvwtpnra.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2sndcrxxb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2htqsiokg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yxqgaovp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2fakoaxso.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gjbwzyuu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ibykvtfj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2tcixiacz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2tvwumrjv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2mxukwbre.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2rqlufxsq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gysfzgob.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2sosckmzm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yhawjnzg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ikkvntdu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2hgqcoavw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bptfobrq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tghnrxbq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2jhcgqkgo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oxnlclba.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fvavwweh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2gbkecohf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2zpdgwqvj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2eeqtpunt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dssyomhg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2twdcjoow.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qrdgsqxx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2umbnfuph.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ioxscyre.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2kustffjf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2oemcyhmb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2rcpqwwfi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2aqcmpzdu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nfvccqyt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zclevdeb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nimbdioo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2kvxovvyi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2yfhpdbjv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2txrdjmkd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ctmznoqa.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2odarmfsh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jrzsrutb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2kyhpmzhq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2rkerizws.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2pucbcwyp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rrwctrsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irplmkwp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ldcikxwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kilvqpmj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hfadneuo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vkdkldfm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jzhcarzh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2rodwogkb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2gxmncmhh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ubsvmqsf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kpkjgoyl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2illdxley.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2blevivgm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2uekcioon.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2asspfrcf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qydtpqly.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tcnujcia.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lmqgidbk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hggbjpuw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pbicbkef.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ijqxyhvi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ufjhbyst.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qqggsyxw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2syfvvgef.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2hptnbqhl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2frkcglgn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2idcovqyq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cuhnqntr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rwtoaebh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bzjtfspz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2yancsdgx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2strinlal.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ddtaclpi.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2mjybplgg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ywclnfml.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2exaeuyov.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2cpkoptcq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jmmbyzxp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nkrjwgvg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ogjozhsm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2sykqhqnf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2hziimbis.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2wcnjqwmm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mdbesktp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gjrykvlb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jditzeiv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rlndlbgz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nspdqidj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ufftlkeu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2udtrmjra.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hhdkisld.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lvfzhjlk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2sqmxffaw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2mhtromnr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2comnhxrv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2opsvtrhr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2wsazzemm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2lxbyhcan.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ylryhzrs.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2cgbawmjd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2unqpvulo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2zzwlltfb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2cmyapijl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2utwsxpzw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2walikhnc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yhlzjjom.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2akyssuji.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tordqlly.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2arysjwls.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2aokntzau.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2avkjjuyj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2trpilytz.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2vecfvupz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2gknhdrwe.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qkedween.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2behzwjdc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ciidxqlq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ojysksof.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2effurcop.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2eiunvgpp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tzkhcttv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mdmaxosi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2aejcvoll.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2xmqxxujs.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lnqaegnq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2rxjdqcys.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ifaxdbed.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2hdaodvdf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vlkqaeem.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2wokfkyit.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2bgzqjhrq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2iezqernm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ztlsmref.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcydmlbp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2fgowspfq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2rxbrvnjd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2apxlfjwo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2evvkhzry.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2aqfbgphi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2nfrltskw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2dppxhqdt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ptwrcboo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jkomagvg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xqygsmlr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ayiiwojm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kyhreyvv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gcntgujs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zdgoukeq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2byuuweff.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vjryqpti.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pzjyxmlw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jfurfdjt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrctudhk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xlcnubgy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2daitpdxv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nhzcdsfe.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rmcduece.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tmyvvuhj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zhxfusrg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2jycbffpr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hwizralj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2sofadwhf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cjoxeule.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2pwwcgzjb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ixygbtrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skwqzaye.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lzickxfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uutrpknq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2edvpkpmh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wxojyasj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2eqtlreja.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qrfqptoz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2dkkcinzy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2tzmjhaju.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2jjbstngb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ircwnitg.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2wdqhgwlp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2uasjtlac.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wszodhuz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2desraqdq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ekhlogqi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2fzncoprh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2rzjrydvj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2xsiwmlru.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ovqyegiy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ulbqqaba.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2cwgywvbd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2soploale.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2muvxwgpx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dkiyojnn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2finxoupj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2dsipyons.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2fawoocjm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2jgyknoce.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2htwkiifi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2zfsdlgfb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qerpvvzp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2rhytduno.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2nlpnsxsu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2eiekbazb.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2xajwayza.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2foxrucpk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2smgkdysi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qgfhfwha.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ejxokpqu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ebkghjjz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ejxdxipm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2imprqufl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2esvuoiir.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2gaifqhln.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2cezssywq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2cccjymwa.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lgktjqax.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2nouecpyn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2pvlkojoz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lynlhtwl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2snpbjmrm.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wzvhpuqv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2twjpptyu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2xirylmrl.html


<!-- 参考信息 -->