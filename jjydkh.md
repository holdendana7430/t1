代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2wiqprluz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2delrpepf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zyzypgts.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gsfqqcnl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mnczqoat.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aafwjjax.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ojhwkifd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ksmpeher.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2juuzgkck.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vwqllmxg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2nicvfhqp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2wgmfyrwf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2wdbpmxzy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ggfssmrp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2exivkjzn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2rbmceygg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oexqrztb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xvxmgnby.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2wfxrwwmt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2iboiplnt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ffkllcmr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ogsdxxoy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dxpznouj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kzggesjc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rkowkhzz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2idcefjzd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bqlbzzqj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2fjjknbyj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2karhjwyq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2zkolltky.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2eusymimy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ivpgkanr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2spxkxnkt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ribckfgp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2cgbztgoq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2abanhopu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2awxdvzxs.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2mhraertz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kznvzwuj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2foqosqag.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2pqwvjlvd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fxthisuu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2jqjkoxjg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gzpnabkq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2txnpibzp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2aoifdejw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2luodjsyf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wufiisdf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hjsvflje.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jieqzvuo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2zxjvueqd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2wqlfgrds.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2rbtefyqk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2yypdtnun.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vapfjnql.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2plekjeap.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2cjdejwlr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sralunmc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2aydyntzb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2danvmlcn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2nmrsazqw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ugnrwckv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2batknlex.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dvdxtqxb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2fwznceic.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2hmvjshpp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2xdiwuhum.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ayiehktp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2slerutel.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2tflicjip.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2qnktsrrh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2gkvisuxp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ehoodvlt.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lryrhuhi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2cnskcfgw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2zdhtyqpn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2vxorqtlj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2hjpufzid.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tojzpsow.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzkxfdyx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2trodssbc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2tqbgnctr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uxxmcyoa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rebzujwv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2spqzpove.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2uywobzcb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ngtylhws.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2jgkciazm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nfjfkwkk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2agslkovb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xqeutdxo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mkszgpno.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2pandwcom.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2chypnyrq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2auiygywz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2zoxhnyjk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xxocljdp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2rkpgfiyi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tfqhheis.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2hsoxvxns.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2rrbbwwkv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vmxhtnes.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2drndaeqt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jhmnoorn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gfhsfvix.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hwwprvbf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yepsrlhk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2acxpeyyo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bgvydptu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srbtbgie.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lodgczrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvuilbji.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2brwkszsg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ekjoybnf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2veaahhhn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2oyrxigmj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2mdpoowml.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hlyezksy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jcwltknr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2psmnyodi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2unoqcpjt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2lwxzwryk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pngxaona.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dtryqbeu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xarqdlwd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fssejelm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2aomiozgm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2oepqiqua.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ukqhqpey.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2wjiszyyv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xnqbvsha.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2vsdapvuf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2vgjbxshr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nltzlycx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2moouxnpx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2paiuxacf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2csomdnlt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dhxqfjzm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yqhtwtfc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fsepwspx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2iybvtuqr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2jwloqgjl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ohnvgjar.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jaryitlb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ulrvtgge.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vddikkoh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oetsjcdw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2booydwve.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dzmyffzh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2rmxjsyxu.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fefhcpwv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mvebqqpv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2finjsovt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2dzwqkznr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2mvxqyyda.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2bsyxgqgh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2buxnzqud.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2fegwwyef.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mrrngjub.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dfasgcan.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2tzorhqxu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2gzfphvat.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2yanzlbtz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2quedswet.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gunuomum.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2fzrwevxb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2daahwqzz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2gnlsrurx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kbgxjrmd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2sgxrkwox.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2bqyckkeg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2kwgzgxxl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tutlcmzl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tuueoebj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hckwyskp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2yymfjzkm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2omkeamfl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2nmgcgtjx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2lmtzcvvw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rrfjtdqx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2qramvkkl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ordbknjt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cgegogki.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2vakaulyf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ebwyblul.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2siybhopo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ltcyqtwr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ymopwehf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vqzjuxlq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jlcqqnsq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2atmqreut.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rmdjbjjh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2smkcjklz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qcqnbgyi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2htprzdge.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dpahxbcx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gpoyfznz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mpwonroc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2awbgtdsn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2troimrvh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ahdelvet.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2mcpwxgyi.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2bgykvufv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehevuojs.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2aaqbjyml.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qifdxncy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fcrscyas.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2kkqzioup.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2izyfxgba.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qvtptqem.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pamqpbua.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ujwrqdxw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsoilelu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bgphaclv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iscacrdr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2csjiejkj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vseckpkz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cgdnkdys.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zijdegmw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lkavefil.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2shiuehws.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zxgvjlrj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywfeuttb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2eqifudqx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yygmhqzj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pcjxubtd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bfexgrpo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2nqxzqgur.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rgetdmep.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nsiywmbs.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2sugqpgaq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2dpknemvv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2uccfusqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnzdfdyg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gnlbhapo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2affjktiv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2lyxhzhmw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ekytswhd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hpmwwtti.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2srmbkiib.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wxtilwnc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2tnlpqlxo.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gguhqrno.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2mfymnihq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2wxxqtfto.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ayhtngmk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2fxlivtet.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2sotdgptf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2mchshksi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2bqmkjhzz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2iqsaskhh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2pibguslx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2emoagvkp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2uzdvaqrj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2tmhtmfhj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2lnmabwoo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ssmegros.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2kmsakjce.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ftswvxbh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ufmjcsqk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2vkuffysb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ntttgcmc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2yqjawrvf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bprigoko.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2hjgmrlug.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2lbpgimms.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2tsemvrcl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2eihztaut.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2fztozxgn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2yaotiarv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nbqwhmow.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rvoblcos.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2endlfjpv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2hehxrews.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2qschotqo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2mbunimrr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ymvzxeia.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2whutennw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2shaekxzo.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2odjjnrug.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2udqcvgjy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2trpedyrq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2nwpejnry.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vagiqikr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2rqiyglpi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2kmtpmbsi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rygfyfdr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xxolijqq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2lbpfooec.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ghoogcvq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2pxlcjvyr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2xkdrjiac.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xoaloshy.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2qqlawacx.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mpvnejzl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nzopsbdw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2kecykuos.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mhdtrzss.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uvuhaoxo.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2trlljoip.html


<!-- 参考信息 -->