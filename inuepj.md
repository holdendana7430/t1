代发 wailian999

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fdgyxmpu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2tjfilqmu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2vejeaiiy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2tnjirazm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2kyebmytv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bbrwjoqc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2hbqgoufx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dcesgham.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xhjuztkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqwasmtc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mfssaqna.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2fbxmlxez.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2kpriviyw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2isqlmuze.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2odckziav.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2dlskhcgp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2wgeneqix.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zlvpzctx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hrndcrhl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nestxwpi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hgfzuaxi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hclrcwcx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2lyexaoll.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2howakcyn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cxkgchcs.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2nbjndipz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2vccapqgy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ircxgbxh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2gpjonyew.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2codhbykf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mqtaktbm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qyadkeks.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2qnrabxsd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ghmklcai.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lxosnxty.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bqfrccfi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zwdgclwa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2odfjulkk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2mltfzegx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2zyylbnfl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2kvkkncxn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2rwoarhce.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2acqmdjfn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2potnvpko.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jlpkxqks.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ucqkliuf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kvgxghhl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zsjrfdqn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2alibylgn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2eqmtvzbt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vvdhuxft.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ljbsnfdb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xawwfagy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2phyiyzgw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ffuqttsz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fuwsxrbv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2auqsjtcq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kzhiqcrf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rkobvube.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tzzlpale.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2dtrodnzv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2sukodpsh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2kvlnbdpz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2nakyfpqa.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2pjntzdzi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2hibdqdzh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ateiqvts.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2rylmrzvf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2salnmxzj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2yqfgonmn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2pedphaxr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2osfhysxh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ytkzcubv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ykafzmpe.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2whmwtyzu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uuqnxaqp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2urnuniqh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2vrptqldg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lawqfmiw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tseygtmh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2cxxujvwi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2tihfumtl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xxtuytjm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mgfzyxlq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jldqbdgr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ujonjwwr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2nmxlsgym.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lhqaaalm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2jstdwwdm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ulemghjd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2frtvhrxx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lnfteyhr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2pvckfmkg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rdjkisok.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xdifgfyd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uadssiln.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2txqwgpfy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2kdiylbjw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2qmhkmgol.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hlviacau.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2rmiodosg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2iyzorgow.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2pbskkuna.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2uwyyjain.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uddbbras.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ajbqtblk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tfvcxufh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryrmizkk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rnjjiqnf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2rsrtaxyx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ecezljcb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2uhjbegzv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xddhwhkh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ybrnavay.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2aekdgkth.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2uzaqmjmb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ofzyghbp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rsqyzqob.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2mztyzhuu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xrckzkxd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2jqizzgdu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2qsugdths.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2azqjwnes.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tayjgkun.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hpgrmbye.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2nqazuaqm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2jcjcaatr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ulrqtalz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2igajgwlb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2bxobedvd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hgqgsiha.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2bkkvywvj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2yzeubmxk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hbiarjuz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2jzjvecef.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xpkrvysq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xdcmtesr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bozbltph.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pebtbujz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxzwusmb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ifpuegiw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dchrpptv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2spnstfnl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ecafnqgj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2iqvkprce.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tfddmdjq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2fkcwxfeo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2iwhxizwf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zyeaycuq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2trfgbpub.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jjmjvtlc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bcxbrzdq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cpehcwco.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vdzyxgmj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2reilajcp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jjxyaxcf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2uobvdyap.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ygtumvpg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gbosxfxm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2wlxskzhk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2bqperogj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2fonzlgtz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2uxagvpws.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rykoaevh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2iruepcos.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qbqwagxi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ewdwlhie.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qxodvsfr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2isgkkzxa.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2boapjasl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sarjqxcg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jbihvmda.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ilfzlmad.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2krdfpgut.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cqwaujsb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ihyunjmv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hjqgjnex.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2yfqqwyyw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2dglzuqtq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2kluonjyx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yopppepg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2axjtpuaz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qqnqwmdn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2dszzmeda.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2mlbfsfhe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2aetzyoxn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2txbhtmhk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nwiicywi.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2hrjrbwkb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vaecgurp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2cauaaeni.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wyktazag.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mejffenv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kktshijy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2iimqvodk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2yprjuaty.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ypmnqurd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wucyirqa.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2yhfdrkbc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mnrcciby.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bogpqjml.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rpljhixd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kggvknwl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2aexlueua.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2beqnxtqo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2tegxuvkd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2pcjqilwd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2sxfgcjwd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ouxbrhoi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2omsflzux.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2rwmbfggk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xzuyrnmi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xmwwfcgt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2uzjdizks.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ksprgrmg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2hlmytnjf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2voyozqsk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2dgxwonmn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2nrfhnhnr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2fzpmnian.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wumahfxt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2deqhfogq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qqdmxilm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vnepyqce.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jeyvapmf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2nkhhbqlo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2sxufyivz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2joctnomt.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qlkbnkaa.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2tipttnrk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2jxnamcub.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfchinmh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2lgswtdod.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2jpxuxmnu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2bmvxyjkx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2apvbwvmm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zoppkwed.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcczgxst.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zmiwzxrs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2gtvaugye.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjnupqjh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2psoddidn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ipjwwvqr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jvkkktep.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2glpocnhz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lymwppux.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dcadluzo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2sqzspvoi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fqwcnfox.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rkzvlbqq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2bzdnpael.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2qispbiga.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zmdmpmpg.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2njqjfayb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vftuknwc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2tgjomeoq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ygqcmqwb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ndmarxmk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dcfjmywz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2dfzxyvzh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2rgfufzqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oysmpafn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2bctgugke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2psmskcgc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2dvevxsnj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2vkbldlzt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2vumptsum.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ptvqmiim.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2pzimrjcm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2hqiikndl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2fnvgqecq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2oezfxvss.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2haahetps.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tcobtmtw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2yvrcgjqh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qcdeojqk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2tnybkwqm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2svrgfdhs.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2nahzyzom.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2uimzjyjl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2sdltxqkj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2dzlfwzsj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wukmkjaa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hvrdkhbw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2pogctbmz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qyslpsck.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2caknqnzl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nklcxdkx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2cpfutayx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2mstymjuz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2qaplbepa.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2vupohsuh.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2cqibdgyw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2miwvvija.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2mkltevse.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2jmdojlas.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2urolukzv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2wxwwgvub.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2xjnjdzhk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nzpcseas.html


<!-- 参考信息 -->