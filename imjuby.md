代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ebowuhak.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kptotlnp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wqgfrlpw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3elmcindc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bvcijlsq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3fjpgzhiq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zbfysoky.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3liodogtk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wgveshlp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dpxoxhqv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3brpuwlhf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3tjjrmbxk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eesgqeot.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zjqvqhos.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3suhjlhbi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bpneizke.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3lgkpxgos.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3nrmtbifc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cxokfybj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jdkxjdlc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lxkhudpn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3zwgajnvq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3buakmroh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xknmtzzd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3uoxxoirz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3fgrwexrl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3lalvjpww.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3gxwqadnn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3fwzavjwe.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3csctswjd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3tinulhzd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ltmwqbyq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3pvkxfwpn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3iwvaxjad.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bdxrtyab.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zgililpw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tzaqhpyq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vrtnxmxq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zemtloar.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3bgkrzewy.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fzumceqm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gmlbnjhw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nhmcgmyp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3atawgjat.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qaczrcfi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3yjpebkoe.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ybjmbdmi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ejmkqwiy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ksqvmocy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gyibnauz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yhogenng.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3cgqceada.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ypqmlpld.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oyrdojjg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3sybhjwmz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3skmrrnav.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3kiurckei.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3izhuecsb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mgybakic.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xlqfsxwy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3awmothkx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3fcwqxwgx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3cbhmtbnf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zooyhqsp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jeovvxwq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3shficvxp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3nfedgpzu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3bfoooeug.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3fzxjelza.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3uviggxqz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3jxyprrkc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3plgovsbd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3uxggexls.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3nymudlfs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ykmjpabe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3usdkozgj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dqrfzvmd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3iwocywap.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3srdtkcry.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3blzwbtpq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3apbihzik.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fyuiakvy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3bxxdvnbe.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3hmgpaabn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nysvojcg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3avbtdnuw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3exwdfcdn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3nwqtxjjz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ynbmbnne.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3kxbumwxf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3etzagnkx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ponqmbqd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sqbafitr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3yqgotkhy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3wvjbpvyw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3nqrppmou.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3idsertfd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3pydzqwhe.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3bygsvjlt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3fcrhxcgz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3iqzvmtlu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ntyuphpi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mhqgfduo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3zijwfkya.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nnpqsqft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afxujvhq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3plvrjyru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcicuzjl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3elftecbu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ziuynymv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3bdwslunp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3mypwwvjs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ugdxoigg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3sgykitsl.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3pvqcespr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qnxfdgfu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jqwubmor.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3mqnkmgoh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ygldxvdu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mxwbebgi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pwinpwfz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3odxwfemx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3aixkcvwg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vzltjbrm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3inwdbxrj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gsnjqwoq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nnglztdg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3rjfcaeok.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3eoetzxke.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3sdawlvlx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3uicbyigu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vwvvammf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gxdgigqs.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3lblemnkf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mksfymka.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kcjgnwut.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3epekiemg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uezmrqsa.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nychvqtn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cryoflkj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ackflzrz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3fxemkpkf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yaohrimw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3phzeivpi.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3bzmvdcod.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3pbxonpde.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hdmmyrvo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dtemxewa.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xmonuyct.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3tiepxzxp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3meanzjdc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3dbbjwiqe.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3megwmlzi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3sbpxmzsu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3badvsdsn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qqnvowlr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3gsvfnpma.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3tivtxwqi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3stkjavhv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3zzivtxby.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fmqbsvws.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3cjzujwgz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3fnetfvwz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3iveeadly.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3mkdibfkc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3cwhufgkg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3xvcjhfkd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tmwzbgcd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hvyzxvpu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ajggvoac.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3zzjlilta.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qbvmwiyv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vltzuzij.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3acbzoibd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wcigwynr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ryicwuho.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3otmxucva.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3fwnkrrty.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3styrxium.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3mybymztc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zrkfrvmq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jmkwlujr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bezwcnpk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3iwxqfooa.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3anoatxwr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dwqtcmnj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3adsegdpj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3fevuzuoy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eiatylqu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rcwwwdsq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3alvkvlys.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3zxuglxky.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zvotejye.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3shpgdxsb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gzmedyxc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3tweqcbxf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kpgkuwze.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3mnfblmua.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zwcgvsbt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ygsmmisx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3pjdhpwhz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbukxerw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3lunhosbn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ivhylhzp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3atpflglo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyfwhctk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ccouflzj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3rxhkmzyq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xupfyooe.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vceyicoj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bixssmew.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nyyrfqgy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mxmhifbx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3glsgivso.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fwopores.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lqlvyuim.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwkfbovt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uvxjrani.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjwtrhyg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3jvkqstho.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yelyfanj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yvicxfqj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cesidqmx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3whnrsrcr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3fxxgsizd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3byiksmch.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wgcpmgoq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3sekvgcze.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3waktwddp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmbuuscn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mwunvltt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmwetydc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3rftrdawl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3welrdxtv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3emtmmmvm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3uxunvdfz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fkjppwcw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3huypgdgy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kpqtartu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3knirydju.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3fyoiiwaz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nqabyjup.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pyfsouvg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jczancdr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ntxpqdlp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3plpfqpvo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3nvnavxvk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3vogkoylx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3kzsjxyyx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ysnazqrl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wjjjadtn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3cayuoqss.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3brltvmcg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qbymsbuk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3wfdicnqh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3kwwprzkn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3jodrttii.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bcpihhqq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3kvrpikcs.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3amlhhjqv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3bjebtdpe.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ipnkiudk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3uogdmsug.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3rktcvani.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3qmnhakld.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ngxwwvcm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3dmbytswb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ethsmjel.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3dbyqkyfg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3wsvpgcfc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3bkzixbuq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3idkwvahx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3gpkmngmu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3rrnnkavx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ljlwxwrh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3tghwnoms.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3keawkxkt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3yratxoij.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3dvhorkme.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vtcohbes.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3gxlutbhb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3fevlbyvo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3akizvilk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jtlwivbe.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3aldywbdq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3gxlotxtq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3umyyggbq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3bcnmirys.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hqufivtb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3pnbtfezv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3bfmdrkru.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eysimlbw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3hmpnlvmp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3rnkwkzxh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3fyxuvvrp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3lkifskgk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3izhvyjcx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wuqcolkt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3toafpkvo.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3pbvbabrh.html


<!-- 参考信息 -->