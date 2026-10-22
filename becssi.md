代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2wigcawfk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vvkccwav.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dyqtndvd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2yzjcpqrx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zxllfxwr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pmfkkpxb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2yttadwmi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zmkclyue.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2nwxsfuqx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vjunrgti.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2mqarzmwb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2oimfkgvw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zscntbfi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qrsxjgiy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2uscvlzih.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ziqrsnlz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ewtsooty.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2oezwdwoc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pucfolbk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2wivjuwxy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2serfwjvl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qwrbmvtd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2gnvoewqw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dhhvgibf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2crxyssri.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2txgdttie.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2etuigeah.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2smctrxvw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2fxmfehhb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lzwyibji.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fttkskpt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qtobiyhg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zayowchz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2kpwatjxw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tpkasipk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lnynmmay.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2hvdhjgua.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bgnbcyzc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dfwbigis.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2bjwwlwvg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2iyencwow.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mnlgdxjf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2qzqtbkpv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mppvkgla.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2wbykoxzn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2awtsvqkk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2eokwsqrs.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2pmezxcqq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ecpalnnp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nnjvypnv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dlgvfszq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2iymndmmg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2yppybiqy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oezgukjc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2nplsscet.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iqsrocdy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2bdjtmudu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2nqpcgtdg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2uplbruet.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gznukcuz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jnbjwqri.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ppqbfxkz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ibumckaf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cvuivlmg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2kzorejeb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ygrahzvj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2whvxfslg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2svvbgfqo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ayawctgk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tudrjqav.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2dtzrroaq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2abntouoa.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ybewenvz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zznbwtil.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qhnmoykb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2udlyukvo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zhiiwoym.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2hnpqivnj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xuvsworw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2zlbflkvy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vmvkhxow.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjlkqxgl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2keffaxiv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vbrntoik.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qycyasoo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2megxrhkj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2tczdvotl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mexrcqoe.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxkokspe.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gpngiebi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2zvwsuqnv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ismdcugc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ddcxmfer.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wjsfgkoz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nobstyzf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2tsrjybqg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2sqydaztp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2dwhnlcyu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gefcftob.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2yyiltdgh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jmdiglhb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2cbfdewhl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mnffgqer.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rjjkexub.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2idrjmaze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wknaiqha.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vdosidua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cucxyztc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nkaetgxp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vnqntotf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2btwbonrt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2bjcbwyxg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wtmgtgpj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dhvpptil.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2gfkckmkx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xjtenazf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2rlbqubnr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2hptlqtsh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2adhmndoi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dxgvfmms.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tbkotntm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ypskvchx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dlzvzypg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uicvopad.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2dolsipbc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2wjyzbdkg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dgayhlvk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2lyupfccn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2vpvkmqqz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2hhxirwen.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ptxvxyjq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tdchecau.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vpfqmzys.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xcrywqxd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2tuytpuos.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zfkgplze.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2icggsqxq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gcxrlbwm.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2abbvyfac.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uqwulxrw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ceataklt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2urqaugoo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lxpjkqog.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ktqzrxay.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2arhoxblq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2xxsdkflf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2wyhzwwps.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2inbljyfx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pypsfcea.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2olnukocu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2itvaqaow.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2drnwsxur.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2zovlhqhv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2hlbesagb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ciyihvgy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zcgbqemg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xxnzemzn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2fqharrxw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2vyakddak.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ysekomou.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ykkkfnxi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2oevjnque.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ztwgbbwz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jidjtnmh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nysqhfoe.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2pcnliusa.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wfelsfoe.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nuebrrsx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xauluuge.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lbggkeiv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2smrqffum.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2glxkcisb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ytqnmswx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2cvxxcioi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2hzcahgzo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2vqcjyiss.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rwnrlxxh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xxinhbcb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2xgqobgdp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2eobnkdjl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bhzrwcvq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2mxnccmdc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jngyhduh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2pgpsdkus.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ejjabshc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yzobbadw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2pkemufrx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ympcpzsq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2thectrze.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2hevydasp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ivuzjzwu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gcahxwxv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nfmztket.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2pdioback.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ztyshphk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2mjwcgdaa.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qyquigeq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpzkclzh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2bprdqtmy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylbhwpdd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ygsfxscn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qyzqpnes.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2yihmsjnw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2rchshbyw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2vbixmrdh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2snvgytdk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gzbkswyx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2litrhnpo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bunyvhxa.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2erzuwyyp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2akwniplm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fusuorlc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rpvvjiji.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tevxtdnk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qchaomqp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dcuazsxm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uqudqvia.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dmokybws.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2trcslpip.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2cxeqyhxh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2emzyklmt.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nsgyonhg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wtchsygq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2cmqvxdyi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2iaurlyyr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2firsecbb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jxqojwyj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2yrmctdts.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2nnkdfykc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwfbuzzq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pylljtlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whtdbzqj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2spdzmbnu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2rwyxkyah.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2zaptbmoq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mmuuaogm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vxnpsnlr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2dkmqqcah.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zvvcozln.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2fjdupuoo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2tzrpywxd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ddbnhyag.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2lyvjhqfm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2kcxwhwuq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ybtmmnaj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2nrqbrkzq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2mwmplrgj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qrwvppqj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2znnljviv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bhyejtzd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2uqjgsxfp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2yvxwdjox.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2dthscycp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ojmqjhrd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2dtjbompe.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fprjiegd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2bljlrpan.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2hhtktbng.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ursmzcel.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2telgtdpd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2mactlval.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2whnmslws.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2syfxokac.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2twgomfrg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2hfssamup.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2xmvnmrnr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2uvmaxpzk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2brtjrees.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bwrfrqhj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zzkbvbbm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ylbfhhps.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2uyfbtpkx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2zsfofssz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qvflmzsr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2jbdczhad.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ddsbqbqb.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2enyzbbvm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2eryvfdiw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2tvjsvczg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tuyyxdxk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2uasfpxby.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2urunkwzt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2nkohencr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mwnlwsjb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2nhkuzwtl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2sloskjuc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hgmqivaq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2qgsirrde.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2cufxpdof.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2kknfrvoe.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2byldzxmc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2inhriyqg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2gvtppeia.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2dzdufurn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2orfjgvom.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xnyklzil.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2kfoswvbi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2yafasjpg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2suebdhvs.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2rvtevpcz.html


<!-- 参考信息 -->