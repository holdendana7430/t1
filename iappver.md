代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmucqmuvl.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gotcamomw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/grisxapjw.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gisylgcqf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmkkrfde.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/geoufpevf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghecgvkyv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/giubgqxfq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gitgcawsv.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gmbizqekb.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gbgftmfhz.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gbihcxfgx.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkytiptar.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gbzauybzp.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/geadsusip.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gggusmxsa.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gghacyhen.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfuuynnk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfkbbxam.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqxfgpde.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gvejwxjlw.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypuwvonk.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gzloigasc.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gsottuvvl.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gwpivpoaa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfaflzvi.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/glelsjbia.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gphrpkfwj.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gwokjilsv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshaisamb.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gmstrloyw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxwuizyvq.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gkczesuhu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvqyxwfh.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpxvzvsl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gfcwnwfcn.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbilqreb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrhhxyeu.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gbysqrajq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gltaosozj.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gckshgcql.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdvhtwnc.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejokpyil.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gxdoukitm.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/guegojcex.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gjqfgdntu.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesajtlxu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gflnhbrkt.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylupztdv.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gwafnthbx.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrgbvnmk.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glskuheab.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gearegrvp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdszriwwn.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsfipvse.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwkmhxrg.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gpvkrfwnd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjbvtisig.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoytcuau.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gtoglcadv.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gnkmrhhkb.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyolbfykq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmppdxyfv.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gglwaxqaz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gnwxvvpzc.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/grktwtmel.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumhxmylh.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gwetguhvw.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuypegbi.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/ghivltyoz.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gffdxivkx.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijcmkgaq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrdlgzrt.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gqhvztpin.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/ggmzqvqvo.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gwopnndwa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guarzjnru.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gncaqkirg.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrgiowmt.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gkeopfjad.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbupexuvg.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/guegxzdif.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmtlpomw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gftenlgze.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gyolyqplg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyebignt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmoiszha.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gotgnwegj.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gdvrxqeop.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gpumfdrkg.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdvjhbkeo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavuapnfh.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/glchfffrj.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxtbozjy.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gpdnwyczr.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/ggkfjupdu.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfzqxdar.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoddiqlp.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gshwlvlwy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gbfrlfcjl.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gvllzfwvs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gifjetahj.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbevputev.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gctzwbdtg.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghiqgsjwj.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlfpfjgq.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrwpolqd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gfmffrtgv.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gdbrnvwzr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gbrxkcsfh.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gzdjrevcb.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gskmqtbhq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grozcsnvj.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/grqvkxwky.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gzoxemscb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvrvrpbo.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/goodtgayh.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gzvikelqn.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexagaybs.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccqevlxk.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvkgjwxv.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gjfhnnkns.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gfabncjno.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gwxfositl.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gfbysexmv.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfsabtat.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gftsnjaah.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfvxvszm.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gvizyvoai.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbjoohpu.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/goxqzuoim.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/glpxwoitb.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfhsrexfg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsbtcreg.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujactkkw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gpsgbxrrv.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhurfmeh.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/grsaickyn.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gzcksvszu.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupflrlfv.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gokgwhkzr.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gzaphtalh.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gtdljqged.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gzwgxaqua.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/ggkxenqjj.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqsanqge.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmdvtcrw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevyplsll.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmwjpwze.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkqnkfqq.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgtoyhcu.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gusaptovq.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjeejnkp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozuirptn.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoyvpugb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryrjefju.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gafqikpkr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkmlvvsh.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsapaweng.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gppjoxtje.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwosvnfnl.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmxlpell.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/ggvzpfzzb.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmnkgoea.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gyxvyvioy.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpedmpyw.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gqgwxocak.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdqtfxfc.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/guxrzxuvj.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gjftntdov.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmhdzigc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/grpyoruew.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbephvhgd.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwxmcqwx.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gohixmwcb.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtcrmbwvi.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gyqebzvxz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gottgxess.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gnmyjryyy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnolajwu.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gpldbrejp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gllqmurnp.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhuqvdir.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyvoryhh.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszlaweat.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gckdrhldq.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gytupzher.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/grxhbqbnk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmguggjtl.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grgvnyine.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxrdrnlz.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrqkmkgq.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpipcqtvq.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzyzuyov.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqfvukkb.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gaxwzccrn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaziotulj.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/goqzvnguj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtnxkrxep.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gttbmhbsn.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgpsmtgo.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdcrzirf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gkswhlawi.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduiphlrh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxgzdjlx.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gzytyfojv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryzhrkff.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqnvfyxf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakdhlrxu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvzcnyci.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfhcejjlc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gerresgsk.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gkllxdokq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuhqqozr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/glcnmmfbf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ggdcaggqq.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjwbkuzl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gevxxefrv.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gjchcewbj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfogmycyz.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/grimgffgq.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxbyevfb.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnfjgikd.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/geuyzxcxp.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/guwiylfsi.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gkpjwlwon.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gobivgkco.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gktxqnapr.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gdxoukyfi.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/geexqyjcy.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gknojehow.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcxbaxqq.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymfcqafg.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsdngoii.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gteewymnu.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gqenywwzd.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsirwtyc.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhuzxogk.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqnvafud.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/ghncnmpnb.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gbonkdwhr.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaionefu.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqwjpfhn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gogoxnlvd.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gjxtppdzq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpmnyhxd.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gcryipyzd.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gckequhgv.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gcfqngdsz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gnpqgyhuy.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gkgmxmose.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtunmicz.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gbyxvxwlz.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gydubnicg.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaoaariv.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gvpzimwyn.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiullhfl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhalknqv.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gslafmszv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznpdebmb.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzpbabgk.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrxswnav.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gduoojwvo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gmakzilvb.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/ggyeuempe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gwbkymjbk.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gwcflonys.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwfovyng.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfaulkke.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/ghgyztsdq.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gegviftqu.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/glfnxowqc.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gzufrrsws.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgkwxgbk.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gzopjzfbc.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gygvtsock.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gysuztgsu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvbximgg.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gxydyeffw.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gqoxiyvjq.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvxzxzgp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/geiojnydl.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxymawru.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gwnojzpql.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclrtlyvb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gpioppjza.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gninbblvu.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gzgqtxwcx.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gegeppwri.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glruxgbpv.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpgclffi.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/ghbksyfbd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gvlqmdtpm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrleldqb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gegtkpbct.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gdmdwqkst.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxjvuohu.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyawvgwh.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gxlyxydyf.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkmmkmei.sHtML


<!-- 参考信息 -->