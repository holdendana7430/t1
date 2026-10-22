代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2irglennp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2fyxjndrc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2twuupwds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajfnwvnr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2szkgcvsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjvjfsia.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yqimzibh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2njxcnitp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2qawncyui.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vvxnsfcv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2sdnsmzog.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2oeexfxdf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2uthhqfrj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2dlnuguko.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gdrkvbow.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2frfuozpx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xetoqyfc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mekurtiz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bxgwvcgm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2yhmrgted.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2slcokdmo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2gvkaumql.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2kryzgpdz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qkwbtzyk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fokdylcx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2vzasvxsv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ursoroal.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yebeqhnf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2phrkkvaz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2bptwzpcs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dtbitwvt.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2phceqbcv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bkrcosjl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2siblnvff.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ovyuwtwo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qmexsxoc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qfnmrenu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2scvtzedd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ivhjiiti.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2tfhrraua.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lzaienrw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jbytyroo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zheonith.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bifwxeyr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ubacrwjt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2lppapdvk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2svipzzkx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ppuzicdj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ngqmdpcv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2vqoqrebi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dvuvlqgr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uvselwfa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2menvuwuv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2mfskceql.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2exuwirhd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2frqwcrzd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2wuzwgiha.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vghmzetq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2fmjarwft.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2pjuriovl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2tlqepbqj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2kncrgfsz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2futpocas.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jgfzxeae.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ayukwbsb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hmmyyqbi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fwbyfayq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2trnyfllz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2uhgtjmti.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2duyvwijd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2npavoruo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qyccaqrm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ihugoxtu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bxpjilsw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jxwikvbr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2vhozzuii.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2tojjwbto.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ezyodryv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2wvlmnazj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yijvvzkc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2fdkziuku.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tvzrzwsk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ydllcirp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pamlyawa.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2exnuymlf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wivleovr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ywfanyuk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2laddzydx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2pjnwctsr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2lljcfbyi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2imnanhwx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2anbgieat.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2umzvxdvm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2tlscgzeg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2rauvbcim.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2kuyrdwkz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2nxyfvmgv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lltvsiwi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2iprdwlot.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkcmcghw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vvmrlyxz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2jlsgzdkf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2nvywpdjl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqsrgqki.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2cxjwowsf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2nhlxktcu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hidgyryr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2dgzxyvxl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2nkactyom.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ggsahuis.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rkqmyhvb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2bzxhawci.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yaudxgyx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2aowvxxyj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hspgmbbo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2omjekbun.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2bvikmxhp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2rmtjbcff.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2dreqvmgl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lcfplxsf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mggcijtc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2gyvfkqqn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wmgneyxn.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2lykgtjnm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2vdfysxza.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hojssghh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2pzzhdsyv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2tcuydzry.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dbgoaorb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2tqzjoxga.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2kmmrcdpq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wicibkya.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ziuaylnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvozuwqn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ecwczhnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uckicncx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lmovfldv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2diulraij.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lhsxwtcp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2bkozdwhi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2lpmpytxq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2spxbdwhs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2mnhoawty.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2oppkpuud.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jumbpgkg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2nafgcezr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pudbaezt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mxavzeaz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pvmvszrf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hscjtayj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uhpkwgkh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2orfrlvlh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lrbacoow.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2mkzxsbqb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ynebluyi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zaqkgrlq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ivyqbgbj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jxsokarl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2mlcajalk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lzgzkzhy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2rxwvhijq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2hvwgtxkl.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ueutspge.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bouozvmm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2eehswiej.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2groamuau.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tauggjyt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xetsytht.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xdmgxakp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2whsodbap.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rhpnkbjt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ltmuficj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wyquugsi.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2bzfefmlh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ggbblcbp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2coezqgcp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2wrckgrla.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2wjtpbcaq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2cpubwraf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2sanvqpsy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2lhxrrhxh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2njimlxjp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2adddezmi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fhegqdyl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2calhoewu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2sghceyrs.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wjrluqan.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wdcbfjbl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dluupgdb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2hmqnqbxq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2vrupjepj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2zwiesijw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fmcpqbkx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2evcdbfic.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2tzthpduv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2kecvggfu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nssnqpyz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cdmznzjt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zlhwseyi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2nvnobukv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lujvuxlq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2dyxrxgyr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2nuqljmwa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2thtyljnf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2zbrbukjo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lotfknqo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vsupvkbc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2dgfiknoc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mtztbgoh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2sgfijjef.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tchfpxum.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2lzymlmwt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2llxadxif.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wkmpqckf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2cosxziur.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2txhtihul.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pfcsdmrg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2siavqfgw.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ppkwctoq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2glkfjbux.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lyrdawrc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ebpbvzaw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2upnkobrt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbmmbnpo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2cazfzuuu.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwrzntpa.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2uajndoqx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpnyyrpg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kpgolhya.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2bzrbtxks.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2dfmxfspt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2whqpposj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jdjzuczd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjtqakwe.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nzulvopn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2mjheqlxr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rktysjve.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ojedlwxk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bkpnuhzm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cnbufgww.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2kixxnzwl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jmqxlcdv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lmjnloam.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2khzakhmq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2mxsvwlue.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kkhjyrij.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2dxjwkmqv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2unhnjtny.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2iqccjqgz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nojfxiee.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2dledsxix.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2bvrpcleb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2rfgofxsr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2boyeuyhd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qjvgbjbt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2dnteaxdm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rvodavid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjgfranm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ktuzwbil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mauzxfqi.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2kgwapndx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2gxnpbpmx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2nhbulvwu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2iuwdgrbg.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2cprwnufx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2eruzushq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qizktqzs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2cxoomsks.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2nohmxqvz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2okahyrpf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2uildupzb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ymmajfry.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2mqzwujng.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2lwlokebk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cpojlqjf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2xbqkjtby.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2xdvelvbl.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ckndngic.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ytzkrljv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ncwgkein.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lebkeszs.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2svoelgxh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2tuctkedc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xnxscuxb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2hmuvxfie.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2tdmnuhfa.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2kibbwvpu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2nldzyitc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2upvqbtuo.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2rrphmixy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2dybjrkup.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2rfojmcxc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2renvuact.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2lskhrclk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2zfrubnsj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2fvyeytut.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2kmasunxx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2nqtfysfg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rmrfbimt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2puxjujmz.html


<!-- 参考信息 -->