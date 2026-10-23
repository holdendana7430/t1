代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jbdhbcks.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ucifeqmi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3oudgmffj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3iqvtnfoj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ujckwvqb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3jrruxpfr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hkdruewa.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ydhonysj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3aqlwhaxi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gpklpupe.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hveyqwff.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3lltsgcpm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ojwwylmi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bswovqyf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ovgdqnbe.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ekczdobi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ctroanhe.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zttomjeh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3idromixb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jkmaoqwh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cevactgt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3pqdvtoqd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mlopahfy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lgvqfpsu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3qdbvknve.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3oatehfcc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ncfkvijl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3qzidczsq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3rjtbnfjd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3asgfhydo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3yvdangci.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3quhupcku.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3viblbrfz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3uzzuheal.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jczouout.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3twpdllwh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3llzkdwsa.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qdwckume.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3iohsnkes.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3irkoffde.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ktbqhoap.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3lnmksodv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3qvswfpgd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rgyzptrp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3bulrpdad.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmdqsryu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ngbajglz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3xwszntvi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3nettguiw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3mbmywmov.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rapouddv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zxqygrgl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3haysucyw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nmedumjr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3wcikkpsb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qidhwseq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jbumsnue.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ffqrrhem.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3scorxdro.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zhzlzrcn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3tohboyfh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lplqqtzm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3bhwznras.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nkqttgoj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vpcjtsvn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hlkbmutj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3muxuzhij.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3olsrwjen.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qkbzuiza.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kihabgxg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3xhbrubqr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3csddtzij.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yuqiimkg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3lreaquvu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qzrdzowp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3mpoicqcn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ettrdusv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3iotrsmbe.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3znavbyyd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lepjqfay.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3pxzjuuka.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rvjwcyfr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3beivqpbd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3apmllwmu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zulnehpi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cnkcbfmo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dkpjxwlm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3advymekl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxhxezdq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3npgsziyp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3opxcrkhg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3fmwozudh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3zcxenjgr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ayriigiq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bilbdghh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wmgnasln.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3lhdkummy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3rrsqqpdl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3muizrsil.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ddsvueon.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3auiszods.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dndpjzeb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ijdcacdf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hunhdvzv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lptgmgiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbyggijb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3lrhebznu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjmgqkpi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tgyzvltw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pyerissa.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ymhmsxdn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3kuyvhovz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3znddiypm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fqqecwzg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vaxrxdmb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3duebupcb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3auseuoal.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ifsaojmv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fqjrrovy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qgeqjhpp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hjtlphno.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vqhofmll.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ekjniyef.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vxkaxepm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cejgvfvs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3kbuebilo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3twrcbnre.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3qufjmpcx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3njkyoqbw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3cnnvuqjg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vyaefcqi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mydvxcua.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3kxncebfh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqtqqmkq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mejczgby.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ubvfzdbl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3iipzqmzu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ursjxwns.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yxnfdqqn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jhtznlzu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3zkjkcjgs.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3uuhgudzr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fmwvdzsn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3qnjbvkkq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3bunmecfr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ljqwfpiz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wrmqnrji.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oahdodko.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lktstxqu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3gkjrmubh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xpdzpnoa.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3eeqksrus.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dqlppmjz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xbfphrlt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3khfxqlve.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jwlzevnj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3iwarfauy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3iniefywg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3uzclxgxv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3zryxbaqy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3oggopsaj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3pfqxaxxm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bbstabau.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ldxwgwvf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3kzxioaus.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yrclsmpe.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3culuobhb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3crrijvbx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gtxlxwtr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uhomrazo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3pgtgepxr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3pkkxavxb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xolcurjb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3eokpijim.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3igjdlrqh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3mawphonp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hvdgacoy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3yahurpzl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ipolxsrd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zxmbomru.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cyxpncab.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3acmhboes.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jbovgtju.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3pokzcqvs.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3evkevcqc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vtfnabmq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3spcbzzlm.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3cfsehmqy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3umrtrjhm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kwpbypoi.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wviaiqbl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fmvvyqus.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kcsnwiat.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3urldygdy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ddnyhdwq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aabbqluq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3bndcxncw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3erkedqei.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3asslpoug.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfkigoly.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3asqssvqz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcumormu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3nsrwzdxf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3peseqyev.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tvhntyhi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqnnboot.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nlpnwmjl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3skaavzhx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxbfaswl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ubxqtzhf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rfoqzvpj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3iiemvwli.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fvxgdzlk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3izqpyxqv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ktudwukt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hmioinru.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3krefjtab.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jfbbujvw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3vpnbkvyj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3cgtiqvck.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3njweccjr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rrbraccx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3byakphbq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3pzorzbxa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ykoedsno.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jrbwpnno.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ttfyhdbx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3iafgkmcb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3rsrduave.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skdwoibp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gnvytzjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkfzlwpq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ibjeygbl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3nafojdvg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3muakcmhz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rephpcnk.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3sabwbmuj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3eyihzkxj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bmyemqed.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3zwqguaun.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3kjtodeum.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rprhyhrm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3bbsaibig.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3nbqfwsvc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3unmrhmcb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3eksisizl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3reyhffoh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ixyzzoym.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3cuwnvkai.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3gusyidqc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3khyidlyo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3rmfclrdo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3peanpxuk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ztrqwgrr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3uatsuoel.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fwldivcd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ifmahjjh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3njtevhlf.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3kixqeemq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ifwfxgos.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qtaqzmrn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3njfdlvfp.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3bptighzt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ieiyfcgo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3cnyxqmdf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3yttjcgbs.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3qnimfeay.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nzusiizz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3aggtytuf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ijbnjtqv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3lcwffewb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3gddmsgbe.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3vtstuawu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ciegfltd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3sjowamum.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3lnwpybtz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3nnhxhbgb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ufoejbgd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3lirtxqwd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xzzacvsc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3jufpwifp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3hdjsnxiw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3aiwgpcrv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3nivrjvtt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3kdtvyihw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3nqpprcrm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3rdjruwlc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ezednlee.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3jellzyah.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3huboyhgi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3oxmabvuw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3gmsdkvft.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3hhupvzdk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ndeaisyr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kctettfm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3igbvtamm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3qmuuzbxb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3sbbaehhb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3biskdcbm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qeqecgsq.html


<!-- 参考信息 -->