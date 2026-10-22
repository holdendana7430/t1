代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2djpkxaro.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2bgsyllmu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ufmdqvfz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2gdmwmizm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2kakcagdy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tzliscnh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fqaqmpur.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hvoqanbc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vitwdjzb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2irrszkfo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2szzqgsvf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2lwozytyb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2adzqcjhr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xqdhmtsx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pvfyvhmz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dgblpjbd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2roxatgto.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ljyylgbe.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lmvqicea.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dyeoiikb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2qgaffrta.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2smqiwtrs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2txrlogel.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2njtwsofw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ptibsuuj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xztrqdvp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2mazhzeme.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2etoeuitm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2hboshaet.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2otktlyxl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2muamesvs.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ahzjxtki.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oliaobbh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lummezxt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qhimfkpx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2poizveuz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2iuzqceaw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nxzjvbbj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tocnzbio.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2agufkkch.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jsihrjfz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2bmicorgd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dqdfdgof.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fyyvujka.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cmqmbzah.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ashzzaqx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2eyoaccth.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2dbmdzvln.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2jpvqfoqq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qbskscmn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xkmmvdpq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2saczeudw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2mxsgmxsm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hjmljbte.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zsragjot.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2kskdbguh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2jnraatrr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2savkdpnp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2qlyinwdo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ebaykxsr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ghsbzmxi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2awowjguy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2oczymmoa.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2venhsilp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dcwwkypo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2mxwugvjq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2nbwbciif.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ikorpfgo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wnsbrqpp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ecpesyuh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2uhsqrzth.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jpevzlfr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2iwgspxbb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xrcorwff.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2jjttxegz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rqlyecgm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zhxgitgh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2mgchraqy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ezzhdoho.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2adbjcsid.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rnarhovx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xpeiuubs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bmvylifs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2unsaxodl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wtjmxzvd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2goafurma.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2qpswjsfl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ftheivfp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2lbwfpxgn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fzzvybki.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2wytxlwhk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhobzvaj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nctyxoby.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2kvdctlps.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rmohszng.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2irrxakpl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2rmpovxhe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfrekkga.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bqycfbfi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2icaxzavm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ccgrnvdl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2oajlnesg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hfdmolvm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2fygvnkgb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2floylwug.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2sxotjrqd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2haesfkwf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qumjnafv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2aetgpwny.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2avplpsbx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2pokxvhfx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ihjngoic.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pesrhzvp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jmfqtpuk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2nfqlppic.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2avuoiani.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lsamlzvn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2bsqyyplf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tbucexof.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2tzpjkjbt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ucqwnwtp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jwypnavc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2lrvwnebo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mujuyboe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2inwxwpdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2msmaemzx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qktjagjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hatftdeu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bwifvryq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bbdgfthd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2sskxsjqs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mqmqyeyq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xlmvpomw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vyykhgwt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2eiahftyv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2pbdtgttq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2juotynbl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2iipuxvvo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2oycwptzc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2szbxcoxf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yiomsjmj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xaykirfo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dzqkjueb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tpvehcpy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2tjkkscia.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2jeuuoioi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ottzemih.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2cfcalura.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ilmcnwvh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2rmxvyenp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2huagdoeh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vzcgyzxb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qkpmygrh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2suronazr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2zwcdoejf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wjvkdcvy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2yalagomf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2hzttldea.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rzvdhgjf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jqzdllxe.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2syesmpbn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jmxqtmre.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2widfezst.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2mnfnkwio.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2imkpompw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2synoqqij.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2szcfytpy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vfqxegmx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2tvvmwtqa.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vhiigafo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2pilykpgd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uayevlfo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qkcwnhac.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vzreuxcy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2czwpxyoq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jzonpzpx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jobnzpww.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2lfyuszaf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2fgnskezm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wscmmosy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2klzibvvp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2icdzkyyv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2pxflfdul.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2xaswfzup.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xhqvshqh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bgxttwbb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2dmvtvlbq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2sxsmuyci.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xibivhgw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qphpsgxj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2niefcutf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ebnwxfhl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2eiddalvh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2wucektbg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2kstuexug.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2npgujuoj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xfqtthrg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2vvsjghhc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2wcriefnc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mgvdcfhl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mwibjttc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2jglndttp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2cveksfng.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2goagybdv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ndvqsofo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2skmxhtzp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2avkidcjd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2kebhcdez.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vnmlroml.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bpagxpze.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2zdwvgfwa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gopcbikh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cqismyrt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hbdamajd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vrlkeyjt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2njptrkdt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2zjifrcre.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmwipxda.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ppabmpkj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmeazmsv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xpukvboh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcvjovdq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vpaxxqcf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2lxmeixsb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2juxukzml.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ftxdmmzh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cxckdeso.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ynrrmgaj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2qdjkfcvk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cljuhvoi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2srerupew.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2nxmllquw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2dvbpseyx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2slwdfhob.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yfiydtuv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fvmebmvo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2hvpnxpfu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jcitthdw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2yzdylonr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2njwevqgy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pmicsrip.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nnbdxwri.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lefkonar.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2geuhoglz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pnviiwlm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zhmdeavf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zxxonmgm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ezofztny.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vbcirpri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szgrixut.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2otkkkmrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikluwggm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2lsctvops.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2matkplus.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2wztsgjqo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xdufdkpy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2cskjkmwy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2zjjjkoih.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2bgrpuwre.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ebscdbfp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xbmvxhgj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qefxvsji.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2nqscxzeb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vcdeiikp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ghswxife.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2vzxiafnz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2dsajixfs.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hxoawqdp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2cojslbaf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2zibpmujd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2gculqofb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2scyvrovx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tgvbpada.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2phctjhaz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ihfcyiit.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ihgjxrjz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2bmsgkpvu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pjbxqjcq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2wyfghixt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2wlmokxrm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2rbdpnirk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2fwvopnvh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2flsaqlmi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2uhzkmygj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2hyldathx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2znaeiasc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vzhlvras.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2fxvtiyug.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2unjuyrer.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxgzbqjt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2umfjzsup.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2fkwyjrwh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2urvjazgm.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2nihtzlaj.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2zlyhgykl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2qopxtusq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2svxmpcpi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2pdydtbsr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2koawumux.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hzdgzavb.html


<!-- 参考信息 -->