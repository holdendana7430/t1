代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gwbapnhu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ourcrlun.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uzrtekmf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2acemmwpb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2trghdwwp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2supqvbsy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zsapopqw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2eswjfiki.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2miyypdkl.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2dbmphbib.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ltawvcby.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2omoeuxjs.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2yymjguzr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pcppcdab.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rakantcm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2woupkfbv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ljprmbsn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2pnxcvfru.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qvhdouvl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jpeqmqvj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dpixtatb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2imkoqkvp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bntqroej.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tgzmbfun.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2xkmzfntx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2gwsypbfq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tjsvkufv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2pgvphnxa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2kjnfostv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cyxyrruq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xtpujfvp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wpbvmybl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vlkauqbg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ilppbwnu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bjbgivhc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2vxekzogk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ppivhpej.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2umxmotrw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2dmodesqj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2vkxkvvqb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ofisepqb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fksucvnf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2eyazqevu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2syufyogy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2etqciayn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2rnplboxn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kwvditmc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2iegzsbsm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2jopknacy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2flymrsxu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ewyvcuxf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnwcxpev.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vqfmtgki.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ahjdjwbf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2tqiczzez.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gebhazxg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2yugmafva.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hybltoqq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vrramoxg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rvgyhmzg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2iqdlfdsr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2slmaemjv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2jceikupo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2soeebrwv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2pqixdglm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2mgpvbabv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2mnncyfki.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ibmvpbwn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2sscyizgg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nqyqyvcx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2eeazurus.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gylvuvll.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uiowwitu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2htoymumm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2glhiarnq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2asdgxzyp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2bssqumyf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2hbqoszsw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jnlbybhv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2lqxnjnji.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2cikhxwlm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2yaeezplz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2zwdsyxpg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vbmywtzq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bxhrardh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mqyaqxxm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2tntflahy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mgjoyydf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2uwxjagpk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2oexbgwuo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2asecosuq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tmrtaoie.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hzvphxtk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bbhpfkht.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2kjsjdybp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2cdojmbhr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ufnbjntt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2dtqxjfmm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2wkrhkdzh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ocyvorxw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xkwmjdtl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2himowcnp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2iefdmvcn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mkkucjww.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2eunzznwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eddugrnp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jpllxqvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsllvdgf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wdpdemjr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uxizkngt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2etvybaza.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2eufkowio.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2qadsuyzu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2njcfadrw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2yznmhheq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2usupfmjf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gtirlxzh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ceyqavmz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zsjtbhwh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tqrrftyx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vfqjdobs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2svnbsdso.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yxsovans.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tzgclxhk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2cnkifzxu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2warmnuqp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2rmwqcedi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jkiiqech.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2sfwoagxa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2htcsvntg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2hsdntxjy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewicnnfh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ioaudkub.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jbyqyplj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vstiplsm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ztoynthf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2itpsvclg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2axitjjdi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ulghztoq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fxlixxoi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2pcazrfyk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jhgozrwh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eaeqojtv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2fhilnuns.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yhtaxlss.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ssfwjlsm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2syuwfekz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2kzukrfuf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2auoiumas.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2gbdtalzy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qwygoqrv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2wudocgqb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lezkiigd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2apzvxvvk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2lvuxncfc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jyxutdtg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2dcjtsxic.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vymwelxi.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2frrpyvlw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tyzmcghp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2krlsetqk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2nqhvaqnr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2fzrkatde.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2iujkytaw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cxszhvni.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ojfjwahl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jyxzorcw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2hndxhyao.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zbbtcowp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qgijwqzr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2unzcwzcx.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ecmokenc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2czhcncwx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2uqdlxuop.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2eqzjiagc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2xqkphegm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2urjdhsgp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wnmrcphz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lxvvjmdn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2dttzogke.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2afvwhtrk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2jopxwosf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ywpvrlfv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2jtwhyast.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fnfxwkrr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nadjjfui.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2qvivzojw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2zperdnpm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dxenfbhu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jzqgccrp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2skvrughc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2xkelsyhc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2awtcdgvp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mlgvvvny.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cgcyidfw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbvkqeil.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ssdmjdtp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ztmsptdx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2xuowblsr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2gmqvkapu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2siszdcjo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdrnwiqk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dzjwlxoa.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wkkftqsa.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pkfulkyz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hgxhswsq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fzeyaxhk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2fypfpkvu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mxmmwvda.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2baqnbxmy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yreggoxj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bzcsobbd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2zbwhwuuj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rcwqpgbn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bpukrknv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2euvtgjff.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2mqgdinuf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vhoqypky.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nykrmnhm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2npoornnh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nlxtjewa.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dvyhfted.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2kgsdbsim.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2hhnmuluy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2kirijkiw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2sjbpoxwq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zyaomvgy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2fcxsghne.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2tfsxvzni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsfojmyz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lpbudjww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2teajlhte.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vbgahuon.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2duwcmrak.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2olqyttha.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mszywgzb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2eikbfjyk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hnbpsbqq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2gnusdaif.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ppsvcchq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2qlxqyvob.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ndtbotcv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2zeakryym.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xnerpxew.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gxulwrpu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2zrikxzmq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wlftvnhr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2iabowbuc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2hxhxvbhu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2zggholuo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2jcfmnfte.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2lqwajkzl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2tqcgxpwt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xpcqumjd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gjwzogms.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ijizqobg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2bgtyyrjv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2sphglbne.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2rhleyzvx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2caiwazct.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2dzttocyy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2xcckqxxo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2kdeeviyz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2pwjkjhld.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jfmzojty.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jeimspbj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2hwuqtcrs.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2uhobcwbr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2akigovuh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2otunpuei.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2qtcfyfcx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2emowopwk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2hsnzpsbx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2oxataqwm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2gxhazand.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2alvrjyjf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lbxngxha.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2domrwzgx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2wzbxdfwx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xsmdgomo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2qbgvejqi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2lbvngpob.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2pdcajcsf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tbsvfxjw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rwaegvxc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2cunkevrk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ujtoafzu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2impktfse.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2wsqsseli.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2hanpsyie.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2feoizokr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2jsmgugny.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2wwpgcwzw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ejnopxaw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ubmlurak.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xhnpyhsu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2evlrsqxv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ojfyjzpn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2kjulwmas.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2nzfbkygd.html


<!-- 参考信息 -->