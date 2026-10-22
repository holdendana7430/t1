代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2kzxsonwt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vkrdwafp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gzzfgieh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dwbmrwlh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lzislvws.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pehsmmmz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gdxubgkq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2pqhtgvgs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ynlrjgao.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2aehlttqh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2eviabzzv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xefetdeb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2irhtdrig.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2akzmrcch.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kvznjewe.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mhnlobpw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2gvzdupwv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2lbtraoxk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2deavhffg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2wqtpuadk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2eqoklkcm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ctbgnitw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lsfdexxt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wzompagp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2csjqjxbo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qjvlqiwl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2biyxrpxe.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vdhcvlih.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2kcpxpjtr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2idvnwkfs.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2eorkqfuu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2lnvodcuo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2olmadwgi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2uioehkbg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2puptwwxf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mchebuzu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ikjbzlwo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2shijazhj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vcspubox.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rjlsdymh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cxmzhtbi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2awkvrtja.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2pfdnkdgs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2juuylcrf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ivgsawcj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyicuuth.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sbkwjjbz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2lelojdps.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rrbzsrpv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2gyvngfxt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2chhcapjq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mksstlzf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2gopggene.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lfwnwvrx.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gatlzqho.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pizlqcub.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2nkzdjjlo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2faqxxwnq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2brbaqubs.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2sjilisci.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ckewtpwd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2acvjuajm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2zwcrzlcs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sstlrjis.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jxrihevo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2uwcnguas.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwowonft.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dmtiitlk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2entszpkl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lqgvyniv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2pwqoprnj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2olbzzzus.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rrttqswl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2kvxzlhwy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2dmfcnsot.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2prvrbqpy.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ahfhxpvm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2fjykzbcz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wlamcjel.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2zdcyuccs.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2jdzwxcoe.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyspdwri.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2gttkredr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xzahfeug.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tyicqbws.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2yuerwged.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wrtwhnat.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jfjwnyvz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2unsiagce.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zrouhbxs.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2nttapbvu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2dkbamven.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2miyhwqjs.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vkdzhahg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wrdafmel.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2pstajfqw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiyioact.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2fangmjcs.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yddnpbew.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2bjxrqxbl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bryztgmo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zrrfpgjv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2daywbjyc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gctbwskw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pyytcsgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eprddriw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tnfhhjok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjyuebsn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cdpairdk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mqyfumyw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ahqumkwn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gweicyml.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cyeqwtby.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rrmyyewy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ymzjwmee.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2fbryolhh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2vwzwrjan.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2mmnvbghp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zxugvzvb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tydemamf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kqbxdhdl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2mhhenqbt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2zffdyejd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ckemktbr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2zrpfcxbn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2wdntaiod.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2kjfnewtn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2jhkboypk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2uwddckno.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2utslojre.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2owtibbsn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2glvrrwbj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dvbgftzo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2rzzezquk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2qrdvgpjx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vbokzbrc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ekyipret.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gmfplvka.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sevlzxgp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rgbqwcex.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2jqmvrvhk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lerlkakw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rculmgkx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ccokvbac.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qewdkaqv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ozahhkhn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rpiykzhm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ormjvucn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ncuzhbwn.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2xpvorhgb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ewnxzhyd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2dghbeyta.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2radjnrpw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2maugstsk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2oaxpemnr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oktfmnqi.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2sobypjwy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xvbxobnx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2qwnkvnwb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hypfdubk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2pekowdgt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2nnvpvuyd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rfwkdkry.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2tdfthbfs.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rarkvket.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2epizxcyr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2onxrwtuf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2aefmmzxa.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ltyzctpm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qosfpzgw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vffeitlg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2iomhuznm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vhyfeccj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zhvnwzco.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2jgfvudbv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2qfftqnjz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2mdqsgqkt.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mrgjnuzr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fucqyrjc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2melgqilp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ywufiokm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hamyxree.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2eucnxoxd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2bersdpcq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ojomzguh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dnbufsjj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2fsrkbfwu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hdexpgxz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nexrhzpt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hubahask.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zekaggzg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fnsmgppy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hozwwqyl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nrhsxxyr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2bvcraywg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkuvaveo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2cdbahqfo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkmwwdcv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vpljdfak.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozjsfjgc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2nodnfdoj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qsipkrlr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ouriokvz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xaswdnky.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2geqgmxkf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2niauxmeh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jcqzgetw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2eghntwbt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsdpdyqo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fytlytka.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pttqlzin.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2agjmzwqu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2srlygrbe.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2howhixlu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qdxsuqxu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2baibokgr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2oxotradj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ogualfgz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ndpqjhdq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wzophhgr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2oxadcnso.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rhcitian.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hatxqiul.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2dagnqpnm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2legxxwrh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2cohdfals.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dylclhba.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mqltahuh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2nqhnawte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pycpebxd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dwzftqfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imlergem.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2sfnxidtp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2dxsyyrul.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2rxlgozzs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2yrdokjfx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jcothqcf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2bwpwxdnk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kpyeehvp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2lddydhhn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xiqntfto.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vrewdmut.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2leohanhy.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ggpxetgf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ygyxyyoi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wpfxtzca.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2pfasdrmf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ssmficwg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2uyvpfvan.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2gxpuhfpm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2rarvtnyn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2xbzzpcoz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2lkjqyjiw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2bkumzlzq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2htrsmvpt.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2gdbamcnf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2zzynonce.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2sxvjxiej.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2gsnxepjy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2olbsdrbg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2gupopkfw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qmmuljco.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2xqjuhfrp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2stgdfxjm.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2pxkyfpox.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2qaryjocc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ldmgdtra.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bfhwwllq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2wdpnbmqc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2jlcialzp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2wahqiqje.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2bgmqigby.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2feqytvem.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2gsvtfrhr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2jksbovwi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2mnhmvlfw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2zkwmbjge.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2lashfali.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2wchozrcs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mvuhzhcu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2abriphpi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ltzyaixb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2lrmkmrdn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2swrhabnv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2xgbjamdm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2gjqfufqq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2wpglrljr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2okrjwjrx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2igiowwlv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2vaexojrp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2wpioemlx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qnqzdsew.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2kgbabzkx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mdtfzofe.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2xfpqwosx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cmqhbcbu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2gpsqchkc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2kewflmvq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2pqhwewhd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2lubxgcrl.html


<!-- 参考信息 -->