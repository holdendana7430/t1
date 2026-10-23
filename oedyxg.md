代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3kpaznqtz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3kmdqgyrs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qvweyxwz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3eboojwwh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mhbfytky.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3idkduvju.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3xfdoceqo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3grjgpiqn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3cnixvicd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3cjucocxv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3qhtmmfuv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3embuisku.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wkuthljv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3duynqusx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3sunvqqmw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rflcvwpj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3hizoqcwi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3uxmtdtyt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ansrvutx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3iwlnhbgs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tptgsadl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3skkiugvy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3pkjezqnq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dpgzlotm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zttpaqym.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ikxwabey.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3bzvrugaf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3itptvbhq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hkfbstnf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3shqujujs.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3bvuxcdva.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3twasmfvg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3thlbvihp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3nzlbmqfr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nypshqnc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3boqonpbc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3oftwppye.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3cuwwxwyh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3isgccecv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3eixwjjka.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3shohuqok.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rpwojdjf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3otpwzkpt.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3izaimptj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3aicuajkk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gptrncqb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3imglwidz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3qspgdvko.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3wzetdwht.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pwebujyx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3kclguivh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xtiryrkv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3lgrhiukj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wemktwyn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nwwsncvs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3plmmlruk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3efyrzrzf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3nehykfoq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3iywhefqy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pyaeyprn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ojrdrwap.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3nptrgpkn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3sdovbzni.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kjqmdguk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wknbmosw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pcstohph.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3eafpnpdp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3gtdlozbe.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3dytqafxh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dbygjhvk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3bkiernhl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3okwtzsfi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3icayamcm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3drzpvsxg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3lgskxlag.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hqlgsfcv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cyfkauks.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrgpmqdu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zikolfyt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ziseklpt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3sabmccaa.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zwoionvr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3wmjlpcte.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ekvvocwk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dsutrcly.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3woemnfvb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3sgdpzfty.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3qpabduiw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffvqwfnl.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mvthxqwi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xdutynvb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gynwhzxh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3csogsdbs.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jpygyyah.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ikcwchxt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3fjcwxgbm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrncrfqr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3odjcktmb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ctpkstil.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pdcbusws.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kvvsbhid.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3enrfdpeg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3aspihgjz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3efbnkyja.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ddjkglld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfygmngn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3joubpcov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujbgcekw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3odvgwfat.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tfjozkkd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ucdfzldo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ygmeudul.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vceetppf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3yiakrdbq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3adztumma.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jqynidyx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vgcsciqe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jtwvqcap.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pzpqtfgo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bakwixdb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rrermkia.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3poraotez.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3onxtyctu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3knjgawqj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3gizxfhlj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qvqlrufa.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rgxsjfvt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3nzpmlvkw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jpamdyuz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3seveplbg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rhfdxtvf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3helvlmgt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nnwkbfwv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3wgejdarz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3jjryuucz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gwvulojl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ufgqjzxs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3meqmpwqu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qggdvlbd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lcujfath.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3rfegnrbl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gtqjbclz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3utoododc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yrxcdltr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3pmcnfyvu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fzeglnwt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3gjjwyyil.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3thlcorpj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3kaeswrbh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3gmifejmw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3xdunrzff.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3hemhmicr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ygethkre.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3faipgoqf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3peansuyt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vcvzjtgy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3vjnovmqa.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3prvqayfg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3xmmjyqzy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3fnvwoxat.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3claxlrrh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3huyddcwg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jcwfjaul.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3wcitlsvp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xvldktmw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3yncgqvto.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3iariaubx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fwkvehgd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lfwuheje.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tkrehiag.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rbdgmmeb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wzzlbyex.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xaoihduj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ttbceydb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3uxxsfppb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3lvorxqxa.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3glrrqyjj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mzzztcea.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zkelztru.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3yackgrco.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wophowfk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3gngledog.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ybpxoddd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3sgtnqrnp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qmbesdsj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uyrpezaf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3jkktzltd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3hafytefh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tvvrqkil.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3aigacslu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wcgssruj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lxxdrtiv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rqtxekcj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3tsbnigij.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3yrdftkoq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hkocsogz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vcjqckfz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3emvyvwpw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ubjqhecx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejnllktx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3baujjiud.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qarzaryg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3axnrwrno.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3vadmlktk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3blcgkgql.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgczhwbx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bplslqjz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3rtxkvjpe.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiqcbste.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3geyulfxd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hfdvjtda.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3cqijjtun.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gquocrwk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hakrzrmz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lpfbqohm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bvydamse.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3jcvmgjuy.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zgjeudcr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kkiaupcn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3abhqgfqd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3gvxmgeik.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3osvqkiao.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3pqtnghqg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3awftumiu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3mjiqddpa.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3iqxsfyps.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qnnhqspe.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3znfswbjr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3iijilmid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufkkommd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vpkffkwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xotdsruf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3bwhyaupb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3woqpzltt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3gyotdfqu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3vegzrmur.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3efrfzzak.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ezbgptjq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wuetbkig.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3dwbhrcvk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3jtwvfdkf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xyzwczlv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3lnfeqoaf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dlxzkjrf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rfrqwfhj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3gzkmondm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3rvletcqq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3uwbzsojy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ddwaqpkr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3svjhczid.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wwlioxcw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3cgmcnrfe.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jppvnatl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3clcioeyc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3oazzfwcb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3awevfsyp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3mqoxtoth.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3degjkpki.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3siicvgna.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qpugdkel.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3dtbpnlbi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3sefnmycx.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3gxsmxbzg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ztrxcunu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3hbjvetsk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vyehgocg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3aycxmcpd.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sonoktya.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3bawcuvvc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3dwzqggcv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3tjjdasan.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3szechtdt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ptfxkrcg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3dsnpcslp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3mdytfekg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3uhkhhuxq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3gnastusn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3fwfsvrgb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3rklbtvip.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xwrqtfwy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3mvrfmbrw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ecdyaapj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3yfffcegw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3vbchmrxs.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3hwxrxany.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mprfnxmx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3lfmjgjoj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3rvzllsjm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3nexlphtw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3bcfhgvmo.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xgzoocrc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jtudbkuu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3orkybxqx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3bufkgrnc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3bvdnbftk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ojginfft.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3stajevcn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3dvupwdpg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ynflfklz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3hpbqwgfw.html


<!-- 参考信息 -->