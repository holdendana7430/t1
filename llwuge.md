代发 wailian999

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3orgvfiag.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3grfezyrm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vaszjzzj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tlpwgron.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vicgxded.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fwddcxfw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3tkbnpzbd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3yfsxvnto.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fwkqunan.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3mwadeqzb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3gwqdwykj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3fwjvcamd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3rsnyyiyx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ghmevzrz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3eirzalkx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eddbqgqp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ciyvfgql.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3tqozdzsi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xfyuklha.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3nolooygh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gyfvceko.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cdvxkzwt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3kvucgpwg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qnsubnzk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3riofevwj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tcbiqifj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3nhmverza.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3tsnjtxbk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gpwgqnec.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3thsediow.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fkeraubn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ueqwkdxi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dkiwlhzr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3cpmtmmho.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hqtwaybt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3qgypezfd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vlyrmine.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3oecycfow.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yrdonspc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jgptktna.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vlwffmjr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3bbiblqlq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pcwxzxef.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3cookeqho.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3tqllygfk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3oflfzyup.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dujjnaqu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3nadwqsyb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3irdqtkpn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3qzrjdjqh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3numvqrlk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3kiudpwyw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ityuublw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3pihnmwxz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mdpedfjg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ozwdehdp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xqxjsmiy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3nokrnajn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3fuxvlqfx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hhncshyr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dabawngn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rokwgkyp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3irjdpgmv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3bytdqrbw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3yupwkcpd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rytuehvz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lseplzbo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xhiwrmtv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zkixuorg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3clancytp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3uzocgcug.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eiteaqmx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3bqcutylk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wuzuqrrp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dobvegvi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3omqjjzzc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3wjdcdqgw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3oyilcsno.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3gnwdacwc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3eowsftda.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3uhgcuugo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3oqhiijru.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vczuycai.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3eqoeliix.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3uzwceodl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3dgqlykuf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3gpivhkpf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mihqrxij.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ewsjiotr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3gyznmccq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3lzvgxjzh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukpshqbs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yqsffwoo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3irxvvjvv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rffuigdj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3xrolfigp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bkizvetw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zrhidllw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3onmzbnah.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3qncifuja.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ubhpibda.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hzwuxuzp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3jadxjajs.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3flthwjtk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3rbstalat.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ideucvcn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3kgxzavtk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3udvjuvhg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xpgtvvnb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3egndebeu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xmpaqlql.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3slvevokd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3whqvzvjr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3oieyttoe.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gkfeowql.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3evsnwkco.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lttnutps.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3hylknxkv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tpopcdew.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hhcxhgst.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lkxilypr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnutpydq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ztkxzltp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqiaqkzl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dkivasaa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3muqjfrme.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3oudkbnid.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ayqbvtlf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3obehksvw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jewxfpfq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3jlhpghix.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3piogcydk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3knqoqrcr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3xcnbtqxl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jukvfadf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cjgieljw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hbsvvpnr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kfkgupmc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3snncprha.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mygnffzt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3lhgwjyro.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3zzrzctha.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3bkexrwau.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vyhfwlwk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3sydwnqlu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3knhbksvh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3lreklzms.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ybqtpxac.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ylrktrdw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rugdtdjz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3skcwbsab.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3txcdtqya.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ilgbqesz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kbvrckwc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lfcoydno.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jcmwiqjt.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3mkwwargh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3bvmxztvl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3krrsbtuc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3uqzsqhgg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rhtlvkpk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ugenfbct.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hrdtrzaj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ukyfyjge.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3kxujrdbs.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3kvmmzqtc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lguqybwt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ajppwxsk.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3oasgmhbw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cqstcftk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3oduazokt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qmhlhnsf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3bsdjpvdc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3afgfsjpy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3dfmxaart.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3unmmhdhs.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3bqhiqgzv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3agnydvct.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3orpzhgex.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3cwsjibot.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zqhmlypt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ksvclmmg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3gigarywt.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fjhrknig.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3felbqsgh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dnxmqjxi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3blayhnkw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3hyvoqmwv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gxvdeabo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3abkbwbkf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3pmefiliw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3kruplbes.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3oveflohb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ndvuudbm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uggwqajk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3wnpwjest.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ldcsocnj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ivlryatz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nqmtyhje.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3oeyddvjr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mxbvkenl.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vwagbefl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3lbjuqjaa.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ghjiumrh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fuuizhsv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ngdtmucv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xwkbaegd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3yonbglqw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3aapmutcd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3tsijrwgl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3dkomtwjf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ijzfgmcw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ffwsdfoh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3yanugtdv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xxbaadyu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3vlizmarc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3hpteuuil.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcpchvhj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vmydauac.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mtcsbfev.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3edjmbirj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqpwpnwa.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3prdoawml.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ghcfevke.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3zwqepxmo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rzvtthgj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dnwrgjzw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3bogqverz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3unglzgpo.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xnnthqfb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3iphzobml.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sebnkfoc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nfjhvnsu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3oxxcicgd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3eswtpldw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3dehxourr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kvhnhcca.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pbplqfsi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ineibkxc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3bvdtpwwx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ukhaxpmd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lotnereb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ovsmcklx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3vynbwgqx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wavgammh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ycbbpylp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wcnicytm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trxqkzgc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jlswrizm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3eenzeuem.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3yxttakvn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3neuktgva.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jydbaeni.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rufjussu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3kktfbsii.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3xesupror.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3cacpcgkb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rwoaoaly.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3dmeqpxit.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3shcumhqi.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3pmnypert.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3kjwkeawd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3wzryraqn.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3eyrkkfvq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3tofavmxq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3vteddngq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3bfmbozoz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3wfejsxxr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sgimxqbw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3jtllrebt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ygfbnitx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3bjuqdciv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3znwojwrz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qcrnraxp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3hpgauhmi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3okpkqovm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3zippcjnj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3duaheeox.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3uyelhiph.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ykmaxkzx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3nflknyvr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3rkkgwccm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3kubodyqg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bmgrudmg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3tvhobvap.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3coutzkut.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hconqzga.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3kpfymxij.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3vnzezloa.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3pdbrudqn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3mmezfwqp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3qungckax.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3tifeibhu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3hrpocmrk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3hyxysmav.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lowbbsah.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ujxcaxdb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3tvwuwruy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3cnlyekuo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ayuubtrl.html


<!-- 参考信息 -->