代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hzhagkbv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3rxleancg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3zypmjevn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3pbgwasnv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wlzujgyd.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qnfelueg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3yecizskj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3khbyhwuw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3pntnfmqt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ynrogytw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uotazjvl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3iuuyqqrp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pqmcvgwd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3nilsslmb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ablbcgnn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3sbpdcfme.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3gnmiqgpa.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pldyneia.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3rqlqpfmg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3icdqewwb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3foecblfa.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3phwbjnrl.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3lvopufsf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3prvuhkoa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3klmgeuwr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3gdtiqpnr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3krvphbrt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ztikppjl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nbwvintp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wpwbrbdm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3cfusdefk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mtkfbjyd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3poncawfs.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3cuybhbdg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3yidfcrol.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wtbsnlrp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3rrpwyjho.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3deavffkv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mdihxvgb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bsekegxc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3oclboyey.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vblengzm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yysbfhmz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3vcsbrlhz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3adukzgtn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3imtufnry.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lllpcllo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oizpjjis.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zegcmqph.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wrvpljqx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3qbazgngx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fbmpzghy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3bxqvukqa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3woytorie.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wjymrjvj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3frwjubpg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bvdmtwxt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3uxptakqq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3cmnpnzxv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3edrqhpim.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cqvtpjfv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3eovzfhea.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3tfvjnhim.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3cuwbfnrc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3jsxweixf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ytmdpcpq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vurfndyg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3srlchhsj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3gxdkioeo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwibhnpw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3thusttja.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ubzxqcsl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3xfujsjsa.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3bexyqtga.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3dtbalckn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3mxjpdngv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xycgctjw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3vxhcknrl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3llnmplzf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3rbijirss.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewjvoihm.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nyidpgfh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3zwnclzgy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3udeimtgm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3vuzcmhop.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3natppokv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cyxjqdaw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3aueypdua.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3bihbxqre.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3faczqzic.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3eazcraaq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jmwakrxq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ukdewgxu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3owtoaajl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3hgpbppud.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3bntultgp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dbohlfmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cocrmhtf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3cuzbggoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cqhruxjd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vrsmpgbi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ywzmizco.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vlcuchim.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3flwizvpy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3oezlevgo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ogpjtvms.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3cdtxciof.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3euhjrvuw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hqxipybg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3njtetlis.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wbwnelpp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aycbktwg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zkmlrcyo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3galdmzfh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zisnmyxw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3eoyatebv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3pzjcsjvt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3meeqmkvt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mgwbaqhu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jkhfzbjg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3uktruqhp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lgnkcxxm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zrdpyvaz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxozfdht.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3cjcjrkau.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbddsemb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3pvkqrqvx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3osrsxrab.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3frwlpjjr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ipbvxmgm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jejdflwe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sewcqcqw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3qbizbcla.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3pnoahmyp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jpxrecjg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3owmjzeuh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hufygrgd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3uuunytjb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3evdxnysy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3uhtdgjey.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3javzvkdv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zrrwgbuq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lrtrmzdw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3stnrqruw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gxfzhylv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cqwgicpf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3fxieucdv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ecprmagr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3xmwxpvuc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dswuphmc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ychxyslz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3gqffprjs.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ahobbovd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3aksumsrv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3apbcours.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3krpplurn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3birvrwgj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jzqedhcr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ptkpvizl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3yeuguvtl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mkabbufn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kvjjmdzn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3hereclcw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ynqqaydp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3zibgcacd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ncbifekj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ggzsvcne.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ekpzvlpw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3lnkqbbxf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3plyftvjt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vwplhsgx.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3mtjvcbrp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3doxdenxj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3troucqhd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3awhzenhw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ymnvwrcl.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eabygymi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3fspurmbb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qmklphdp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3gaowoljg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ikjiifik.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nlippecx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3yueiarsl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ikduonbe.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nzbrpnyp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3qdbzcaik.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3pmnpnwnd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3sqseyqvn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zapvzfnd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3esnryire.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xradygew.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlbzebem.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vifaabsb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qqfydztk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ruvkkhlz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3hmejiwhq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zaredgtk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqtmzmor.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3phyhfojf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3nkynisek.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3rhokuvip.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fiughjkd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3smrijrys.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3znoeoxrs.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pzzbguxo.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xbpkluqj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wdtkjeex.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hrupagmy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3cohplsem.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kqpcrwwc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3finaokee.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3wwwskcdg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3secppygj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3galgfdrl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rxganrtk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3mimnqqtz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3atkxfslb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ewviyuvr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3iauoxznk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3mrojmilf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3pipjeoyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uycmxnji.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3syixrdmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdbtnshs.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3gtpofzwe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3nzfiwtmf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3tzjbnimo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iijxmmlu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3glfhpjex.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3flilvoma.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dchblrby.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3bbbynabc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3etcehrfm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xqsbuetb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3fkkpmukm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3txdgfccg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3relmmwff.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ljgnredw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ltmxjmha.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3jwvrkgmz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xujrqzqh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ydchzpil.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vagjjqts.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3phzenbwp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3tlknbytp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eulhxybr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3svhxddkv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3shxwxasq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3cxgtrvdo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3piuskigu.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vvzuclmp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zcjuziiw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3duklsncv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3molpqoht.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3iqmiezux.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3fdyubtvj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ojxcdxax.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3mvexppuv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3sttizlrl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ytzuoxzb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3uxmnlmtk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gcgrcdqr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rhkahmnn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3alxhpwqd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hslwoljn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3gwlylllq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hdjvazru.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3zsgpgkif.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3odylwifm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3npajvuvj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3dabvbpyf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xhrzqdsf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3gljbwugb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3bjiudaex.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3hrievpel.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ekwttovw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3mbvoyixj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3wrhhjyqa.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3kbsrbasc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3mtpvhiqf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3sxeienlx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ldkwmwin.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3jpcxmzkd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3grydskik.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3alvachqf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3rarcpyll.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ekypczao.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3glyobslc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3fkuqgcto.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3gmuqqfaw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3xicvkqdt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3mcblakqa.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ehymcefs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3vohegxrp.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3reucquzs.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mcxrczwi.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3xiqebcfz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3kowertug.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3rqtwcccm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3vimdwydr.html


<!-- 参考信息 -->