代发 wailian999

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtoaieig.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gnsajpnic.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gtbssctrv.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gmwhdpfvh.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gvspjoluw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxisdiyri.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gfhebsjpz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsvbofna.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gijzrwzsh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyqwalco.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/guugganbt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvxdxeqc.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gfucwawap.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galtcvscm.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gurhjyjxi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gsmvdcvcu.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gaomvxzpu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gkorfxjoi.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gpiefmzsb.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gvapaajkp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gssbujltd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gxcewxbho.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gcxuqbmgx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhgjgxmr.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpfckqzzl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gtvxjjjyq.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuijlpou.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gipozzcty.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gtyaaqqvw.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gayykaoem.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdyxdbpo.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggylegcxh.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gumrnkvll.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gnmwtcbeo.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gufgzqlur.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gceukvmba.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaizgtsp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/glylcigwj.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gthfvkdtx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gsapuhjko.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpcazlyy.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gafxbodxq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gnsuqykge.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/glgwfrkuo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqilutqnj.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gltulxyuj.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gzmyemgvg.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/guwgydimf.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpicnnoq.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gxloowyte.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gymwpvgyx.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gqxndejkt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrxhnnfs.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gjiirrpas.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknknippn.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gtjdniuxp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyzkjdtom.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/ghwqvlwup.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gybxhxnxu.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzqmqaat.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnujwbys.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprayygzx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gndhqfhqo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/grbdtwebp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gabnkakyu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gijylwkao.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/glxkfiadf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guliqqwyk.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gucysudpu.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gdinmumuz.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gisfldohg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gwxedsirt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glimisqfh.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpahlzgpe.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gqsirqkwa.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gwchhoajj.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gwoydvbsk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzouogkly.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwzesydf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmusqmxwz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyiqmmdz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gginstfnk.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqluxuvw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcfqhmrk.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyfrbdbvb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypaapwni.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gkzcpqohi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnolzhsmp.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gyqmalwam.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdqgygsq.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gwffprbqo.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gkvpcrcnr.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/ghwztmvvx.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gogbmvzfn.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gapidwpmr.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gwmeblsgr.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojyclnty.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/glogkxxsy.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gacuupqou.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqxlkgdp.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/ghzhgncvo.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gfereexbd.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gnbourgcy.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gsmlxuetf.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuhusorn.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeunmzjy.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/goytfellc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gndvdukxr.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkhztccs.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gkagqwwhg.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gekxvuqwd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrigsych.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnwxuyekm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gipristru.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdarjssia.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/govksufyo.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gneijyrcw.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gvfpkczsv.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gzyqiqqdn.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkstshmq.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgumxfwt.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gdjztobof.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gamhmxsls.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/grvmogwmk.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/guowbmdca.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnevrfjsw.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gbygbsxya.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gduuodurf.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbehryuv.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gbwmjbegn.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gizsctqmr.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnzdkplv.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzksidxya.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxodhytb.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gcjnxsmhp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gsupryple.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gjouaxnhd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gbkzfgeeh.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/giifzqezq.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gyefihycb.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grypfxaqu.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gabbiokzy.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gljpnyqwg.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkqjtkvg.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjhkqjlq.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpekufok.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrdgzbwz.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdxlfrze.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqkcaexkd.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjzizfyc.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaqonvtb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gtvumktnk.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gboxgzzwi.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyurmidib.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvnddubn.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxyyqfdwc.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gqmecdvtg.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiblniqb.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gqkqixdjr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfqwiyyi.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqhkecfx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gezxhmknf.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gqnqqhnsl.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnutjnuhc.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/guhsjrbar.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsfpdqhvz.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsnlltrz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gtjsogolz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gujqcctem.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwblbnwkd.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/glrtgkwao.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvctcfli.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gyeebglad.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvgmnyyh.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gwggaahzh.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gzwjoxenn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gfadjqjne.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfuxkvik.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrcuuvvp.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gyguoamyg.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmmhcrnz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvbabopg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gckuhahmf.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghobkrlwl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/grsppfrzg.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdfpwgol.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnjwjegq.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtjluwof.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlmyrgbj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/goryejwhm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/glmkeutkk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gndnzxebt.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gprltjcjt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxumjdtq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcxuqzzs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxatytytp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpebwana.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gzefkqyjo.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyczwqbfp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gyispqjop.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gccckpgzq.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gtymwwebw.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gdeutiwsp.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuqdzbus.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitchdmlw.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghikuzaeb.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvokljcp.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gndbeykkq.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gwflordcd.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gtywzlqwl.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/ggobgvbza.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/givioobss.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/glirrwkyz.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gjeolvgyn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gffaiglpz.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gikdzeupl.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gnzflvayz.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gwqaemzwc.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gugmkzyqt.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqbvezem.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gcokmumjg.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjpubxac.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgottudz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gadwhdudn.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gfvlteazl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktlzbjdy.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgnebwiu.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gyseqnlmy.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/ghqzsakpx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gplxdmxvj.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/ganpuonlu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gepnaxeyf.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gaszuudot.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnnovtxf.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmufwqnox.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskwxgknx.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/geqmpsmpm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gbnbmpvtk.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gtajmhire.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibetmstc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjdzywjv.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwplrydkx.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gmobjkjkz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkctblnug.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnpoblxg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/ggvbdixlq.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gztxuxnak.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gsxczkynw.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekqvkpce.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gaioyoraa.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gkuuhwzsm.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/ggutxwfgy.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gbndgkfdm.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gsqmztffn.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqvoynol.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/ghuyumzxo.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/goijfrbsz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbikudzrb.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gussmwcam.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/ghhslcufg.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/giglrzcex.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gapcqwdhv.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/guwmstptv.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gxsmuoopy.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlmdqfos.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxqeugib.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnpmcdzt.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gylspgsle.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gasexzeyg.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gmbgczrom.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gjhznvjqm.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/guqulwwjv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gocfbctvz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/gchtsgshr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gilkzrjff.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gltsdcbec.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhzeffef.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjhtowmw.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gnelqonfv.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhnfimbh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gsxossnwv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeqgdgzs.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/grdmqbuwn.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gynklqylc.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuydbmvu.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrdibxmx.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gqjcxckiv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdllougux.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdxbuarg.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gtslujrws.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/glwzkvmjq.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtidxvcig.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gbefbulte.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/grhkcmzts.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjisghbh.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/grkmuimlh.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekowmddk.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/goorybjnf.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gsklynbkk.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gvmhlpusr.sHtML


<!-- 参考信息 -->