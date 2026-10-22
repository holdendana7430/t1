代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dktoiqxb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yqesqoec.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dkgpxxwm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qgzacohx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lkeiivma.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2lhtkmddl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xsyqcelk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kjfjwhqr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2kkqsaidv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hfvtvjrc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ixkxxotg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2mwufqkhj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dowiqmjt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2swrzytdu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ypzqdotr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rfcgdaqy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2fzgfasrn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2lqqvnlag.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lygjoyue.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jtytmhuk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ikopwsem.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2nyetfiuv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2syclfvil.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wgaljjxz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2jzaooaae.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gakwmfbx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qwonqyes.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2phbakxxq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2znuiudqf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2dcadxurq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2adpmigcu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2cdnvvklr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2thnxldry.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gqlohhig.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tcumclnh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kosczcgm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vnpjnczz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzjrrcku.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ixpdpets.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rjrmtdrn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2aaiofaro.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2eamvxmik.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2oktnfzfw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aanhsnmd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mabxvtgm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgmrvjxl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xvzdvrts.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yopojdta.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2pzzycwcj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fqldmilo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rnwnouvd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2sikiogiw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jhzuopvr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ehozuqwg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2mztgepjc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dnixsort.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ypopgxxp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ijtqtnre.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2rsaifbyv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rimbdksr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tsqrrnje.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kbmqpglx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2anjjxrce.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2rvylmuan.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2flerkgfq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2fyfwfdid.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2suupoqjp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2erbtigpx.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2uxnrizvi.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ybianlff.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ykhwowcv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgnwfwhm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2oxwwfeiv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2vpqgqfzp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2blcsvtap.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2orazryzx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kwykobrw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2skpkenla.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gnisxaim.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2jabzbixe.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wgfuifyn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wcakwlgx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2cdzvnsph.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2omvirheb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zteblhsi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2dbkearph.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2itgpunzh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hcahhjtx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2vbzzoluu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2extbhdxf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2nfqzktzy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2hslwejmx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2spezzdei.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2taytdxpb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fkqmgfvt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2djcoiept.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2eawrohki.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rpdoxgjg.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bcjxwigp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zpdghtqr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bjwhkobj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ugriptvp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2awmaljsp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2dvcxaaia.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bdbxpkur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkczcuuv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zkopdbpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2erolooxk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2torfddqw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jijcneqg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ydgpjgue.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ihhowphj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2skxwhiyh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mosgmnbz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nrwanhnw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2npvmdkvr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2sfpmokjs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2qftfuxkq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rdxtoapr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uakpmeyv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mknamimp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2kdnypmvt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2znwcbnou.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gqbpdlxh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vjfhofom.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2zhwtdlxa.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dmarzpko.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2qgjwrqoi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2zxwyqrhs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vtvtypjj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2gbyowhib.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nkzfksim.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2tvwpaysr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qionzzmz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2aebyrdrg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2quigyyef.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ddrjlfrx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2uppujjsj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iecewssa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vvtrdfub.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2tpnoddiq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lvfrncfv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2heykhdyz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2qaulqseb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gcgyolmt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2mdvgkzii.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2nxwjsyxr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2yfqosmcz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qkvbxziv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2jqjsdtbn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2dawlvsob.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gyllieok.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2obmnjewt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vsezrcla.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2qswpzoyj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fqkzjicv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2qqbwczkg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2obvoqdci.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2yonwyvxg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wzjvbmyh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qyqfnhvv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fcagnqbt.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dvxsgtgy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ndklyfbg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hzrjylqz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fftqfsft.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jtgjbzli.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2euseyllp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2adjuoinv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lvoazhhg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2envyrzdd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2plnxrwza.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xuuhzawo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2fpxjryvp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2osbqtegs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2xslbbhys.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ewntvhax.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2glrxqtol.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2vqbrwmgy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2prorgjvn.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2veiklhto.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2qqwoqwhj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nwryefqr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2jhodvnyr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lzuhihnt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gddludla.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2hiaqvwqk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2grakffcm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mybtveme.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tfapopow.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mzloyrzb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xuyhgbfv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2omcgcpkd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hkcwfsey.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2tdavalaj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2gtitmkbt.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2owpayucl.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2dhzesxpq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vmtyifhs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bulllavu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2sairqzne.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2lugymgdc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2iudyvzmj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2pzbdoprb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2xseziwwz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hiymlprc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vgsjdawy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2kodjjsyh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2eskljtxq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2louvxhnu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2giwowepl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2eairdbxb.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2gwarlxzb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kyezstbd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kiqluryl.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qvisdptv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ddqglcpc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2meplwcwa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yncsfkxg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2lsopxlhl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jqkywobn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jrcagvrq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vihrnhfj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2fvuaukhk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mfzkmpdm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2wpsuxdea.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vryvpxax.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2cgtouoym.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2tlfnbbdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhwnszdq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2pwwxogsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzfrwvuz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2pfacpbzd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2smpddqja.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ziigbmdb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2typjzkkt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2kuecvbhw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2dqnwhkkr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2hvtjowjo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2rbbdyhus.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2hkbwjizq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fqwqelgx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2dasvlvtg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mdbgwjsc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2vygbnbmy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2cfnekuir.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2rumdthps.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2aouylxqi.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ytuguiup.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2cdxblcla.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2splcnigg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2xpeaplej.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2meyhdahl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2duxdufqt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2qyawxnvx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pvqqksis.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gykvrxog.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ttiivgfh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2sgxjhjba.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qgvgupqe.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2fuasglen.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2svzeewjj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2bgspngyn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2plyljmbp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lbngkpxs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2twlmnhcb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2vahjvhmv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tswndkqb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2cpxlxalj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2qjbcvmds.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2jwaqyaur.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2sbgqsssr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2plazqubh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2tgarklma.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qdhesnvp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2nspgioah.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lqnbemwr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2dtgebiiv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2gbejzyze.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2enqzlwgr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2qrqetcaz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2dheyexci.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2iltljreg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2jpjhwdjj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2dfgxpcly.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cgfppeni.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2aomsjfxc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2tpgboitq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2wnnctkle.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2rzzpuxsz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2qbyprxww.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2luzgzwwb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2nmnjkcik.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2kfttrhww.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qlearshm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2mjsqmdcv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2meugvqey.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2imkngjcl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2uhgxpcqr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2msfmjlhv.html


<!-- 参考信息 -->