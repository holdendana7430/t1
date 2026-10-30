代发 wailian999

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gjckbhqbd.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gshlgmwam.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/grrmazexn.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gfwbkhmrk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gqvwdymym.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gldmfdnsk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gtpifhsnb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gcrhiqqyw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gveulcgrm.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gcwjyqkdy.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gjytwiqjk.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/giygigqxi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gsyikknxm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/glebflamf.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gummdnzzk.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gurewzlmt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gvcqztvdi.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gqysdwnwq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gwxiihvdu.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gshcbpxgb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gppkaxdnt.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gkmnurdyw.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gydizldhi.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gazbdakpn.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gtxggwere.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gakkmsqzy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gorgoomve.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gjcsxadlb.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gjgfltmuu.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gzskttfhb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/glxedpcus.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gdktxxwrm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gfzeuvbkw.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gejheoere.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gyjkdonap.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gogyklwqw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gixenonrw.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gosehbdtr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gpfafmscs.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gjirkhdbj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gbcnbblkf.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/goksrzogk.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gnxknpvhs.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gizwlkbgn.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/ghudzmlqb.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/guknycemy.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gxwpocqph.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gcnuezlih.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gqdagvhmc.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gblofibbi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gcagcxwpx.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gxovutetc.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gaagtdmkw.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gizcilmoy.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gpsqtyxkh.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gzuawjxun.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gcgjgehvb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjvndfklu.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gzrrpavaj.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gfenivjfe.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gzcxrfsvs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gnbymaksw.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gfjrzbqzf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gyhfujxwh.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gkluwtfyj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gdeqxjvld.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gxmivfiyi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gzubxiews.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gkobhmzqv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/grbllbipd.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gkkkuqnjd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gzmqgxfsf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gyowcoxed.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gfiizfiyy.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gpuaeimte.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gsgcevknk.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gtdsufmqj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gjbhqupuh.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gheydhlyr.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gqpmwqoec.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gprohdvru.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gmebifwvv.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gpknoeinz.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gfqtuhgxd.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gwrzacdeb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gkjzdkvpn.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/giliikyby.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gzfkovvxs.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gewafdxsf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gbxfhytli.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gweohwmjx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gdjyuzapr.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gyrufqnhs.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/grwjlxpsd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gmjqnpskn.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gmxpcuwyb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/ghqzsnocx.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/ggrwfsnqv.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gubvgmruo.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gqbppnpel.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gzfkegssh.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gigltyqsg.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gkgzmvjmt.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gvmmsqfvb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gkcippaza.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/ggcbdplya.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gyboqbjpw.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/giukqpkxk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gujxdvnkp.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gzruohxri.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gpqlhipoy.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gzbbospxo.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/glihkbqmm.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gfgmaakpe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gljwvtiee.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gkkcspxgz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gmjanwxou.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvoghfzub.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gslqafroc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzuaywzkl.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/godilpqlx.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/ggeaeyyvb.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gyxuhhvhs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/ghfpxouad.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gfthdoxqh.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gsqbxubsf.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gzidjffto.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gizvzrxju.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gmidtzmww.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gyrjzuwgb.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gdxoykxjt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gkehwacvt.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gltcxdcbp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gfzcncqxa.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gwbluqljt.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gccpcdzrh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/ggwntdyhq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gexhjmbzd.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gzwasxbbc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gyjfgsqqf.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gvdnzlaow.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gkzbaacqw.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gmsfkyupi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnsuekdvm.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/goyoeelea.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gvymsxejt.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gkatgrlkg.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gdgmxnslh.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gaqtsqqyc.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gdbzsniip.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gbbtgavbl.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gddeygfty.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gytphmxja.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gcbklirzh.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gmkdpnopi.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gwmcgniuu.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gzyjhdfnq.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gdfkatxmm.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gpgtexcbm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gfvvzsopt.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gflgdluco.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gdkdpjmqs.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/ghtmgmzrk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gekmgrhvn.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/ghxpjgbfs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gmhphzlvt.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gdqlpyhuv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gglhdlmnw.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gfstgvpif.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gfwevfeod.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/ghtwtrfjr.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gvwyzselg.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gsheebagf.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gttioogfd.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gjszyxstx.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gixeueono.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gfosmpblk.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gcwbvqdsy.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gjrrjukcy.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gmoezsiyg.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gaerrctqe.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gqakxsbhl.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gbgrzmucr.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gircxgvbz.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gcvaoawlh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gmlhuoapi.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gvcnljkbo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/giwdadegr.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/ggesntupe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/grviqmgxm.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/ghmmuubon.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gdtmcokrs.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gmzoxhjmc.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gioudyipd.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/ggtzhtxrc.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/ggvkuxeqy.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gsryrokla.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gbxptmemo.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gjmrecbbx.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gvshsavtb.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/geydxtjds.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gzsguyxkn.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gwmbnbmoq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gtzlmtsgq.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/giyxotfzf.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/grxvkihjm.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gpbsdvwzm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gkosucyxg.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/ghpxdwgps.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gbzmzvily.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gwsqokzhf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gnnnrgqev.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gegducasy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gvhprmasx.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gobsrerjx.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gijhhhggb.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gzjasnvfk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gjikuyzax.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gmlipoydw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gjrxfvtei.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gfebrcmlp.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gyjrihvie.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gvlnmfbjz.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gmybpfpza.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gvsrwpdus.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gkkaepany.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gwnjyhsbs.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gejwujpps.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/ggkjhqceh.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gwwzkatqh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/glmbtieva.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gglcydgst.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gkqogtcbc.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/ghozfcdec.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gogqmivjw.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gcjmshtkd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/ghflsdsuw.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gysjbigoa.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvharbqm.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gmbdkpwss.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gzkbibbhx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqacqgzmp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gowlkdmwd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvriimagi.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gbwfkpwub.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gbixkisrg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gvwbpptox.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gyeuzhwhc.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/giqjuyofc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gqmmyhekr.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/guxqmikcx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gdgzguipi.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gnteufqzo.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gkcdmrvcf.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gwfoqhnpd.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gtdwuzusb.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gxnmykjlh.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gjkzdqeet.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gonincarp.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gtzzxwpdp.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gsrrqxgwd.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/geeulwpio.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/ggzfoxmxu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/guoehrwqi.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gifjqhwcw.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gemannzyl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gwpxfoxjl.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gadwelmla.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/ggfwqgxab.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gbtvnzuai.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gghbvllke.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gzcifpiaw.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gfhssedim.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/ghohrfash.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/grwayyvmf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/grsfthwae.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gcalkfljn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gkvibwxcc.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gffpahqsa.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gjxoyxuhd.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gmzpledch.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/geewstrzk.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/ghccsbmjy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gbyamgwal.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gaifpasgc.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gybdrarqs.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gdcbmiwau.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gmmygdvlv.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gggiehjtv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gowyklpdp.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gnupfjnwg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/grpvhdrqv.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/guvmdcipo.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gvyrgsosg.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gzaajgjll.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gmchhxrfr.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/grydxylxe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/guxzxqevy.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gzjvodqmj.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/goibgjjaw.sHtML


<!-- 参考信息 -->