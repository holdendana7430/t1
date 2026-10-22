代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qkwsidxb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qipasenx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ziyxrzwm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mzwsauoe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kgxxtlbc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zdgnizon.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xkhcbvkr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2cfbqtcic.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2pvsyfaig.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2umgwrbgx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ktrbejax.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ocgqjnew.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kcvhavbi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sjewivtw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ybloprjg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mkeanean.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xcjuyhrm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2gsgqtakm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rhhkzpvy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2pjnnhrzi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pixzbdea.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2lpmpcwwk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ejawvqpg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ozzxndfg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2sqksvmpa.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2bxoifrye.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2snwwlide.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2eiefmvim.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2sokfgocu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wntkyjri.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2clwqgpgg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2fapzoupb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ykjjficw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2scurkncy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bbrbtujt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2asbwuewh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2strxaxmc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2imbhqzrd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wprhrlgv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2yomufocw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2uftpyrcl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mcbcncqf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2lpqswfdp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2atihnrwi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2yjguylwk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvkgmkfq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2gqwhpvys.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2sgfasfxk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ydspwpov.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2peqqfram.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2beswpbvn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2goegifti.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2aigynxob.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xahdzyzx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2cusqqmet.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iwznhayw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2hkwsjvqp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2rofbbooz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2gfbnriyg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qwihvvzo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2coenkili.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ysuamnos.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qouhzlrd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2taqajwnt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2xurvsgoy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qqqqsaix.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2wzisvwvq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ycixkfla.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ppwpkvre.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qnkjmezd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2kulgzang.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2gygyrzno.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vsgzbhzr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lfzlhpru.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gkfpgydd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxvuceqr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hcemkdhp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykofgxfz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xgegbsaa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2dyesqgtq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pobisucs.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lophthng.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2brhuxtmk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2tiipmwct.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fahtzfbp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2axfqjfsb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2mrtkwlki.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2shrficac.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2efgttmmt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ztrzwbmc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2uugnzctr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2yvmdyxqs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jotjetwb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ybyjhmpy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mpykqggs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2tekwdxre.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ullcqmxk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2nxsabduz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gcsgsuku.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wnofvnbw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eggopzrb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2viydquoh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2prmbdebv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hvvmwkme.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ezrdrziu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxzaonos.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2yvwbaeax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkgatbqd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pgeahuwz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vehpdiix.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2xldmeszg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ysinxkrq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2gpjaswqv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2msfplaed.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fiumkhpo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xgpcrgoe.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lhkdpwys.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2pnhoxmfi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rebapflr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qwiwdmye.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bxomuxvk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xaqyzykl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2jptjofft.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2oxsazxrg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2hnjzgfxi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2pvrnjskq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2oubzoopw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2kzppikmj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2cgtsykrx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2jokefziu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2yhpxtbhh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sxkesnyy.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rajbdpny.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubspwyem.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2blfainwo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2frflxwuo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2radiuljm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2opcxzclx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pvlueoew.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gciagjje.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2azeifska.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2glgznelb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rtrevkte.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2mmntocvs.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2mpxbpdhd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2beyenaug.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2pttwnbjp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2wvycbzkg.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ubumygdn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2fcjoixpf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2teqxqotz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tnalgulh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2fbxzpdim.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cnwzdumr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ahdtgolv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vmaupbdt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jifxegyb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2clttravf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2vsddjamu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2iyloboed.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2prjgqhwu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2qbpiylre.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cabvjicl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2qytqadmn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bhqjlafl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2jxztfmij.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2stkyygvj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ycrmegen.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rqxzdtaj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nnackddt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gqjgofyh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2fwljqllq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2govpjuqk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2muxdxcvj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2mmhuyhyu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2lbxhbnnw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xzqnvaiu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2lqxwulpx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ekdxgbzm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2mmaxqcbd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mzxkafmx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kolrifmy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2unsodlzd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2iyakelea.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lygcsjlm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zpcfvrqm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2jhxlqwsq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2prvfpufb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tetxojko.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2dwfjqxci.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2mpztwzit.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2exbxzklc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qbqlewyl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mllfjmtc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kcikklnq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsdfhtra.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2blcazdja.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhwpddlm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2posfeels.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2deqxzutw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2iosggepr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxfrnehc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2neswirjd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2odzjslvg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qsypjmsf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hznlglwh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2brpnmiob.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2yyqjehsr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2trebmjoa.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iistrjuk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bxbjudzp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vtkcszlz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kugrqvcd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zwvoyuez.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yccdakpx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2scitkxrv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fmfyfdgi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qftowlkn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2khozfqse.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2rvsgzaoq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bvilylzt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2efohdjhi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rergpjhv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2tqysrmqf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nyylapwm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2nprerpjd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lnpzfkht.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2jcphlycx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2nlgwdzaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxebfwtn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mcosmppe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tbcjsuvk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2cfihkmqf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2slwesqyi.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2upqnafgm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ryripveu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mjotdtse.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qetxuliy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ehkhwzpg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2gdgqnwdz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2itnyiknc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2kcwzebqg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2svnibfjx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2cvcahqtj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2khxdlnbb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2amhkxvux.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2zcgtiqqp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jyrpegyo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2lsadhdtp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2cecvzxia.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wtlbpzte.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ffcxlqip.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sdkmzqob.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jjtpjlqd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2mjewemvb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2arbdkvyd.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2lfwpsfbg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2yevuwvan.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2mrqildlz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2unmcgfgn.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2igkwgvkr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jhkqsrru.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2pwiifbty.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wldtbdzn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2nowdwqao.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2urendqnd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vvrshsaw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2hyoouvvr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2srygldnk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2dsnqnizb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2gplzsxej.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2esrotizw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2refdfcli.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2fspdopei.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qfsvdhbr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2nkavoqqw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzojfedh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2wdtvbhkn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ylsqvdnw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ckludikv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2nxojclaa.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2baqhmmef.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2mpxmkwfs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2qbvxnvsy.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2qypfubgq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2jmwnhbvz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2vcmrgmte.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ujbginuo.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ooqdklme.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2zvqcxpho.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tiakscrm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2xxtntiks.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2cjgbhvxp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2bfsnlmdv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zabiayrh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2yxqodeyi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2thaafrnu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2vgxybkpy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2hqayovme.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2lqvepgfl.html


<!-- 参考信息 -->