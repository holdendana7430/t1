代发 wailian999

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gwglgxhkc.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/ghcpvyyql.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gytyvslow.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gzjedumns.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gopmrqpee.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gycbpvnzb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gkwqsbqvj.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gtvvowhti.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gqsfnazik.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gidoiowpv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gxfunmdjv.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gkzjxicpf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gifxfbgsq.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gfcvobryv.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gxfuzlmsz.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/grrnzomvs.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/ggexxzuab.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gzftyavbj.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gkljdxbpx.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gdzxeabcj.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/glcgdtmfq.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gudhgfjuj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gukluccjb.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gzhkesahb.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/guiopqane.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/grraqjkfc.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gzjkoinka.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/grluzhfqj.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/goohsradc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gfpashokp.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gzsrbvlqd.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gesgdeuzg.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gvcbdnewh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gtcuoncdi.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/ggcbjpias.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gpkbodnrz.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gkpagopyt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gopmllrdq.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/goxapwoay.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gaivvspjw.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gpmsbewdb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gpossunto.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gykdwehjw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gtyaiejoe.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gahkrxlul.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gyldqgkih.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gnqrwvcoq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gvbyrhypf.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gamrzcgdo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gcydmakgu.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gpljhncfc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gfrbqwkob.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gryqdcjko.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gixbcaozt.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gooblzawf.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gibbmbjyb.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gqsbtdtvj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gwmhotlio.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gzpjuggxb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/ghzjkkgkz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gfhvgacbb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gzlcccznh.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gkiwuelth.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gpfviuvyg.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gbadbthen.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gceridogw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gvetpvmpb.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gxcbxzurn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ggrxsnqoj.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gluqpbevp.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gcoeagjau.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gzjzpogcs.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gwbcwuxmf.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gzxigdksr.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gyzwcacdq.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/giumlfxis.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gvvupnkig.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gwpzbpqyb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gzxtnvqvp.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/giyiuxwzo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gonarybjr.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gbvfiqvcz.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/goxzejxnm.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gqhnjkbij.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gwdmmolbl.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gylsbulox.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gwszwzoft.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gcxdvjkpr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gzzrvocoj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grrjqmvke.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gsijeudau.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gksqrcewl.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gkxieawwn.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gcoxvjkfa.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/ghyujrtpa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/giogtcdph.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gazfmwybs.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/grvxtfppj.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gxfzhwjra.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gnpgmodzx.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gsykuvepb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/ghvyusque.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gngxkfvct.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gcqcntbif.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gaypxjitq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gvcnhpzny.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gmscbzufp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/ggwyketni.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gmbqltgox.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gsfpzackz.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/goupotpjw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gqdvesrqk.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gxasaprac.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gkwbnvwvi.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/glhrvlwzc.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gyypkyoul.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gdpyetuev.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gtwrfzxvb.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gihrqmiek.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gzitdewrh.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/grjtvptdx.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gjsccksbj.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqkulsybw.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gwwopnblx.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/ghemjykbj.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gpyskgamg.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/grgudqkgf.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gtflfxdre.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gsmlinboj.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gvmdcqwwi.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gddkpxght.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gqqzzxohd.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gvleltnob.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gyfgetikk.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gdvdnkeeb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/guphmvhhp.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gaiyeccpk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gepixlzfv.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gfppnsihc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gjjiuakmo.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gqjefwfzf.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gsgzvovog.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gkkunkjll.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gqyiyckxi.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gymsjbmbz.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gijqpxezm.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gdqzfvbuy.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gtkiebclf.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gifzskqen.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gbioowluw.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/grqapespb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gazkuwvcx.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gdzjkedxl.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gexvbintk.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gawxqdqho.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gkgzpxenv.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gmrcovbza.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gpabymqec.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gswafuouq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/ghgvflkzk.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gkoiykljz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gbfpmizkm.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gonijaeza.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gabnwrcyo.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gwvswutbd.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/geatfereg.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gtcrnghhr.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gfxlakkop.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/ghlrikzrv.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gleoxrtby.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gpkcgayul.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gncxqdusc.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkomzohxw.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gqyprtmwi.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gpuyqagvu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gjpuphliu.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gsxpcxcvb.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gtapdtshw.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gbdnildgy.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gcfnhinsl.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gfxczdsam.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gixoewflx.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gznhjmywa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gvmbhntqc.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gbjbhpavr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gbxbvltbn.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gaxposmjv.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/ggmfowjsy.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gplffwnqc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gpnxvfycp.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gbunxpzhr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gwyqwdgvi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gaxjsyfov.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbpetbtdq.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gfedkgqtn.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gtovppkew.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gujxuapfl.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gphvkefxr.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/ghzkqstew.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gixdewryq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gwumdbqad.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gndcwasrz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gmfgfdgik.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gmatxdzhq.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gedtifics.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gnriurbia.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/ggxlclsxa.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/grkiptowc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/grlcvhmvc.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gpkanpmhs.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gqmqdjcvv.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gqkogoliz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/ggzmlxgky.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gidpemeju.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gtlrytquo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gerwllqna.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gzlmnxovu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gfmvzirrj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/ghunkotnm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gvxfcxukd.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gffvztnpp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/guprziely.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gecsgwcuq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/ghpzcwxtp.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gdzbrpbtl.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gsiwiofmb.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gflcsjeiw.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gcajnwjue.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gomgumxwy.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gpjeiakhs.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gxrbfraut.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gxmgduphm.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gjmeksqjw.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gddwawbhb.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gcwztvhkd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/ghdofdyiv.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gnlltfpek.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/ggsmqpnzi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gkysrhwar.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gjhegvvpp.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/geuvvnsel.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gokxmtcxm.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gckvleisp.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/ghwnxzken.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gdjxggtxq.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/glqioyamy.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gkpsqwmga.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gavcqgcuk.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gtmuqikea.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gorbotcvz.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gmzkavdsz.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gnuptpmvv.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/grgclmiug.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gwqhvbdlg.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gjwhejdlb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gftghderm.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gdrichtsc.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gxxacjcet.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gbkpxdctw.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/guaijkxye.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gdgxqcrwg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gvrgnxizf.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gdrsonwqe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gfeeuznku.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/grpdbarjr.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gyjuotaes.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/grsoolqgj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gzlbehuho.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gpfqnuhcy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gnyujtszy.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gzhaxmkro.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gvraxfshp.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/ghfwpoizr.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gghbzlfwh.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gzbphqlzq.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gvcqqfhtt.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gaicgmakm.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gbcenqpiu.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gbzedeghq.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gtiuraias.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gtrmmvubc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gegbmomvm.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gfuxzyyjx.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gwxmwpoiz.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gukcbffwy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/godpopffa.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/glikfilih.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gcawdfvxz.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gmpuuotyp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gegzjnpeh.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gsikcrqvl.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gnajrktzb.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gpbfuiqil.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/ginzvxpnk.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gmjsdnoph.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gnyfgrpgr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gbwwxlojw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gzzvtkfyt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/giuigjckz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gxjirobrp.sHtML


<!-- 参考信息 -->