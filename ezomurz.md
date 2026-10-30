代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gtjwdzael.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwiehfcy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gupqfmgwi.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gbgtdtgaw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdyljpdu.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gduhpftlv.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcysvksz.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gpgxtpzrl.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjncgmjrg.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gsborvfou.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxtgofdd.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuesygta.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpextrceg.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnicpuder.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpcgogwi.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvycgmxk.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gootlvklq.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gclitdrzq.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/geubrfnut.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmdoroso.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gaixdauyq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glfsrfynv.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngzatowy.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gjrcldxvv.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gnyaiyeij.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsnwbfpg.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gwetzbdrh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/govhtffeo.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqkduoog.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagfpqicx.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giffmkxsf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gfdsfqafp.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqjdugdy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gorcvysrg.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgcxtxux.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfdptblh.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gidumgdfk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gprttchcl.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gnjbzzmer.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfxaksps.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gunicdahn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/glmwqkhvb.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghlgpeodb.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gfuqubijo.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/geikfhrkq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyxzwsct.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gcnnzvtzt.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqsasiwe.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gxtfvlpdm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeqyoimk.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gtrfavlxf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grhptltmm.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gxpyzzghs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjzitris.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulxbrkta.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gczoszosy.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gddmgxeqz.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyzogrgen.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gepeaoifw.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaauzfypt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gksdpbamj.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtwpeqqr.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gweyoebtk.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfdwjpgp.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyppwibaw.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gbycrwszt.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gsnqjftjr.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpbppdhi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gcelfgopn.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfqiuynl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrzzmimz.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjjxrgch.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijrjfnlx.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsymihojc.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gcjoalaab.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqyqjwga.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkescybc.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gqzyawmjg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkjqqojq.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gopsyrmcy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzffncxyj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpzjdxumt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gczxhmcbb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gacvtcjbt.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gsphuzaql.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrcjpalb.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvwmxgnpf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gjjusddfe.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/grobbkhdk.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/giuumhjkf.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gsewozkzv.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgmhjcpc.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gxubsxvsg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gisvubvsz.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/ggidmicsn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/grafjvjvl.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyuxhvwx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefdrnjbb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggamtpewb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgddlqgu.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfhrtetc.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gjtsjtbtu.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxwikjdm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/ggtnsluwa.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvfmahle.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gbdmdokvv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxyobagv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gwqjwbtnf.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gxvoqskpx.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/goiweiezb.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gowkyhmpt.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbobrasfg.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjvgpwqc.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwzpeuvo.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmnglxmvj.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gvkigdijq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduqwhwrd.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gsabcroji.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbywnwsg.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gewhghqre.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gygmfaxet.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/grwwsdfzg.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqmuuwjc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gtlgbwvlp.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gbvuntial.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gmqcvpocc.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbsitgwj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqvqvonn.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghybanhta.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavjolpzy.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/grsfegtkq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gljuvhjjo.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrelncbw.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxvtzmzu.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkmnhkwf.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gpxdhzbyy.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcqsowhr.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gapynoxwb.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpmhamtc.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkagicgob.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gogjkvzrx.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogtoiwet.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzvepgad.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gldilzxkh.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcjjvgco.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgrismty.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/goofytrjc.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gxlxwwoau.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtglsmmh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gdhbncewk.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gaerljdad.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiejhqhr.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gcnxivsxe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gdujiktul.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkeywwii.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/glhryawrh.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gpdlsskgu.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gnoreydbw.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/ggqzeclxm.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gnsltkdcv.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gbcmlupcf.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/grdzppyji.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gpktqnstt.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrjwzpua.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfjtvpdv.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbvvldrx.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnelndsx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfuzdrmw.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/grhmlwero.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gswuoqbwc.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghltfhwav.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtsbaikuo.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzalobev.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghgjemkef.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gavlopcvw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpdiaazcm.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gljxdmfat.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxaggbwa.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbdncgsc.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/grrbztjlo.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gykiqqwnz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzytjbjv.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrpayndo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gigffseii.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/giuipzoft.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcfqjvvo.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbghwglgf.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmanktaml.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoxjdbqe.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gbbbugpsd.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gqpzpkwqw.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gydszgiyi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gagstdnoa.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiewkjiq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gmucjuntg.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gwxikunzv.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwobkpcjr.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsszqltgo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gryfsdcag.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gbdhvokyy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdjdhcoe.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyonzjxi.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfowxgvu.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsyiorcg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqteonumq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrplzbjc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbckxgdaw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gijqreydx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomsewlbm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqmhzitd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbummenz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrkwltaq.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gikmtyxej.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwnfusza.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gojefyejs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/ghksisonb.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gcmunnqzp.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqconzjj.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gfhukpnkt.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/grtwfwphe.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoyxghup.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnthjatng.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gdzntgmvv.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geainootj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhthpvjl.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwkrwwjz.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyubzoil.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gitpgtubl.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godzvkxit.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gosibinnl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gxcozyipw.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gywgdhttq.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gixvgfkov.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwuojabk.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphxptkyb.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmsswprw.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gwvrnfjiv.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giepxyphd.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gnplvjffw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggndwlqyw.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gannezinp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/glgvrllom.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyvyrijl.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxvsbcyn.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/grjvwulwo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgeekfyk.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gslshldum.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gutaxpbae.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gmsqzjkxn.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gkppehwuj.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqxtljoe.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmuqimzy.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmpqpekw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadbdkcdj.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrapskii.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuinssjg.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gpxkwsfhw.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/ggllluxqk.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gbpfygbke.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gkijfufpo.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtywromw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gmkzhcwwo.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gidzaubvc.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/ghisgsxda.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvaivdpf.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgytsgzp.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/golfwfakb.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/ghqzckwbx.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzmovbfl.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/ghybzcsmc.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplprqfnm.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjqirwpw.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtkylwtg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gfjfvljyd.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/ghnrncris.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkugcgvi.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlvryraa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/ggpsqlnvc.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gaturcwyr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdjtwosj.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gwozoutpq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/guqafjwdy.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmbeoxjl.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxskmnwu.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/golgcwjhm.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gsmxydyaf.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/ggacmzsst.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamebtgie.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjyycsku.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbhhskep.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gdnxumuta.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqwrwxer.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaiwwsnr.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gkmcexqlh.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/guftpgipg.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gviiucicx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgfllydl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzxffyxb.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpebvbgoe.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gluhoszbv.sHtML


<!-- 参考信息 -->