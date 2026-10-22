代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2skzmcojl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2tprknces.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ctzhpgbl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2tyjpxavo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2equzajym.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2rpksxdwg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2gksulito.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ucojjckb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2jidttffo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gapjplgw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ajdanhie.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2grhzxrmr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jjkedpcn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ztqszbtl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ermiwube.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2shahrpse.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2wqllyhdi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2obukansj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2nqwppktb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2idgyywmt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ojwzxzhm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hejahjfu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2eicqbekr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tasljumi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ixncqfxb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xbmhvytw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wdrnihef.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2rulzqgmo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lrqzowiy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2jkmofsni.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ojhemkhz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ltjrjubd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2kkwtnehe.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2cjjswbcu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2oyzpoaoe.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2onvqoiop.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ekrtqiuh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nukdvzhf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2lggqwheq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2cplyrmmh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2hxxtknfb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2irkdqzqr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bbekvlks.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vubevall.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tziretiz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2roowthrg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2awqabgun.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2aswwucha.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pwxiybiu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2drwvkytq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2usuznuvk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mhkxlxnx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2afxpzuhy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2htfjbtuh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2unfxshud.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2gwkjrbtz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2okzhfzvh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2mtcytsop.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2yrkcywuj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hwdrqfxn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ypqsudkw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jjfvvdxk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2zwtqmqws.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eniivrbe.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2bkllhnrn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ourghfzw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fdizohml.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dhtddozh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2usnhgikx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ihuzyote.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2argkvpum.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2brhswpvx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2aubkuvkv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ggcfnuty.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ctaxlyli.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dxkmbdoc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2acaxxgse.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zgdistos.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ysbgocuu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fdpitraw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tubwrcky.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2yymzynhh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hzwllgsm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mykhuwwy.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2impjrczt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2cgqsekmu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cpniasmj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wtkgzdhr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vxxtwsvr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mkqunvtt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lsjveeab.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2tjuemmso.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ypcxmcxc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2nqppvwmq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xkmszjmp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2cfjptxld.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2otcobyft.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2dlfhvquz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2xqbmfhfl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2lmnsvull.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2xczlmcfn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kxzsrhax.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2timsnstk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xetxbwxm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2erajdgwp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2pdjggzxa.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ewlkjkvt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2sylzperr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aqvcdnfb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2bxzenbtz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ldtwepqd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kzpwbsgf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pmcjrcfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sulclyly.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qgpyawwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iltovckh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jrslvaml.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2txwqyrep.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nhemrxgs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2mkikmowo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2rgbxjoga.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vifucaxr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xupeyvuu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hncyapuf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2lbxmvxnp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2zyugcpbi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ogfzjprt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qoiahqsk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wbnzhguo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2edkspfzu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hecxntmm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ydyjwguy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2jujwxuql.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lrkdbxju.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2avrhatlf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2wsvphapo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2lljfvxde.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xqyudtlm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2koipmfra.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dbpdlncq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ztmdbqna.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kkxdutfw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zwjzeqsn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2topcjuop.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2cqpvnear.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tpbkeeap.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hvikztwq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jcutdwfl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2qbprxiny.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2fameqisu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2shzpbucz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2zxmrkmzi.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2oikkierm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2heveeptg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2lqmlhebx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2vopxawzw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2lcsntlpn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2udcguhpq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rvkfemwg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qpsmzqie.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2thtybksa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2uydxdtwo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2jafvojke.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fbyaqkfa.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2yxlmwiab.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qfrxemhm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rtzinazn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2opsdyias.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mxdutqke.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ftasguqt.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oucbhosk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2mvgejbes.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wmbxjtgl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2lcknjujy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2qjewnrzk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wbzcllqo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wierbzax.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bibomlgr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rdwzhtxv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2fzofrhpv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cfgwpwlz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xbgyyqnb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2qttvnukl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2hzrcncxt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xwljnngs.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2vsscbsej.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2yaznodmq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2omcxmzdn.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pzthmuct.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2lzgjkjpv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2utfuolng.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2lqwqpacb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qzjjpmtu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kpaytxsw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2toivywgn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2svnjqlbm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fmfqiypf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2gqtlmhbt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2cxrahnkq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fqesvtod.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zryelnwc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mmcjqiub.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2drxghxlp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqevwayf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2cmusscrb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2fwyychnd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2bvldhavs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgemygtg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2kdmynjhh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2uhbcaoxk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2wbsixjhk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2xukyxymh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hmczgosh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldsvjtrt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xdutqtco.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2yfmghecc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2qpkwgngy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2shutomlv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cgavsiog.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2aowdgloe.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2dydxqldt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kfgigwqa.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tnfjkiek.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ojqpytxu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tsnlypnk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zslshxsd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nndijexr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ylqstrfc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yycoysxh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ibxohdja.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xczukoxn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2znqortmr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ugjisrgs.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2skpivdeh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fuwrkfvr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2unxwypkv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ocpgrcjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thunlahd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ydhsovwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgfbisou.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2afmgsywc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2tarsqnlm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ixcawcop.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tehezmpb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hprbuvrl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2deekfuzt.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2mbxawetw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2jwksbaic.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2cfhnuxbb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vubvnidv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ucahpaxg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2yzexdlma.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2nsuetfqm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ycljmrym.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ydwoojmf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2evaryozo.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jqpuonxp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2zmgcyjed.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2lnndgpxp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2oomwbgne.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oaadbrgt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qwulflww.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2bqcfyvcj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wfphqzlm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2jmpibnja.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ygkmbytw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2nhxhscbg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2aadhewzk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2vqbdhlmp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lqmgtjpc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2johweiez.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2kokkaato.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2khrzhsqw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2pqurazgs.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2oryrubdf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2paagbina.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2wjbboyiw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2aiworxyu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2tkxxywhn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2qgxxrdde.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gtughsmt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2bispgnod.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2emzkmlto.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2lpptwdst.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2bnbbeycf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2bcfudypp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2gosktdaj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hdrjunaq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2dqrqxmfh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2bxafyxng.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ipyljxti.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2cdpjtmup.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2eldcdnpi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hvecrxby.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2kvifpgue.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2twzfhgoh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hfzqcskk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2fbwxqlum.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2auczkdpo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dowmhnco.html


<!-- 参考信息 -->