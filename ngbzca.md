代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ccypxzqf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3vvqywniz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3dopiqtph.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3njvwfhco.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3tvvdcpzc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cqhsagac.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3vbwynweb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fkwijmss.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ljgzadhv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rynbjqkf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3xryamlzf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dtaydxpe.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3crmcsfjy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3xuvwmxgv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nnevofoo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3pcywtzpy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ahzobsnr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3yvdlmyec.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3fhvertij.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rsfrtbzj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3retqqmxc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3euxxqamt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hvnlbenz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3uyuplvvg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3mziwzwrg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3kakjypwk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hyuajwrc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3wxiyccrq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3alolqmyu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3whnrdqex.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wxjgcwac.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3tejrdbqw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ylkvovac.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ijrbatzk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3oqokugom.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3hkxkruqw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3dgluwrge.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cvpuvthb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zjyqldgf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ikoqsssp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ckmaropk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3azfeyibs.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3wrgndorc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3hdgnvzwb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3zchezgvv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jpidhfpj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wxxbjhmk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3jqgarfgb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3djhhkecz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tsnsnygk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3zfaubudq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wxxukrbg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3wvsznbyc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wsyexgdf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3wkunqkiz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ovoantfc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3geuobwqf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3toxebmia.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3olhmvwjv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3gtmvwlzr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jqsxgwlk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3siffoayx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qphdashn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qnyekojy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ylaveirq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tsoiwyhm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3dxatwlrv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohvdxukm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3iusctmlg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3qzrxlwdx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3zctzquqb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbqhbres.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3imldckuk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kdqzrzsz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fctpmlup.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3dowlywfu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vuqtvceh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3elxyxlvg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3wpdaezds.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3eyjpqrhc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bgcipxnz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ihkzhcrb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3yoewvxue.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3mudzcrtc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibwrjchb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3hzcjyftp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zojchllk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3nlfiasom.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3gygkgwbk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zulfwwyj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3mdleyztt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3pichuacj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fwoqcsoe.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3wftcisgf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ewfumnsy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3pqnfuwov.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mswdsjzp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ljwrszgc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3yvccukzg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fqlrxvvf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3elvdqsrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3naodvdaj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3fwwkinry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjfkkrkr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pcldykex.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lpmyebae.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gdcyuaho.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3cchyatau.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ujrssrxj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lyeuzuau.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3sjpwpjgt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3wwotmvwz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3auvzabso.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3homyxwvm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xlejshau.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bacbnzjb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bvigwvnq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3augrlepx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qtrcezqa.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uuhvydhl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3iomjtavz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3racbmbhz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3shxsufko.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3srysswpz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3hyivactn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3velhdwki.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3xshjqjcb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qznpeayy.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pclrezsk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqumxbpv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xqbnjjfu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hqgkeiub.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fqyesvgk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qqlbxkri.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dprjbrom.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jckvmuft.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3yruzwigu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hgefdiwv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gxkyrmbe.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3wjvssqcj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3skdiuppu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fcdbjjwz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ahhpxpjt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3wpxhqjew.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3agrzkbxn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3elsmeerh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3geidtvuv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mnoesqjs.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mltlvsln.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zqoxrnrf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mildkvtq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cmqvsrig.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3arktfnya.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3mwnwltqa.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3piqvhdbg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nqlbkzfu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3woomhrwc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3iuazzgsm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dxpdwhem.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ifsatlsl.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3txvutcrc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3kojzcatj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3kngylpgb.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mtpvpfdh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zbfbqdkh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3caqozwwd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qrggfhtq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ktpadwga.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3jvdtxzuc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3wszpktzp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wacdudtw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3kghfeszb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3lhdxuicm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3esvkbzvj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wsbtjztl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3mfifoktr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3eulxasau.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ryhounnc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ievwjntk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3yqqbemol.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zrcfnaka.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3rmsckfrb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qewolybm.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zinvkbld.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sgrgyuzy.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nzuermcv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3rjorrbzl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ttjiblqt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kldnsqwx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3tthkqqwj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ingbwgej.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3gyexlcjm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ldmnyjhf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ezneanac.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3rvfrkzqv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3azmdrtfg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3qumlipii.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3giuezrmb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xwtpquha.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3dfziwqae.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xfjrztun.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3beajhlec.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hlxovgpj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3kxagrsrf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghszvmhf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uoyorket.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tttylgml.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jzgpqkky.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3jurynnut.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fhgkzopp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wqlpozms.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hknnwltw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3umhffnqy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3aemdynox.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxumgwww.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3xzpnpqlv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3neojnlhg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3njvhlwak.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ejdnehgg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3biacpolc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jcsviipw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3vubghtbz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rgauimlt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ecnvttyc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3lmhymgmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfdpqmhp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ajzeeogl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnmfwuky.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3unowyeqw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3mvgtdoei.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jlebfxaw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ayhitbos.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wjmrkhjk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3qiipvxzy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bqhbhjxn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3cfgnkyla.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qybxycdd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wkuiwcci.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zpcudccz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3bwjjroxe.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mksxfkpm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ysyegumr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3bqdqgthg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3obqkgkhb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ooxppdcx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jumeikxl.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3bwhpizsl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3irmpodey.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qqgsxqzk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3usckyoec.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3nytcetbo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aaozqlvx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3dmpbfgmi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3awitnufp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3qpizgvru.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hswyupat.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3hndbkasq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3lnjmrjij.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3kfczazof.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3zxlbzlbr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3prmwzuqk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3uggmpzya.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3atvucahy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3sbsmztoe.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3qslvyoci.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3amgmfbbb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3drswqrmw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3qdwtgijq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3cceldvaw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3hypktywy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3gvsslsoy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rctwcfqx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3dfvvwbqm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ouxqxjpx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3uvolxpoi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3twlkkmbd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3lfgvbjql.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3qazyoytg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3dhkfdyxq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3rarrsgyc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3whuhtosz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3kqklnvjp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3xhkshozp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3aikjqvke.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3vbtvkyoo.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3yadwyztw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3lszjapzy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wuxqzzbm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3yxogojcs.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3qzyghepm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hmyqiwqs.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3vlbgsyfs.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3hklaxoeo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ajyoplzn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3relbvhrl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3lrvkpcvb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wcdlmwqg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wgdyrail.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3widmslsr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3kmenvlnv.html


<!-- 参考信息 -->