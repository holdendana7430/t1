代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2dxtlqpgr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rknqjphy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ccjgeqin.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2cdeouvuz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gpkubljm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rvzzudgv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ldczepvt.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gjemcyjd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2rdtvnkus.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2skfqdgno.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lxqrpzyh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rpvmtazn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2igtncyvp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2fionbwqb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2smkrewfz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qioegwjp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2enykxfnx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2hzzxedmt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2agnfbjqf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xonjsotr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2eclfrgiq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2mrjpsyyi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dousbkyw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qmtzlleh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hlzkvflf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2alspwgjo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dwwmxzzj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2enrhther.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ftrzpmif.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2uvwfjzjk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2nwgezclc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2yyksnlke.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2lzotftgq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lzskcbmz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2vksldlgz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jfaudavc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2xlhdceyh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrxhcawt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mrgebkrc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jjfaludf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2refwbebl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rugmpvrx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2dwlpfeij.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2eerizdui.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qqzthrzx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rrjaspon.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2bgcjkmuo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2prgbpxbi.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2raqpnauj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rdgwvswq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2eguvxzlm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cxnzeqfa.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2cztbqiya.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2cvezlgta.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2vaqccico.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2hirkupfm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2docotiwk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2qyypemrr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2wmfktcfu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2lytmzhmb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ooopwfxv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2detcjmgv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2fkpetliu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jyoebcyz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2sjaufwvj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ulqjpghk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2jzfrgdfj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvdjmlsk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qrgapvva.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2rjxfknlg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sfulouta.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2eqazaqyk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vwwuuqaa.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2arpygdnt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2cgtgzehc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2wtplvqco.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ssdwiggk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yupexpyl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vydnayit.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2uwysjogh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zgegctqa.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2sovifzkv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hvjqjuel.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2arbgqbpg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hlshkibp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2aktxybiq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bdsntcxb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2oyadhkho.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ihrqnoum.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2mnxclvxa.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ttehuhho.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2otjjguyd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fbmwtsnu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mrgxavmu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2sipumxip.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2acodrdtq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wlcycjov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysaaskfj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jovcgtlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kowprurd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kuxzxdai.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wnmisamv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ivmofyoe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2cydahwzx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dqsmfptv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yhwylklj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ahvdhgiy.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2qeouguqz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2pudigoli.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2focisagk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tyrghtin.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vwxbezzm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rwmwhfzu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mdrzpiyc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nxeqpzke.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yfudocnw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2nhpuuyqr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ryzcueno.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xkfpblvl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2evllmezk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2owjgoklu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2tapppjbz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2fiyxfkpb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mydbzfdu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2tilqxzjm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwxtotwo.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2goynwgtk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jrlonxng.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2tmayokaf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jsbcorpz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fdwnofwc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pzvixkwk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ninnmhpn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2docurxqc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uradfeqy.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2xxbqrnjx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2scxjlrqh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2tmkyfexf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2efnkigvk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ipmsdakp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nddoggeo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vkrztswg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2edtxojpz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2eefbzvzl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2syttyeuy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2czqglkvp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2utcefwwj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sflsassh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2tjbewpuk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2tzqfeilc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2gikfcgyc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gjwytkev.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2lsttvsip.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2imertqvl.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ruyktsho.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2mncsiwhv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2bwrcnrzo.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2weonjomp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2mrrnzdfd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2yxutlkuo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pfcpdzeo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qyamqsuo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2lqjakxgq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rryimqdp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ctnosatu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ipyhkpjo.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2unvfamov.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2utdkmvzk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gnqgxvtz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2vmvbqsbg.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2npxllflh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2evpzbtxj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nbmxvocg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ctjnmpre.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pnaqsqsd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2geydbxmz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cpvptaaf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2urstqrqa.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qlpzbnhn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rgewsytl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zkquiwcp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2uojalzyo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2bglafoeb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hbotuuyv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gyoujepk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2svlnphjo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2mmvnhdgm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2rvpxnrqo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2zibvoxto.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2wnqlmkfk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2xjolgeem.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtcuitvs.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2vmmlpuhi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2efnzsbbk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2uvodkvyo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2xlxtdfuw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yhqjrgvz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zjoqrhhc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qsgqlpvb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2kwecquov.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mjkqbxrr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ujbwlwqg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2maxtvatz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ywnhtila.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2agftuikv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ungjxbra.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2eqsvrlhp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jdkiigvx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ooilxitd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aczagvhx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zxnqehxv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2krlntxkt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kurkeczh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kfruvmfl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fyczmvdf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qfpskxrm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2qhcdkxmr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zqhcmkfx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mbjixojl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mcdfwmwd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2hlltkxbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhnvkatz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nikpmxrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkmedbps.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qqmqxdfi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2castxhxz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2bgnvdeqq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2awmcxnhv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zlotkkro.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2bkqejgms.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2plsvquno.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2sdpkybhm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2lmhzapax.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2boslshld.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2troqrntc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2lynpzktg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2lsygxyrg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2thhclqjp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2hnvdstxg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2uyomvdcg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2wxrzmtzh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dkrrkmpw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ueydgpqr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2eyynxhdr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mufxuclu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2hnmhxwbi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2hxyhmeus.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2lipsqkff.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2velyyaxh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2lmdxdblt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bwkuydkg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ncpzyafz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2tjzrxrqu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2crduhbob.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2frmptirf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2lsobdhbv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ezagrokr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2dbxbjeyd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dtkpbenf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mwymjtfy.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2qymzssvs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2rzagzzhg.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2yeilziko.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2voccozrd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2qdhyevia.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2tkjpskst.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2corsvnsm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2gtsoeeqg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2fvtbhuyt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zjpyrpty.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2pghvjuna.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2suhuklzx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gpfbepjg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2klmcxedb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2gdheysdk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2qfrjkecy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2stgusxoz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2fxtoojrj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hevckobo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2stfznlgs.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2keczptpv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2klrsidvg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2udjxkxnq.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2embzfztd.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2yqtitlpj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2pwrtfqzy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yardxksq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2levvfyvx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2drlgtroh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ftnjyvrj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2uavcgsyi.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2jgsvgler.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2hncvhfmu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2jrmrzcuw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dghfrjba.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2nntwqxna.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2nuafkfcs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2htgophbk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2wnrobpbz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2tsrpmmbi.html


<!-- 参考信息 -->