代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3aqpsxovm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3xylnryco.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fyydojhi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mdxfkhzw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3rmunwetk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xshtdctq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xvboedap.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xrwhlxka.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3kzwkixii.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3djyjvsla.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3stafqtfy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hrwpykbc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3gxthwbgj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rdrzpesl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hwkfmskl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3rgblsdfv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mkzlakyv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ofszwnjq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3hxzfowta.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uwsqbkaw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3goxvlzbq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3gkmrpggl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3qxdpejge.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3skvfgoir.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hraxhsbc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qpipikto.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3citqdbll.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pghadmxz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3kwnjrbvq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3gbecodor.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ufsuggvk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3tgrwclpz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3amnjyojw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3zrzshdkm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ssmwlhzw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3naupuush.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kgrmlhvx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zbitrjwf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3cbbrsong.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3onadxnfx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3mogmjdgx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfjzjnev.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3uiqjekjg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3gihmygzy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3uypyhfhh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pjgmrvtp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3puogzvls.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wacsldhh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vfkfycdh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cvfueixh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kuekgnuo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rzvypqrk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3vrdwtzmy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ovyemqrg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3umhxqovo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3svjkthps.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mdpuppun.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3hfhpqxur.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3lxlcnnge.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dpknzdwc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3nlufqcrr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pnqghwho.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3jrszmknu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wimxxnuv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3vgvmlplg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rticlchp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3orqpqvrc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ctmxxyhx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kmhwynfr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3rptpdbho.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ynhylozv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hjndafde.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3nahnvfxm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3rcipznjj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tywgzyjf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qceolfsy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tgicqmec.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3umqxottg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ngyynqdh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3mnalcsbu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gxfkzjwu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cxhjkvqk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3yjxusrxz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3rdddxomb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrmjohqx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3zydxmtph.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3roaedqaq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3wvnozbak.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zkwdnoxv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3eavzbnge.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ranjchqa.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ztsgtegi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3tvmvancd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hxymchas.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3bdbvrgsw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ywuyrarl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ccaqawzr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3yngvvrzs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3apyxqnmc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tzemetbv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ebpyxmrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqyzcjez.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3cuxawhef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnhqvcwv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cprkcqyg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3spxtxxbc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nmmrjjnn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3zfdfvsop.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3hxypisfv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3oouzyuji.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3eteayrln.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ptrvvldr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3axmzxcaz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tdfkcftw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vtrphnol.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hhuviuqf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uvjtcsxr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3udpinwbe.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ftewinhs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xosyfntt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3iymqhzda.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3uegneeqy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3bxabkmuc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3zpovdxuy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3fbhgalyk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3owsonqmf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3yycyuuxj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3neglddrs.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fjbxqplg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bixuqkwv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3nrbypuwy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kxpkxryd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3qjfbrfii.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3mnedarga.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tcftgfvd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xmththmk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3gghhrxri.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3zoszvweu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hnzxljwb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3fqovidkj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rjacbxgy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3oclnbjen.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wxmtorbc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3rjscrlyi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ostnmxrm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3hcwslmju.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3zbphxoai.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3rtgasywt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3lwgyroef.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jbaqujca.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3byawelzz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mmwkopgv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3fvvskxpx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3muqpvvct.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gxmdxqor.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ufsoegzb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3nlglwejf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ggvpevxs.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bbvfffyy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3xnibqptg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tesiinyi.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ilmremqr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rexcaowx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pirwzryi.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gxoqceqp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3altolqmk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3shzarpxa.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3skamarza.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3aaffztgn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ntcrqwsq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3xnpdiccs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3vydojmyg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3pvcpznlj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3yqmkutrg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3jzdehcjl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3qglsjtgu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hbtzwvev.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3iwxvyxua.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pplxdkii.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3dewakalf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3oqwpqghq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3idunxzob.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3vnlzagcs.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jupwyhno.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mlrzbhcm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jnorktwb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jzxeemhn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3luwdnkga.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uqokaila.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3fbyktkgi.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3zpuodjzr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsbayhqo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bbmlpkxh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vtzqwlfm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3bgicmkyk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukzcfzfl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3gajmflif.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptobsxvr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ifgnrcpq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3dnahtcpw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dmqchaau.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kemruuch.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqfucejj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3kcwzjnal.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3yfzilehj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3frcbnbkf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sbztcmyl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3eniwxscr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3dvmlviyd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ebcglfim.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3whkwtfih.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dygyrtbd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qtspbrsu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rrlnxptp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ylssidoj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3kgvhemjl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zlzlglsz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3huaeaqtg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3isshwofc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3prcmyxyx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bgizsyat.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3kenvbvsp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3upjuffdn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xtdlwncc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3qfablffa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrvtuipw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bqkaqqxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vrlqtukn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ohnrgvox.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3olkipihd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ivnporpd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3yryfrspz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3zthnafaa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3sqimxtie.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vorbejef.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ekxfyooq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3miawufez.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pxkolgpf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3qpwwgngh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3xhxcebnx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3labufmtr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qgnioqgw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3mcjsrqau.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3niwyplmx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dkagfahl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kkjkbxvt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3yskverxv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3vefxzqcz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3lfaxnqkk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3iyswjckp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3brjheoqg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3utxqkjic.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ttqnczge.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3dnfrztse.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3kmphhfqq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hcmjjpkp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3arwgfpps.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bphnnhsw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3uliqgojm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hbsepmqf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3lxrtguvj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3lfdqdczx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fqammegs.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wnigktxv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3tvduopaj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3heuixsqh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3zclrgigm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3weueaycb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3rrdprhvp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3wlrxogkf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3kfjtjozl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3kxmfbeak.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3uxqoznwb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3buijlcbw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3iuykxrvs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nhwbocai.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3wwpzqakj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3kevcpfxe.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wqflqmuf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ctdrdgre.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3aqmxxyxv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3gqokqgsz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3tlzbovmp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3yziwpzyt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3drupsknu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3xtmwvrte.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lhhqddfl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cvccwnkv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3qrfnfpkd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3parocdkg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rxikosqx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3vqzujmxo.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3hudlxddj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3fmricoer.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ikmgrtnb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3xynpcpdv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3umrzbjwx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3pdnriitp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kogkgfly.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ybyiafyc.html


<!-- 参考信息 -->