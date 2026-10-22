代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2uoygbyqq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2pxqdcozj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2svsidqvk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jvbtnirr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nlwkyrzn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rsthunsm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ygjfuixe.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pnhiaiia.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2umuhhbqa.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2nvqmolok.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2qixceced.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2frgeddkm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hmksjtnv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jnjtsxqv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2tckosrrz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2hhvjmfbm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hqvspdmj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2shkxnile.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2trixwctn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nuncrqad.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2oiwowcdh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jdgzotim.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fxxxiqja.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2dgvewzcm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ajkspyew.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wvrqtnng.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2mxxysbdn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2scholdsf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2hgekbscy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2eerdanam.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2iyjoykuf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2fiphnzbc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2anltyicz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2olprpjzs.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ywfjgqju.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2dfmegyln.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ocmpwkdb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ckbeolki.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pesuuyyw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2vsjhzain.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2cznxbxwb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dybqxhhb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2mghsgeac.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2iaxwyylr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zyoatlqp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2xekeoqiu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2eingtyel.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jvkktuow.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2gtyflpxp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtitshrc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2citjiydf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2fpkagrxj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2fjwdhiyl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2vwpjxbic.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2tgkqxlbi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2eqgalzqx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2pdydatik.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kywahezt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2owpoghcj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hkqadjtw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vxatrixe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2kuvhxoou.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gqugnxex.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gmnuwnsd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ouwyvowf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2bebtyzde.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2fcowwvvg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hnrsmkmw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ydntkdxa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2rbohxpzr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2sejygchh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2azjweziw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ywtaydrk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2afnxebra.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2nwzjhqlt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzyhpipy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2blpbqiau.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2lxvstmyp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2whvcgnwm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvoeofxf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zpzsqght.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2utvttsul.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jungknox.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2qvwkxgoq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zxuapaux.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2jvbqdfag.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2htxlhqbj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2tqgxtqoi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jjaetxhm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2jegngkjc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vewewnsh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mtaiwzav.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2axnlmjih.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gbzyuqds.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2rczuadij.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2djbcgreh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ewvuogia.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zfhscbnr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2btouoglk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xkyyqdoe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2tskeuprb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jufoshyk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2okglamqt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2neloyphj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ncqfccat.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wigztwia.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2bfxvhkfs.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2clgkhguo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2itfbcczf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uchhgjzt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ucsliiay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibrycsqf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rakdlrgg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xsgotkrt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fprckalm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2zjtdkhcu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ywmfzllm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vprkfkvo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wwkqmizp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ykplhsoy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ldqdmxpp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ueasfnbh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mdzsfifl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vyvrxics.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nmaclvho.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2alccsawf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uhjpjirw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2iqqxmkdz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2rohsuwvr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ekhhgejk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2adasmtxx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2szxkyieu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2jpaktwsb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2pqixvfga.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2jfkjhuyc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2upafesbi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ehrstibr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2fcfqbqsk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2mggcwkfn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2unxryxwl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2cgucutuq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2soprhvll.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yumlpjaj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2aqxftjkc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2fzakfxlq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2vnetkdhg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xsihblvt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2wlanscxy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dnqzzdsv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2gbfldkkn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2xdzukgau.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2dqfoqhdi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2zeunloqg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2njvovhsn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2nnsmolnq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mqimzwqx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ekcbabcd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dboxwyra.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hyauwuzh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bjmsryhf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2plhylgln.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hhozlqcm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2qdpjqoty.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lszckxxr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vihkvqqj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2cinazhio.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sbihhcku.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2drroaayn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lunrlqow.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2kbmzmrkf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ifmvegmp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2emyruupk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fmuojcqe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ersuflrz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hjyeviaa.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qrbhfddg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2nqlshfxz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2svjtbaeo.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2xfbbndoe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2bswfmpxk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2iiljomby.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2hkmvrofs.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uitbzynd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2uokgvmdp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vtngzblj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pwcxrneu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2itrcekef.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2zandzxxd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ddbzwuwg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2sgxuvewc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2elxymkig.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2cbhhpjxy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xczhtprd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2txfqglwj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2cjvfejaa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mtbxtaul.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pyoyvhgz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2gusnhjlp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2lsnlquyh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwxugpyp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2drirtlge.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2wvohcyws.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2dpwqzimb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cducseis.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2znzsfzud.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2glflhwqi.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nxzrrzuf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2bqrisnxz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2onpizdco.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ajfzuzgr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2doinjhxc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2oefxsvbi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcdqqena.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ruiwphpa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qhpiyfsa.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2itxopuip.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ztjzaven.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mgfnufky.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mdddxidd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pickcbrd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxbcvegw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bevhcjqx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xlnjnyji.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ghuftits.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ovkafdcz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jvtqwnok.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2nvpleiox.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2wngbmnzg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2flsnpzux.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pzahsnka.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zimcyybh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2icnlnbkw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xtisfjol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvznjilw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zxxpumgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cetffjlu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2kebxvbjg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ttikmytg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2jszvvgfp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ivvtjliw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2naxtqzxb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2dpfazpbd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wjshrueq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2pgarbkcw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ikxhxnfm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tfvkngjn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ynfexopp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2iefcpunk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2nkqgbfmn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2rfctipes.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jmquqkxq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2txpehvbl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2jtqndfey.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2lymdcruw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vhnadubs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2humpyqma.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vqjrdeyw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jpyxuude.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2yupxqspm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2lmpklhhj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xthnvqpd.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2jkzszkoo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2zqsghbts.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2cvitnjtd.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2gmaruegf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2tscsggqj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2uonfbpao.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ygbtcbfi.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ipegzzbr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2aucxyxhv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ymlrkpdz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rwmwtnfc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2exikdcis.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2eyihqljl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2yjbzjbdn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2vyxslmyp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ocphyras.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2anoqkrkm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2dodijtgn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2kddlhmbd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2anwstuia.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2cjmibcjn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ihbnhtfe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ermbdmoq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2pqbvgmxv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2xyewnfvd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2cuygjvqd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2nznzukqw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2xzfcgkvh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2hsjkjxtv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2rsmkdvew.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2qmzqggan.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2thqfniji.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2quvqzxqh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vbsvxqrj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lwxewhge.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2nvblguwk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2nqkbfjwh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ceofkmgz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2bopttrol.html


<!-- 参考信息 -->