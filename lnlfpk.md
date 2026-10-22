代发 wailian999

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2pjswrfec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kedbuozr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dqlhoqjn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2fblttfjc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xacpfczv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2abzxafsk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rtzdhxyx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2dmtoxuod.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hvneqhzb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2zgcqizdu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2aoiytvpf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2syyupfzx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jbcnnqej.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gvqgaynf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2yueihipr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2qufwfzkl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2jtfxkwps.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2dtpcucyj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2qpscklhb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2quiewvwr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2loipktww.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2afdpeckx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2aqwhuvyx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kfhdiihn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2dvpbkfie.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ymovpgse.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kbvkwmwe.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qqujlung.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nvcvuhnm.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2bjpjtjvu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rmdtefpz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gafindrv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2lbjrqhwd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2eocikibs.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2zdequnpg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2sqkcvvei.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bfyhzgrq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2upmktgaz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2xcfmdgbb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qwmcilss.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2fdcfyosf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2uahwosgn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zjimbdam.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2nqqjnlbu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ysxcaful.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2oaxgnscr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2tfrlilxo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vuiufmbn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2dqmcdnfm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ozgvlhck.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2mjkljxkr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2uvewbqvm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2bkburslc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2cthmtket.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vasyjxlz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ujhsfacd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xcchubnn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2uswsbcva.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2psydmtrl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2fmpkjjer.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2anveiyck.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2mibybvim.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2nywawgfk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2dhszelzr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lewnumyc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zogjzduk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2dforfmsw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ljyznaou.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2dlpqaqyp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2beanxsxc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qvtitwmb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2rhlddqbr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2onnqlzlx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2hxdruzyv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2mzkezpbs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuuyihfh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2suncseep.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ysiiruxw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wdnbqfmv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2btczbyoy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2iftreetp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2wuzixdds.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2amebglgl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2msvzhonk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2loiahnvt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2dexwdzxm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2pvyuderz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ignntsjj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uqlunfqj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ggypvuqv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2drvveejj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2mmtbxqul.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jgnrskwl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2dnzzfwnc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gbpzfide.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gogcrzkq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ohykzoif.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2rvdrimyp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2smbprnsz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2kgeeiyiz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2iqqbwvpp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2nbnjfbcs.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2azammemg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2wjmueeaz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fnnagmok.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ahudiwem.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2shdhtihs.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mpqqzwzv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bxvqzewn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ibklfpce.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2qfszuljn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rtzjivoh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2pzgglpxg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gzxewjpc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2kzrtepas.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2opdyxolw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2whofkkfa.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lcsqcbjc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2kgcqaydw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zdkwyxjm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ktrdvafe.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2lncgdhgf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2cxlgpjgm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ggptjokm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bnhpgeto.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2tujpjufm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ucuorhhy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2rxiqrmvl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vumozujh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogmbfpgy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2swstbops.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amojrxie.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tpmnjsne.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cujtxzam.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xekjpxpa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2fkffvdsw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2nnzgofgt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dnsngunh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ccfccyyf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2qybadwml.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nzmgyvld.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2hckzydqn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zqctogqb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sxofznqw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dvhiyqnq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2sgmbjpdy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vhckxbsj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bwaijjpe.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ghhuyvms.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2cbcbymjh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xtxwnkne.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2grtiwsdr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2pgtmnsgv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ncbluzzh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pfgreccp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rtfdlrxs.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xteaqdmz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xnvicbkf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xphqgnhd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tcfddlni.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2feahgvvw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yqjfuxpq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nwkkaijn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ezzoybwc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2fczryrne.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lnkvsvdy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2savhkevo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2oumrisvx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lwtrizzb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2blvxbajy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2afbufqoo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2tlsodnvq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lbocgnmv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2utmrjcmt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2xokoqfyh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ntxiiwug.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jwzmwcuo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2svsihzur.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wuscbblg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wxlfkkyj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2lrsvuokv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2xzgdsoep.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2jxnyderf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2atlzgplp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ngljljgs.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2jhgbhpqr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2eeyemxnj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2lkroqoie.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2tzchvdtk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2iwwkuhjg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2lsjdsaez.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2uirfpooe.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rrpzbagm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gzepxzhd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gxfqlpth.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gsrxczbc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vladdkjt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2toexzunq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2yxxkzezk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2egmrxyfd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2egfmrabu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2jxatqzdw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2fgpuqdvy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2gzjuegwo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cnluftqm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pmdbqqwb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ckgcdgrr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2jzpnqxtn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fytyzsnc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2swapnvnu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2hmoyxeyx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ocqvjgxe.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sslniuxm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2unzlxjsn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2bunthyvk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2olxbdmjg.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bhwjogxm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2rmauxepg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2btohuwkv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdktvlni.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2qvmmsxng.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqtmlboq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2jitzigxw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvebdedj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xulcvrax.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2vzyqdokz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2mrnmvgyr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hlxmezvi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2eugtuouk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxcpjzst.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fqhengzq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2amqypzud.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2aceorhab.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zuyakbeq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xobkgqlw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cvpkkctz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2nzidguql.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jxltvetg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2psjxbbgp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xmpuiihd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lawhmztl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rdadnnxl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2cikeygow.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nzfuhcbe.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2henkblex.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lelwfaws.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hvsjyiyo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2shmavaic.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dinpuiyn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2diiyfkor.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rdrjcbbm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xfwmyoxe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2sadaycoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygvswoiz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pnjutake.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uiozmbny.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2sjjiooeg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2emaxnsyl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2dggsgife.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qdnmdqkf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mwksrmda.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2vrwykvrk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kxbflfbd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2buchrerm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2gzyaiwly.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2swmdtsrb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2sobpgdzg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qfonvqjy.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2gzaagdkn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2pwvqgvev.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jcjyotcx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2clgpagav.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2geracvrt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2thmvnezf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2evhpnqsp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2bbhpvirs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2eiqgsfir.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2wbhqxmmw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2skjssbyt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ztemoquu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xwjdsuub.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2opzjwgmu.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2crvpvlkr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nvwighka.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2mpvsgddc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ynpjhfgs.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2jywytpml.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2fmiwnfzr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ryzufmah.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fpjfebnr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2mzvtwiqd.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uquqbnqm.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2wvusvdwa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2xwlpuepw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ydcmhtbn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2pjdeoqvl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2azhqimfr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2oienbgtr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2rpqruqqe.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2iqujzgqc.html


<!-- 参考信息 -->