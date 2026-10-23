代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rdhqfghv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3egzdkdat.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3azqgwzye.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3mywphvcg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3czragljs.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3womlgonx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jmwzhawh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nykldxex.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dreiickv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jghqkeqv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ebfizkse.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dslyfdtq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3badsmmkc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3nxerqqvp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rqzuwolb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3glnmadjt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nstrivou.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3zxffjzfn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3cszjudzu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wmgqsgxv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3qoksehut.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jxqxnqfl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3yhrppelj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3snbrwyfn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bxbzfvko.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rhuzwmbk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hmwcfnle.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3naboahlg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3onawijhw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3brkggnfb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ljksbdzb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3yyhuqckg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3pbxixjzt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3untersso.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gysqsldo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3usesfluo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3limkpzwn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bnbhxzqx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xtalhosl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dkghjpwp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xwhagrfg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhokwmyh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aubjwvkh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3emtinxnk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ousdqbmk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vblsqebt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wtqbjxwm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3jycikzmw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3aioelyti.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sbeevagp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3szdvoqci.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tcilqspc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3okteixer.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ixmkwxud.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vbcnwtja.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uovqnpkx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3sdvahyls.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ppgizzof.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ryhconvy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lufzppie.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3axcqlowz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3tomrvawz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3gqikewbn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xwrbmeqe.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3vapkchij.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wyqujkxa.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3xbbrcmrh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3eufxfgkw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ichqrmue.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3kympwtvt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3oewfpbeh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vivcrlcw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tmpvyqrp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3vpxxlxaq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kmejnjyf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3gmihvdwy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fviuhham.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kluwcczy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jgikolzd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3gmdkbzyk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kohiaest.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qtwgmkqh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3zxbhtmri.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3lhkakjcu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3kzewherh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xsridonf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3puzoovyd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3snxzbucp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jjqscqoq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ydnovfwv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3niprwonr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3pnkhpuvs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmwujgio.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jnigvdbb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qvchkyos.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rnkejuqt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vtbzqyeh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3lskkmjww.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3iwklxibx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jluujxcm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xzyssetm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyjpbbqc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bjjcpjor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqbjrmtu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rsywmtvn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xapcaczu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kgwfhewc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yhjyckda.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3xkxsaabi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xvngyqpq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fhhutstx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3syrpshxb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3cxanbgcj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3vbqkkwiy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ytxslfbe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mitkmpiq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zoikzfsk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dxblvdmp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3kvotasql.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3eobeuvbg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3hqxgkbuy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3avhkznbp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3eqcjsmcx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3mewhvckj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3gysxurgm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3sztiicxy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3prdtlrgt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kjzrxrdc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3keqgmuft.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rilxahod.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3kivlilsv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hbvxlbna.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fkdnuktm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3czccpabm.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ghcajvzz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3aqtywzra.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ycaoykej.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ofrgkbyk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rqfeqxwq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3lhecvhsf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3mkdcecdu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dbjqugxp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dcbvcttm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3tfmddkkj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3thcxltmt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3afngqgzj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ehkmhdll.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qffrypsw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3mfvtfovl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fnywilsh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3gsvkyzxq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cabdpbld.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3dfqmngau.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3idqzwtxi.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3arlsxbve.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ozxzcrlb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jaueewln.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3mwugbreg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pgjvfihc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3feysahfm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mtctidrc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3uzdpxmrl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3kzwpqipn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3plyirajr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wnlhxcpp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nvboswkc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3fgcvmfoo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vpulgcqf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3irksrbpz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mmiwwhab.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rdoaznhv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vyqqpxyz.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3txldshtb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fuebqxip.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nicoagbx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lxhwaygy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yrpvlflf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3zlqbaaki.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3qdgpkjbf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rxkhtxml.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3sxlrskbg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vncaxzwu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ahbsqfxz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3wamomapx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hyunxnvq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vuvyceab.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3moetuhmu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kkgeawgv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zegpdhhv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lugglqsp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ftvmflyl.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqkjzdlm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gtcubwua.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vilkisoj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3gjgfvoem.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3tqgvpoai.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3nouwbvcq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3mruzoqnh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3elqzcvoe.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3lsrurjtv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3davkisui.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bhvhbhtz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xqclrkuc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3obchxxhx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrxvpumn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wmxetalp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fiyvpmjw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3upjiyeuw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3zduhvhgv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nykvvhjr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3eugyhhav.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ztrwckoo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3bswbrjjo.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hjanyoeq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xlvbibmd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3llauxzhe.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lxyjgwpg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bziintgs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pfqvhnst.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3vzhifywu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3estotazk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3oiyqmpgr.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3irinlvag.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3glffgzak.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3jkblnqkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nerrsxrf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xukvvnjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zsgwomkg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3zkmkiuab.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3kmsbuyzm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3grxglimc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kqdttrxw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3swlduyno.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ujrwejfi.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3npqkvknu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3avdxkgiw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3vxwittgz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fvudxqdg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xcieonle.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ltxrymgn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3urrduvba.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ekponnyt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3znebwitk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3gpczibma.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ppcupnjk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3eafvqutd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wqjqdawy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3abopngfn.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dlaotxdd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3agcxzsqt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ryrtcbbq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3crndufye.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ygxpvbzt.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3wtzzrkkn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3xclffitx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3boukycwn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zohliqqh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3pezycbcy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3fbdeuyts.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3xrqosjoa.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3fdmmxfhi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jssunplw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3tsygxrym.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ptnblvmh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3blmolkaz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3xpapgzba.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gagybizt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3gypdoubh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3kecqquuo.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3dfwzinau.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3vdxwjgnz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3nhfekawu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3dkebusdk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3msnmuklz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3nozewtys.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cimwqeqt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3iwhdsztk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3kbpsihpq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3pkyzdwng.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3myoopzes.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3brirhvmt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3lscjxtsa.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3iuhudcxv.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xthttmgw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3txfvpuod.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3laujjetq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3luqihvry.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kwqegipd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3tcfnetvd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3qtpfmuax.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uvpcsahk.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3lgqjogna.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xzapmkdk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3uqfmhovo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3bxvkqfba.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3eztifvek.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qxmnrzwh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3getjwgyp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xcbprknj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ovsjidho.html


<!-- 参考信息 -->