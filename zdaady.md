代发 wailian999

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3tangstwz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wzpxgjfh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3pqzxtzhm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rzkbyxpz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3wcrfrsbv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3djhpzaur.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ttxrxgkw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3wkzunydz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3litzijnd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gixjyyld.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mrfaryqv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sbijmyho.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3yvxdcbma.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3atwvmsrt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rqtqfptz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ldeicryi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tbqydbbx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3peqjyqlh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zlqcrdow.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3nkbzxfkk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jlponqjw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3bpoosgrl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3piliuaej.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hfkomojq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hnjcwlhv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cnwwbfrz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ongqskrk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3yxasxcqb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3yztldhor.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3psoncqkq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rnqbwhng.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3tmwhcxpr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bylmjtzb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3woupvtof.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3esdvagqq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vuyimezo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3qhvjoztr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3alzegwsn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uvanqypz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3quqoyath.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wzagxoqg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3odwehjnr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3cyggkipg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3mihrhmsd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3leolisuf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3urwdxktr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rkiizyeb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3wkvrmcee.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wlgtaeam.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3wswcnonm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3uqrmrfgq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xvcphrtq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3bbmjerwf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3phuioczo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dglwikhe.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yenqlthr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ozemszwr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulwevbnk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3niwbuuis.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3mynmvpwy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hjrvuqgq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dcrfmsyu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3tbpwsrcb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3tbejywuv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3lqilgcfe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dakeszxw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3inomonwe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3egquvzoy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3kfurtfyk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3dyapjgck.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3osakyeaa.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mpmkenwk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kzafzphx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3menasaya.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xjtxgmbm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ogwxscue.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3vgfxowab.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3cnvpdfpt.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tgwmjeyi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3iqlsrsuy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3fkyepuze.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qyzcdkeq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3tygidefw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3khfrdexy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gpkadtis.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3azfrjbiq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3lplnkiad.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbzlwgkd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pnhuorfn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssntbitb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iuobhvsb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ygrkxbgb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3kadpcmmd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fnegxujj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3kuvpvsmz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3qqoglrmp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3thszmaca.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3etdgvlfa.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3zcqbhzdj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3dhsbtegx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3rnpfbrzb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3tcblyiyo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3uwwcvcpt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kjvcrgqd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3twifkxzi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ujuzyhgk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3dqwttelj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vvvkjcrm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3regarwvj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3szzqhoap.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gzidqxra.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3kprlalgv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vcnoigib.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3yptyutby.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3croefcax.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ayiekiru.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3kcajrfes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqejvutl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ijkxdrca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3daatnfjw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ghhkueic.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gadkqepo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ejhejzve.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3agolgtcs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wvibfzad.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gbtbeymy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3jzmmvtpq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3duxpcqdh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vyprmzpm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3lyexebqn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gpdgyvxb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3myukgqlx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ybmwhazy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yfvtikhw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uiwljizk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bccszfua.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3izfzcfzn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3bnxfetpv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kqpgqbtp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3egbzozdd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3poogrxgp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3onxnnyda.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3qfimmkus.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oijcikah.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rmcheugf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oksolmza.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cylirlot.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fzudwoyb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ewqboayq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3etfvlsfn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eqyqweuj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nupknjho.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qoiwsiat.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ijjarrlr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uovdcqho.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3tgcktfyx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hjieljvf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ocyszpjh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3unrssdbh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rhoxhiak.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vqidosoo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zhgpwtff.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qivdhuxc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sptljptb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dqybspbn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nkeqpeij.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cmyhynza.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pskfaust.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3gcpocply.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3hmizcmof.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ktgekhif.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3opmsfqgu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ztxilgyg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qzrvdrvc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bvukadjl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3huhiqmdg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3sprafkme.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3qzcguewl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3kutgybnp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3louwtegk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rzrtaviu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3epkmrgnv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zhcedmgf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3shhgddff.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zvjpuifg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3brtentne.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rlrdopem.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xyjvxuve.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ayifnlws.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ljloejqz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3nbxoxarj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3nyyhdloa.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cetjiscl.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ahyynnoj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ekycopyu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3acibfyah.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3imzlssoc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3omimddki.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3tzvhxftp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3kqecrgfw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tpgnwsiq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nnonespc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rytxbdgl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lxoyssec.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ydywezpq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3rctdedti.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ebsnreyc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aryshkik.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kyecdngf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3esiyvudh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3lbubvpvd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmwqiepl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3lrtnlany.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dmwsrtnl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3noeerlcl.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3zczsjopc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xmliajdq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nedhtuwb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fobhsjke.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3zmnyzrap.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3kwrszjsq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ybzfqwio.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mxniyvpd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3iwmbpthu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3giuxmxmq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3edfwtkgb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pykqcqky.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3elwjadvl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tomswjks.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3isnvuzzb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjfqamaw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3pbnqeshu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3youuabix.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gerkbjjo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3yyqdmxdk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3uenmpnvx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qyjlmixb.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3izfcmzpz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3sgxuytsb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3wsrpivvw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xklbkdpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htxxsuar.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xyoytpnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3veiftvms.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3uwtybowl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3pswthxbs.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3xsshxzxk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kvdaeggl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3rdjlkhat.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3pfbtawns.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wboydmul.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3sixpuwbo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3huvecpdn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zybmyflz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3xochafxg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mixrgiro.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3tgvnllsf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3jehxxysk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ixlozxrm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3kbjfzreq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3aubupjkk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3iacrmzks.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3saoiqvdf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3nxsvcnmf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3zetxdagu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nqytvjxh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3lygzqwvz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3fgukuicw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3wvkfemfa.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3yfvhxwvs.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ngfvkbdp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3msuhqfrj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3bkvxjyks.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3pgxkxwbq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3vgvvwnyv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3stujkfhc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xvdgshev.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3fvvhrljw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3cuoiohjl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3nrbgdpry.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3nipquuse.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3xydsatab.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ycywzdqu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3llozbyvu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hlqcmmrx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3eggcgvdc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3rkflnhre.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qhowjigd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3laztkoaa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3qotspurz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ktsdnzrp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jauuvgld.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3vbtwckop.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3jqxnpkpt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3nmakrjgm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3vsrjxamv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3aueabbtq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3tigbqzcc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ninsnzye.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3mpttheby.html


<!-- 参考信息 -->