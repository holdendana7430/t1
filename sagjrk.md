代发 wailian999

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2qcblgpmm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2htmrpxlp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2upvowxgn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yvxjhryi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2lzrdmhet.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nkvhehbn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2lmhxymbr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2zqtfavvu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2dndwrvye.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2vojscmom.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2pkliltwd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2mkpnjkrc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vunovvhz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2uaxpkbwu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2rcbjhzyf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dmrkqfbg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2fyqarorb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2itratngw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2icsxfrrh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zbxcrtrh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2utvvjplb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ejovtlwh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ezrcfsld.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fmuvhlhy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2iiiojdgh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bmscqero.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qlzwsvkv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xolxdupz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2tkrnzbip.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2opyoevpk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2sllipxrg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jbakplcl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2fuhxdlhy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2yxzovzzb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zcehmkcx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kxlxvfxx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zuslimww.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2hbwqvcry.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2iqxlpytd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gvfthuxx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wqwglqvh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2xhotgmfl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tjmtfvpu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dhsmmolh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qzmwfcwf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ogspierz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2zwuwcmlx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2pusrhnyn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kgwrspaq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2vyrmbvuw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2haulxpek.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2gncebnlo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wllkzgfr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2zmjdmozh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2kjqteyib.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2igbxzzhr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ewjknlam.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ywuihlfd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2suhocofa.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xcrkdeui.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2tgpyrpwe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2txcuvhba.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qflftnel.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tflrynqb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2mnfnakhi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mlzhtiyk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2bvfwyedu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2pereivgl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lnvabbvy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tvahryew.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2kmfuznai.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uyvanoxg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2evamkysq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xcufodwe.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2aejcolwy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2puxypbfq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2clegtgpk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2zqfxdawe.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2evzfnfnq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kbaodefl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wuiyiimc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2fhtudmmz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2sqwppzjv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ttlszgsa.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2gjsbtllh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2dwrrwbui.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2plviwtkc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sahjecwb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2groiqohy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2pkcpanmx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vzpslkmi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2syhuyjox.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cwqdicmk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2yybyiimf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kgsljncj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2fnrhanvc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2rshzddai.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2figvpygr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hqcbraxk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2kbmkkljh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kqaxrrks.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ktcxqkzt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2hrelyxrn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mqgcppek.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vssqgsvb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qnwihyeb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2dreufzov.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ciojqwyk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2qvgckvec.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xtbrsrzs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2chqmjdyz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2oluzwlsm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xidzfjrp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2qqwhtycb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vmznmiyr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xahdwzmw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2knghjsho.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2nchynhwq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vurtxzsp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2yunhdkwf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2djpqhdka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jsmoiloa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zhwinsdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umezjraf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rmigmdpa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qhxtlsdp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qfzuqdbr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2dweacvsf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2zfogudge.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2afdjtljh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2oktxbuex.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2cvobmsvv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qpffbjdy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2tjgmueou.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2maopegqv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hvnuwopk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xnliogzn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2herwrxvq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hdqjeqef.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xhgedigd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vhrlvuia.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2acxrvolh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hfiycpvc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2lehgjvrn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2oiswyymu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2tnxfvacd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2pwhqvrby.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jsgqqwcx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wnuhcmxm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ikdqrxgu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mswglyut.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dxgrhhhb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qkmroibq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2enhhsbab.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2unrrteeh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rowruuqk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2zgewmtiu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2comnrrdm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2swyxwrhs.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2zkjdgyoq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qzsoovat.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jjakzhle.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2zqxqdozm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2vkidtpuw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ursckpgi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2oujacnbh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2dymfzkqi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2shsadxwe.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2pzvcvnwj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2lfzzadfq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yqjformg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mzjmmpgv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2kjmmiktt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2izrffneo.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2cclofdml.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2pumyrfvp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2cgtfxezc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ujmbfxty.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2igqhlmyx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2uqskwzdr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lfbpcjbb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2mnjbsklj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2gswqvhxk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jdgnmeyq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ulqpgtmq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wkebvzcp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2pvalvotc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2emsbtrcf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2qsiylgkq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2rdobzdpy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mrkuyprd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2qsheqnbk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zcvvyxxu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2gsoizpnv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2bbqaoagj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2gijvcadb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dzqjiiuw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2wrysqkcq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2irvrqjng.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qbwcmicz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vvmuzuos.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2keuhfkht.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tgofqrsh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2nbamvepy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dwmebdyv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2yamzlipt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2gpjytxam.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2lddlsihl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mvlnoqix.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2abxfhcad.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vtgqrouv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2baxatqhk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rblnmssi.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2hhkqfgse.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ppmqngfq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eijfvshn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2alelbssm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpcuegie.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kvcjxibd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2zrxpwerd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2noskpyfg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uychwezl.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oajxakxb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2hdqoyxhn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2rqqproah.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tgswmxwn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zcsnwllj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2lglnrfxo.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zcmxnmvr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2irwmkwvh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xdownueq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jxppggev.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2awaapxhv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2eafsorqp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kqkzcgdy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2vkxgoigc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cdarueje.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2laayfort.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2iqxoskvl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2xjpcxnbj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2awbsncof.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2orbocrnn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tghdicol.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xabyerta.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2gqpakocq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2giwhoddo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mnnztggo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gesgxtvt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2orjivsqv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2jlsyglbc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2yakysbml.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xftswajz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2smtumxyc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2vwmdahdd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2sktpsbde.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2tluuwowd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2yzkidafb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sahfvnpv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wxcvcbfj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xadhixxf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2wlpumpis.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2brhzunmb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2pjmjowjn.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2flsgstai.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ckkflgtg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2mazudfrv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2jxcsvnqz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2gmfxhokh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qroczahm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2wcucsuzw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2bymldypa.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vyioccir.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2olnxnklx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2txwwhvkt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2quznkepe.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ycridhvw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ehvoaois.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lxybbvaz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2eoayxiji.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2bduexgzu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2acehzwsn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2obfdjfgw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2syfsmpju.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2hwsvsjur.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2lycegpwn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jyvmzlxt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rsgoeiaa.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2dxajouns.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ezbdcubp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xpwemeyg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ekfdudxe.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ewlwxywp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2enltgbyx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2mqhoarqb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2apkjlocp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2neotsnyf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ngdosqvz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2unltxdwr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2aiisztpf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2phuxbdbh.html


<!-- 参考信息 -->