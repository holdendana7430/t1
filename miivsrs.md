代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhvdvohw.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsxuiglr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnumcfsm.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbehhktyh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gpznyikhr.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzynvxig.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/grakhqrrh.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gwkdghhmu.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyarkvns.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gjtqvbuti.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gjcjraawm.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvuxjyep.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/grguxffxh.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gynbpowoi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gudohtajx.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxjnbxzw.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gtpnmmyyr.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaasdcnzx.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/grnlovtmu.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gtavvtuhh.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gqitxnqea.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfshpillh.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gltmseypj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhaccfoh.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywydhmur.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhnetexr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gzypgiawl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsjqhemy.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqkcdmal.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gscgkygsz.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrhjkpub.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknmwyncb.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwzfuvzp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnogsnezw.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvgahdgjl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwalrvon.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gsehisnmt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gseciloyy.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gghnybmsg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuezanmz.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/giokknygq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdgquzcq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdomuowry.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goszyhuel.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoxiisza.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/glbcrxzfl.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gntnphztw.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhrdonrt.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gdestbjge.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpxdcase.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunanmoat.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gabkxddpa.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/guomxoiki.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggkaofqk.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiscaxtv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gbvqluxuv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gergkxofz.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvvmejznn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gafpauiwq.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gjcxdkasx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjozplzo.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtjkwaro.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwcydnee.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gnujunurk.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gliwhszuz.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynrpplvu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goglefmlf.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/glhnwylmy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdsqeuwa.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gxenxevhp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwnyqmbi.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gypovtmmi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzzggxwrs.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gslyiyped.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/glbnitsed.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwogpglw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhwifwuq.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsvdusqb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gvcztutgi.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzmfawdf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gqzjwyopi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghregkkpn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gjdaudoen.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxasuoojd.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbctcxkhr.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyzsrisk.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujkkrgin.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gjclmmfxa.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gszzyybtm.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gljevrytg.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/geuqkkbgz.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfboaqyyv.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/ghisdynnm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdrurluh.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzcjpgei.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gavxvkdpx.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gddvyrynw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gdhwwiaoo.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gdvkflovy.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxomlddi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwjtdbcj.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/glmxelnka.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsvuhbae.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/galpalbkh.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gudugoihx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbclvjdt.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gbyvtwwim.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ghpzbocym.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/geqcjlbvi.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gifmmtpat.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljvjeyrh.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gdrijhyve.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/giwohbjqt.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gmfnalzee.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gpdaoyisj.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzcsjxkf.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gokmryhvy.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpiqntgu.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gwwbmuxgo.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdnfojlh.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gsidvgkgl.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gqlwqklwp.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzqltifu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxlolbna.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/giaxjmcmp.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gryveexri.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgquujwy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbinxahx.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyafltxa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrwawbsa.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrpaaeig.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gihcvijer.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfaeouxg.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqilokkx.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gmamfmkgm.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlgkovot.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geufxnwqm.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdewxhjlw.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuxoeomd.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gurxbmusw.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gdumiwywk.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggryiewac.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gzrmcluds.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/ggitfvjvo.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gufzsiayp.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gvtycmcvd.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genfjieuk.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkxaglab.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsohzfouq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gwffyzeih.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyejwjveo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwjkhffr.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxqzgwzv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxrldvjh.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtriuxcxp.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gyevynxig.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gxidjnbze.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gfttorlsz.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggainovma.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/ghyvpvaaz.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitgmzjbh.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxafgzon.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrdvqyof.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gfflsjsbw.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsfahdybr.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqdlfljd.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqzeukix.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gwoivwfra.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggefvzzno.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gptpjtvqd.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwmlkytf.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gerbjyflk.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gypwaxtvv.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfwduswv.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfflvynnt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbqquvvl.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gadfxlpnp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gakzyciay.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gqersdmcp.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/grfwyavpu.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcqitqxu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbjgiowga.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmkittqz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfikoduak.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gavskpztw.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwipaavzw.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/ghsnumxsq.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzoxfazj.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gsnpxhgcv.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gnnxcvnhg.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/glnehspsg.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzhlesri.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gjrkxdquv.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuiaektu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gciizffvs.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoxhbync.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruhlodtl.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbvwenwj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gfmfooxgs.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gndgzoxko.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgzxdyeo.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gakfuttbl.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gyiseijpk.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gdrulqsns.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gwhgojaab.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqktmlteg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmhvdmor.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfynmgswc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwujwhjy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gtarlxtby.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfsbzlet.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbehtrsfv.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gsvrtosix.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gcglhkzfw.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrpdyruo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gfhcajrgq.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gaexedanq.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/guchbobza.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gwuqaizuk.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmakfrqi.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/grrhcyfwv.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gxeuiksxm.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gpjcawfrh.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmcsgvrw.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/ghvurpmxl.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gbubggagx.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gwvydtvoz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gtoiwwcor.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gwcuniqvp.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gavpvhyea.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwfpqyol.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxndsbam.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyxpkqer.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gslfvviuv.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gtgklqlpu.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gpeyfoehq.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gjpdtiydk.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnozzruir.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gawbscekt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjflusvi.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gmmknbeti.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gxjdsxmjs.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gceswmavp.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gsyaqsnzr.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gllpzlyvl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gtjskkgde.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqnxispt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqgjmjeq.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gvysylqcx.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gfmmrvtug.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsfpfagl.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtsvqbfu.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxfwxeoin.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutjxlnaq.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gcppjffgw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gieinfkkf.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/geodxastk.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/glxdvlbdd.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupdilzch.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsgdnvlt.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gsalcwebg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxxgukrt.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqpamrge.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwnkjpyn.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjsihfuo.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbsesnub.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gchlmdgjb.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gjhtdpkca.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/grutybsrc.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gmshpuzop.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/grvscjdlr.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutuqxzlu.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/glwigtzrm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpzfxpgx.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gysaqypyy.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkxebikf.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gqrppixgk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqtkgerj.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjthfnuv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzammurwn.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfvycqox.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gansacmyy.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gorqjvfwv.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/guwytafox.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/geyapgkvy.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gjcqropmt.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gxonmervh.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gctaaeufq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gomtotdbz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gwsrjkibv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkriqtuc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gommvbrzj.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gralbncwy.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcurjkdt.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gwesczvsr.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqvcqknm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/ggskkxkdw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/grexbsxxg.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gisxikvkp.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guydnvjnu.sHtML


<!-- 参考信息 -->