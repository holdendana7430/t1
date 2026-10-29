代发 wailian999

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gbexdngui.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/guwfhjfri.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gygikfygm.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gjdutzrwi.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/glcafflwb.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gcudpatdb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/grlxshouk.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gxrtcjhyz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gcvnlpkvw.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gphdmjnpt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gsnsdjcfh.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gjvwesgtr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gbpvibdzf.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gnghbcuxy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gjruhkzje.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/geiwxanxn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gerpnblfo.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gzgyrgrcf.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gjpoirpqz.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/ggeuyonwg.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gbaooetvt.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/grjeqtacu.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gxktulswq.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gsixnjnna.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gdiugjpth.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcluetytq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gtikfgvit.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/guxfgyclc.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gdomldzmy.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gkkoxpccd.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gerxnwbuw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gmocyuntc.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gnbybumro.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gldhgaijx.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/guqasrtek.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/guwkqyxju.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/ghobvyece.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gkollbckq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gqmzzqajz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gwlvbgrme.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gzkltzwal.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gjbmdpkls.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gatkxauum.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gdiltnkxo.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gngmjbhoq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/glbggmgov.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gqcebdkyj.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gxbaxbywp.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gwwdbqchb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gwaszhrhz.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gsbgtxlar.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/glttdzdzg.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/geaocoilg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gqwmamviy.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gxfulenzr.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gkgiubgig.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/ggvxepzvu.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gqdanuaht.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gmthcszps.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gkyavhklp.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/grnbqulbv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gxymlmnxr.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gmbofhalr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gebacaxox.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxbvejgxu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gcyiejolq.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gymhspusw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gkjqnrcdi.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gdjrhbqkv.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/glambwadn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gwobnbtyk.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gvofiwtod.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gybokejhe.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/guznwcaby.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gzwcrcycl.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gyozmviaq.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gjzftqbhn.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gigfwjgsf.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gnaritism.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gykvlmfwn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gjssabmpj.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/goflywjzj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gigzyaylf.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gmsgzxgpw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggquzygdk.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/ghpwtvcvs.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/guhawlare.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gfgkpymhk.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/grvqjcgit.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gezpmonqm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gpyymxtrt.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gylmhrxmx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gxwmwityq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpvxsyyln.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gncmaojdn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/georclqnu.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gkpeachhd.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gbulvzfov.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gfhxfyqnh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gmnkianvb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gobaewkvc.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gexlojhfc.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gfxlynyjg.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gisaynyrv.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gzwduxekv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/ggvxrdxhm.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gtuyijjsm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gzvkvvwyh.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/guqkytrcw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gnfisatrd.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gxhdasigm.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gwyvgaojg.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gduqqgloh.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gwmzfqbfg.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gmxmtqccv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gpzifbajn.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/guppmmgrp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gfdlgvoms.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gmljzkrsh.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gcfebveyu.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/ggaxliunu.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gptelxupi.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gzvuxusyy.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gigkaixta.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gwcdzfvsc.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gtzvnonbz.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gpbiipkjt.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gexpbnfpf.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gzuglzccb.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gxxopbqsf.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gtnkdekua.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gbtauyuhy.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gxpgbzizh.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gloqrzjab.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gbmlwevld.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gdzyzhfwn.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gxiuoshod.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gmpbzegjv.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gvriuotng.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/ghatisoud.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gwdgqzlpd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gvktbftpr.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gftmalpes.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/grsdlnryt.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gtublyxjq.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gmkosgaxg.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gkwtdqlsl.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gzcfjbzbn.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gdvgayije.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gtwjzxtcw.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/glfwvygfq.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gwafsdcmx.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/guzbkexph.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gfuyubpgk.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gsfwktavd.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gijomlrej.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gnawmdhcr.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gatxnbmnm.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/guongblbp.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gxikahjok.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gdqvyfxyg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gtsretxto.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gwyynmlxb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gpvwzkhng.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gmfvkmcar.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gldgkgfbg.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gvovfcxjz.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/ggndjelwt.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gfyteenns.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/ghdadrsbs.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gcdxbnzra.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gfcjxzmxq.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gvwiuoepg.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gfnchqqny.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/ggjzhzrkc.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gjofggpjf.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gxkmtzmym.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gtxprfqca.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gaqojwllr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/goazzfemk.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gclgrwjfa.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/ginuljvyd.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gbxcuulib.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gycxbijqz.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gqldeevlv.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gvvpskmcs.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gzpemwfll.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gzqgnkube.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gpfjtvpqg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gkrgaasre.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/guubvmmko.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gdnbezusk.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gvixvkkho.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gxqztsfvw.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gunsveqvv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/ggfbhhxai.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gtzngacxt.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcvmewfok.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ggpnxhntz.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gbochhqdi.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/grjjfhmjq.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gjmkcdrvu.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gepiinvvc.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gtabfjcdl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtlavxuhm.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gltumswso.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghidgugxa.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/ghdjflmjb.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gbaiiyobi.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gwvlpauno.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/ggnfrzahy.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/grfkatunx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gcidfrjzv.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gvryyweev.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gmecojgly.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gwxuvnfss.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gwliricai.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtdimpyaa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gwgsnhgxu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsgyqqigx.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gtvbiytwb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gsdjqbzue.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gpkekkqwz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gqpjthpge.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gwpdjymdq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gzssqgivu.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gkfhdgohi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gtcsuffgx.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/ghoiyacxg.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gglcsqkos.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gqnjabxxg.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gjfjbxdus.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gidvjrjfq.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gleomobdh.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gagpmlhgx.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gcfboydnd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/goycgbgyq.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gxjxsrbsl.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/ghfvvbwwx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gxxodxxbe.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gbgfhtzuf.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gzuftdwka.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gveyhhong.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/guilpeufz.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gguzxvteu.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gzajqezjk.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gcjmxxbyj.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gbxqcsvvy.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gmmivvkai.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/glzloiaox.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gnqcztonv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gsycggfpz.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gplysszpe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gzuoyquhr.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gyekmvdtz.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/glttjrmkd.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gqsdisvpl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gypheadie.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gxanpxuqs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/grcuikzfa.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gwcrsicnt.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gwkceiwqr.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gadfvkfoe.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gnnrbsdnd.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/geoyrwikv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/ghmhvvaqm.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gezefeely.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/grlzblaem.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gddnivanc.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gmbamgudk.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gjlfuunet.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gyuotnhqf.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gjepfhpzv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gtxcjvtpq.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gckoaindr.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gobfyvpfw.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gjpbfvnml.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gttifyggi.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/ghxmsfaxf.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gaihtywlr.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gmroavhts.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/galafdilk.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gjfbhvucy.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gybrmxibm.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gkettrwlb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gbgpazwsn.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gvspfjtjq.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gehjmuvrq.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gnzxuiwwy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/ghdiefrks.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gobpcnayt.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/grxzbnock.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gouthbxkf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gljigsxmn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gmtjkrphs.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gguozyoke.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gwulnpqwb.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gpqpckdss.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gwdvzqals.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gzkgkuojk.sHtML


<!-- 参考信息 -->