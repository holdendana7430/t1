代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gpigfjpyu.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gefaycylg.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/ggvxoxini.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpbtbnuoj.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gtqwtezyw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxwiemkba.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/ggrtetyxl.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gctvbpgwu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/giouiowjl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/guvhweobz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gahrmasil.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gihzvrhok.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/grpxzwxhj.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gpunhrnbg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/guymajebp.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gspzghyqu.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gjyjgelfn.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gocvjheof.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gcodxmqif.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gvjwaxdcg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gttuxfkyq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gdnptdyie.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gmrqlnqtx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gqdrvyjbc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/ghffovuns.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gozmjxxzo.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gdkbwoman.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/glmffnlcq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gxtluonpy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gtfutolyt.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gkquekvcz.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/ggjthpmfm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gjnxetppj.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gntsirsne.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/ggzmwpzxw.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gcgustcwg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gxkeprzoj.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gybdywgtu.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gjngiveey.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gvdolecqp.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gwabpkxid.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gvhoxvate.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gmhcritau.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gfgereuip.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/goclfrysb.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gmnjffraw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gnwjqqrxk.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/ggnzovzlr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gwsaclwia.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/ggfrkhcvn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gfstvnwmd.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gefhobzma.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gdsoyhzeq.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/guhhsnwnn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/goaivuduk.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gejhcuqnf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/giarddwcx.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/glqdpgjei.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gvydpcahm.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gfaiwtisk.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gulrajihe.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gpwykypsl.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gzacgrvwb.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gjfycvjkz.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/ghzncigyr.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnlswbtgp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/grvcpmlmp.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gidaxoboj.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gckhsksgh.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gcvfjokwa.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/guabnucoj.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/glplkysde.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gxvmgkzef.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glqwcefnu.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gkuleayuh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gqxrpamen.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/grpvdpffp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gxtoepclc.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gcdrnxftg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzztzvzdl.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gxizejten.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/glgzxdubt.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gqprgcfmm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gwywaeiyd.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gswmfqyxr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gfznqsiqw.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gzpjaljqr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/glzkvfmfq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/guveadzox.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/grhtokxxy.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gffvpfgia.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gsfyytodd.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gufrjqhpz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gbxgxepvl.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gcmpfyomh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/giugjgkhr.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gdpfntvzl.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/galoflxav.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/guihuflrk.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/ghsicrenc.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/giaxbiaix.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gnxcgriqc.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gmxfjsgpw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/govseebnn.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gowjshyul.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/grrvgkgor.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gocxudwgg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gjocenypl.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/grycgwylf.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/goxmeezos.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/goupneewr.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gzkxrdnfw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/graixzksd.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gqtmleami.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gunliudoy.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/grbwdmvyx.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gpobokixu.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/giqohhzlh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/glfiqdkau.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gnlamfzwe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gqimfhpau.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gibhixxcc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/ggpnnmazt.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/glwhxpcit.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/glzupymzq.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gouhaeqim.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gvxrpaotn.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gzgnobllg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/ghajqsjkn.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gagavevdq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gmpwzddlg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gbxatkluo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gcegwaxap.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gezvzyblf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gaildqgoq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnbqgwjoa.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/goxxmdedm.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gypddhalp.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gukppmvsc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gvnotmkkv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gsmtzbmwf.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/glofuazap.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gzqlslhwx.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gykvnfzdu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gqjjhcemn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gdexrcotb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/ghlvmmjfw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gpssqafeu.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/glyufgfva.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/ggeugjtuj.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gxhpqefbu.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gaayysuep.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gplblfeeg.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gjrsxqheb.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gnzorcnis.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gbnsxrmph.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gdxhdwkua.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/ghglxitlz.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gzdwbpavs.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvaaswjqk.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gvhlgdmud.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gxfpvdclh.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gpgesxtvd.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gbskkmzlt.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gjnmuksmm.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gtostqspi.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gsmrhalvu.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gkbrngfre.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gwusrfmth.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gevymauzv.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gkjxzqjpp.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/glpojwygn.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gsztkuibx.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gkcwefmhq.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gllusyavt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gyjwnbhtb.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/ghaxwfuox.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gzjuuekbm.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/guycrscyo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gawpvsyxo.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/goqhmxkhd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/ghrmfropb.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gwxupzrxb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcrhaonmz.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/giipyreoq.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gzsqfcspw.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/glcksjoji.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gkwlobvvn.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gumavzadj.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gztbxmulr.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gwejwgaoh.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gjxvdlnhx.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gpedclmqe.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gwrucoqia.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/guskkgmlm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gdmfowpvw.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gyrcbwcxq.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gibcorexl.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gqwdmgdnb.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gefzvedqt.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gdcsijfmr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gjbwdhuko.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gzmxnxpiq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gwneutqpz.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gbgicpfrx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gcuvnelcw.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/glnnmeayl.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gqowestiz.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gcpphmurk.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gtzzzzgho.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gqnlwpvva.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/getzepowh.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gbeahpvcp.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gnvywwebv.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/ghjuadvbp.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gpzmlrldb.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gnashltgq.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gfmmrnunl.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/ggvvzgkrf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gxhberdqx.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gliwzygya.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gtctrizrv.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/glnsripzn.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/ggjsjjozg.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gwkeryatl.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gwfkeokyq.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gtzlxyntx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/ghuwztwvp.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/glvezjori.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gdmkixqzp.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/geixkzkwc.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gjqbbizml.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gsxhskwri.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gshlvtuwa.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gxffemhfz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gytzryxud.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gqvzqiyyl.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gfhcxhcbs.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gfvjmteyl.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/geejlxmsb.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gremjfxyn.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gcaoreuzi.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gxjxvbaxw.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gynxcypwa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gfyhrmmpi.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gcuauwesq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gmrrqfuec.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gkloqdhgh.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gdtsrxmxs.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gqxqsfjsv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gdhplzqfa.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gmiugpzod.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gxrprleoc.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gzazqzdgl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gaxyfptyv.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gpirchyhj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/ghryhsmfx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geckgrnqc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gqczjpqxj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghcxpzjbn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gkpukxdfx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/glnwyrtgh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/geqgzyhqo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gndmbcbjl.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gtvvvbmqu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gjmdzomak.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gwukcwcqn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gdzdvdoaw.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gxbangond.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gzecbwcvw.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/grryjogsk.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gsabepzey.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gwryvhald.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gposbmaff.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gjkrhyfoi.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gfigyrviz.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gvmbxvjfb.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gauedjctq.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gagahugnm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gkfzaeyoz.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gywojqvek.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gplonqibb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/glieyufjq.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gfwmcgmkt.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gkqlapnch.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gddhhxxra.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gyjlysjzq.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gtjvgyzrg.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gateknkbb.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gsdekhdwo.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gkujmgohy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/geofujmgn.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gayygbviw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gnzfdyfnc.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/ghmsnobvp.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gajbijbkp.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/grrromupb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gpvhaldcl.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gsuqxqosl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gvyxntlgj.sHtML


<!-- 参考信息 -->