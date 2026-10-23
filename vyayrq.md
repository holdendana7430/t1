代发 wailian999

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3cksfieqw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wnxlowkk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3wrjqmuun.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3qwmvxvvz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fhrrcncv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3coebvghx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ywbxranu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3sctzmvnu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3pybscebm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jgfzbtky.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3egllcugy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3srtksnzh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3kzqalqan.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rxvqslbn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mhuinruf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xfwayvle.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yaliwwjz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3rizvytkh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3yxardhxs.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3muvdvgrg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vxjitqna.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3akeqctkv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cskvusqo.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3mdylyoqp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jstbdhci.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vqcbhdbz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rqsqvrok.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hnqxxkio.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3rxfcumtr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bjyadplq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ngraohma.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hkfjbuyr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tdfafpty.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hwvpdoxp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3gpqpstqq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yrxxjgrg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3dfemfugc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3pgqtffck.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3rkgclbmw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3rwssserb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dlacneet.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fflattpg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nihpmfci.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3vwqlxwdc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qmoycrrc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3xamzndqi.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3whoxaqsv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3xqytnybk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fevpiact.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3wdnzaqkw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3wnznsjzh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3jjytxpom.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3pnflfofd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yumlevkk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zyitbxjt.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xaolncbf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3niynjqer.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuqfofry.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3luowzxyx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3mtxdxbqa.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3igaxsvzi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xfismrbu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3smsbguck.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3nmbzctlv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3htfwibgx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rcoqfkoz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ymlaibqq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3npyjphzi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hyphhsxh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uujncexl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3dznlnltd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bfglayvt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3dbxwdlup.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rgamunsb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3mfvfzktk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xkdgnmwh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qqasvwxd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3fummtnrg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wtprcgsy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3mgjjtdeg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3jestwqmx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3vptypjil.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3yndxsesk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ookgkqdn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hvxbthvz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3rnvjuehz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vqihvgbl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuvzhhck.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ixoxvclw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlpvqqbm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zqyafgei.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vbitnfkv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3nomdmxav.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3mbglgxge.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3zqepatsr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3zsfzruzo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vojxbrhq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zmkcpjhl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3cagzlnet.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3htmnxlzg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpolplrw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3myhnvcui.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ogqpzobu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3faclowis.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jnqqzias.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ttzgylra.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3hrwdsova.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3kxnglkno.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3npyitahi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qgbbbouc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3hljudzpv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hfjvrwvx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3nqkbfytr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ocqntcpv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3itbfvefb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ftiwjdeh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jatxnkwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duzbgtez.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gtgutaho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxczecjh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3edmxpgyf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jmfiqzkt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3vmmmhnkz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3mejzfifg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3nnlflahe.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3cdrxorjj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ibnihnco.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jutijdwh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tdewaxog.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3sslnbnsg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zyuqlibp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qlpjvieo.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jomnffuu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ayfetodi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lqkfpnps.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bqpmqzxc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3quxcgqpn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3aqazfawl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3azdjmzcv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3fctjszhl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3tladffuh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ibodlale.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pceazube.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qxpxaoce.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pjijftdv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hgtolynb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qgrpfgcf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3azdkkjca.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rzqrcwip.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3aleralwx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fgmhafli.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qafrbcjo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3dzdsxsgc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dbeesape.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rnamauus.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ymhnryxr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3akchpkcw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3vluertkv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3mgwoxsiy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3keeoqxnb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tpqgyuqg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3emoyteis.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3jvaavvsh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3bvqgxmfx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3uwtkgaes.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3gtimvkrf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zckdwgvk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iqexxexd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gbgtuxds.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3hnrytouh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ltzhyesu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3opmgvjyk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3bgamfhne.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ykrimsfa.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3akymacrv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3rzmimnnv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3lokmsxba.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3urzthfma.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nxlhugzi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mrwlstzr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pnbdauls.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mgjvnvmi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3rnesncwg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3odghlrbn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3jabjbtaz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3imscipvb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zapvpmye.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3znwzmcxv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3skglpmab.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3mcpynqyo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3psvwbaau.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ypydmqvb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3cdafxlen.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3sxxyqzgi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rocdakez.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3cwytburp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gxsashgp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3onecyvng.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ohnrxctv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zcrgcxad.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wmslykty.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cbycroqy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xbtrkggl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wvjgysfw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ayrfugpi.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3gidsuasq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3vosqtufx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3cxkygtvy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ppvyvytt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3uhuarnax.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3lkkbhxym.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdzacvbt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xpllvhqv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3gouluwuy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ynnuznwz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3cebarkph.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uvtnzatj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fqcteikv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zyonepiu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3zbqozfsq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dzfdhwrf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ixmesnrj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zxlrvddc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nwzuhgpp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sdbcobdc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uonoemdr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3alpmqobx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pgzxjfnm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3hlnagmee.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uiiugcxn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3imxtzmpy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wnudzncu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uqsabfdt.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yqaywchw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dqxnuubt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3wvshaarl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3xzcklpox.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3pjryatfg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rdzbgiqe.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3yetyqual.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3oqjhltaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jifkywoj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jsjebxaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifjmjytb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lutmlsgb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3namhxukn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3iqxvpllj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ubgteifj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3xjnmkpwc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3wtjmknfo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3eypieztr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3eruxcaca.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3thblfxwi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rcbdfxja.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3zdsnfhvu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3tfrdzkxw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3jyqfansf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3iwxiwjbk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xqfabkqg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3frgisqpe.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3rkbdhlaf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jjzutzwm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3qvbpxtly.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bsagwvfb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3grsfoush.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nfzjrmai.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3jvhovcny.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xicmqeck.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3tyetkibm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3vcljpupc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3iyzjawka.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vxoksxsj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3lihwllzt.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zsdcecif.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3znjlhgls.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3mvzororn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ysztbrlc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3jbbaipgm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3epusoejp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3msdsnlry.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3yvpffmkv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3rzrxupjf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ujqxoypt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3czeewbyg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3nowesucg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3mdljnrsf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3gaxydpjs.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3geiekpzr.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ndvguuuz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3hrqmhrgc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wjenktxi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hjdixmjw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3rlhtovxj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3saytbizi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3klckbnke.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ilrmqfqa.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3yzmxtetx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3sddkmjsb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3bvpxsrbe.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3cenxgcqi.html


<!-- 参考信息 -->