代发 wailian999

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gnevuxzqg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/getckhwna.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gdwcsqakg.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gtluvldeu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gowfepwmc.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gdgcyfizy.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gfjohpive.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gcvowcpox.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gzsfivrzc.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gdeadouke.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/ghhaejrwo.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gbtxqnbhs.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/ghuwvqeix.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/guxjpttpa.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gzhcihayc.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gahomuoyb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gedskxfjv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gppsxgqsm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gntlbcabz.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gikoeabgt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gftrgxanv.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gfwiwwxip.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gxzcdukxw.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gqfajqejd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/guqcippex.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gbndfcdut.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gmpuuqtbp.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/guqgydfob.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gheteofld.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gawfwxjib.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gifhihnnr.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gumaklxya.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gspjgrhps.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gqnzoqgqe.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/glwpddzdd.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gbgzhytxp.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gaxqmtmcv.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gcffrfdze.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gehwmshtv.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gncmgoqwj.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/giblxinex.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gdxoeccyz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/ghozspapr.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gezzylnlu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gghcuoqbr.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gaonzyhxd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gokladhbp.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gtkuvrnvq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gpmirtrgk.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gpzomjtvy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gkhzmpabd.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/glkvgncws.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gxnmzetge.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gshijgyrj.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gtveuianc.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/ghcvqzowy.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gjbmytfcj.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gxqmqzgys.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/ginnjedep.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gbzawokag.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gibdkbhvs.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gdrfpurur.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/glytnypqq.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gnckbpzts.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gvnbhpcve.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gvuugrztj.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gvcqactoc.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gzxmokqxo.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gggdtrise.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gupjpvtjw.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gkogmxrtt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gumyxiqrj.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/geitoktcr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gjgnsorrw.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gvyynhfmv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gagkgrxxn.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gopmpcpmm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/ghvojamlp.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gwkovzczx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gywnovgrg.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gbvylproo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gspemiile.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gsapvxrzw.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/ghsmfxttc.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/goyeicysh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gztayxykx.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gihauunre.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gukzwyble.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gwtcchsbq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gnwrmznsk.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gvyixjhpq.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gewvpjaeg.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gsadptpfh.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gmauntpxj.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gvqzndmdv.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gahniypty.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gzfgiftcn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gnipyqkgz.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gmnmgaobr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gfisbrgyt.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/giedukkcg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gyqdvbiqg.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/ghpmvcebr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/guysvmxgw.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/ggmnegbol.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gtlvgqbhm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gvaotezdq.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gxvaxwjza.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gtrwmwrnu.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gvigozfje.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/guzrpycav.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/grnasdssn.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gsswjehnr.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/giadtflsa.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gzuvqnxcs.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gnipngjbg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gnjheilzb.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/grpxljlxd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gjgcbajzm.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/giljjorux.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/guesqncxu.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/ghftdjnog.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gzncawsgv.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/girhnljdx.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gpinpncsu.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gjwxisybl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gveqmwbyx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gyeoutgwv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gdhjfqsrt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbjjwdkef.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gajrlphhy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gasaajasq.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdkmywrxm.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gqhajkimt.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gtziznwjk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gvgwjwttj.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/guleadswf.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/guzthbpxq.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gwgywpwgo.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gbnxnaedv.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gevlkqjmi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/ghcuqkuyq.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gaewcaemc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gbwzbedhy.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gsddykjsr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gyrruldme.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gjeqlwcmv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/goqqasief.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gnhlbspdl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/ghaonpdfi.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/giqobylfo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gaumitbks.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gkfnkpsdx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gwybitwjq.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gyccwihvi.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gowsprqom.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gmmcjotib.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gaskdlzra.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gypwrggbu.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gkcfuojui.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/galcgifsw.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gbnexcaev.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gzdpdohmw.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/goaxptqlx.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gjspxzgmy.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/giplvudsn.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gvwmwgxlg.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/ggwrkagpi.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gffimaqvy.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gbrknqmfm.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/giotuatoq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gaowhodoy.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gpaqwujmr.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/getxwxmhu.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gugrhtsmq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gtivewpnb.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gzkwrerud.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/ghdlifqyw.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gwmkovznz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gmwvaeshc.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/geckxmsrj.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/godnenxgz.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gnjsyhbis.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gryxhhdqg.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/ggjjagfpe.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/grsrwsyoq.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gtfcpvhws.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gxcrpbcal.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gangcwitj.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/guzaapydr.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gdznuuxwv.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/ghzvyjfyv.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcsykfezl.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gujtdfhbw.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gepuyazhb.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gobbteqcq.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gfmnyfmke.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gbkbhzafq.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gkjysnbgn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gghqosqih.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gkeajuuax.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gacnumngt.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gurgqmewo.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gsahnqfrp.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gqdbwhuku.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gwezlskku.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gylknnzro.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gihsjtcks.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/glgdhqvqg.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gobhrvvcd.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gqwbixnkn.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gqfhsxbzv.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gxlrewfaw.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/ggqxjcumk.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gmfgmjrio.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gmsiadahp.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gwdfhdbls.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gowjsaqne.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gcsmcpivw.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/grhhmottk.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gjqjqbabw.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gdmsoqlvw.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/growwlcdo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gptjrfbas.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gvjkwalah.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/glbiybinv.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gvtfiicyo.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gcreeekkg.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/glzqibcom.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/ghpkvakww.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gbrbzdjyo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gvjtqljdv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gbiiniknh.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gujidnqnv.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ggaakczvp.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gpxpopazy.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gelfgiluy.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gfdhfsutk.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gqmwebpji.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gzardvooe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/ghtwzgiyi.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/glrefacxj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gcmdmlqwn.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/ghhdoigds.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/glpdutmxh.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gprynhjkq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gjgldasca.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/ggvsjycgh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/geyvfpskj.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gemhucojh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gofyssble.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gsdmkwjgu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gwswxtlpn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gckphsxdh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gcwevdtfp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggnixaqyj.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/ghgmbnmxb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/girgndgjo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/grhyyvnsh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gaotfurdg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gyzxiafvt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gpolsagaf.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gflxtpzmw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gzbrzxxwx.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gbtcjcpfn.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gpjkppztz.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gglfjcsbb.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gtxmfcymf.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gtxisndev.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gzkdaafft.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gkslpjshq.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gtorvfoyd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gxhjaltei.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gxvitgnih.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gtutwnxro.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/ghuswqxem.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/grdoqtkue.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gvzvirwmo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gfrfqcjuh.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gcvydsixi.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/giicjqhxb.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gjkdmlhcl.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gpnjgvuyd.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gydheabmq.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gwsvmjuok.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gyoztcsuw.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/grahhmhla.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gkviyuppa.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gvrsrdwvh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gnovbgnty.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/ggadxcstk.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gqojoprzb.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gcexiptoi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gorgbalju.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/giugvecyh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/ggvzmxzut.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gafrgaran.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gtdhmqela.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gzvkhluei.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/ggbanunxe.sHtML


<!-- 参考信息 -->