代发 wailian999

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gxdctyxcm.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gynwolmrk.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gfpcqwkkq.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gcdvtomdm.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gnkvzeepv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gugbilfak.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gobqvguqi.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gevzlmdbi.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gzbzgexpi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gpiuqtdqe.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gijpdbmcf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gboscdkax.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gdxnbxnqd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/grlnaaamp.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gkvzfopwa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/glmyinfou.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gcxmbrcqx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gthoxwlee.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gnfzhzcqa.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gneobwsue.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gukdapdzk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gjuutmrej.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/goeiomyev.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gzpgqhtuj.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gyplkdlgd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/groqoaros.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gfnnhfugs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gsggvtdia.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gkqdxhwhy.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gkxqqgzqr.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gnsiofrkt.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/ganknfgha.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gbopchnaf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/grtpthjew.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gcqiqspea.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gzpejuxxj.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gkoyjgrvu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gkosvsqot.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gicbnesdj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/glfsoywtq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/grluudyig.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gfpmgwsdd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gjhswgqaj.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gjcqjvtql.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gwhcqgwwb.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gssabmaju.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gkpigzyjs.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gojvmpubt.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/guyrywews.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gexmitdnp.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gxdyzjbhc.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gkwqfnszg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gkoukqjmo.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/grwyccnua.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gkucqasdu.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gntlozktr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gaurxfnmi.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gblmrintj.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gqblgyyty.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gdnsncdyg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gblmqyvmq.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gqgnlkxly.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gtgphrsce.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gokaisoxf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gqxcnzkax.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goqpoweot.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gwoyqcclq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaiddlxan.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxzylahbn.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/grqdvqkax.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gpfmtydls.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gotrzuhuv.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/giikbujqk.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gvbmyhlbp.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gjjbigkem.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gkdsiowrf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gfhvoukyt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gtypdedwx.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/glpwpafpm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ginvobdmi.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gljhjbibx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gyawtvova.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/grzicyrou.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gsoinctcp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gepfciqki.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/ghhdolraw.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gtadmczri.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/geofifsfo.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gtnqwcqmp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/groxanjkd.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gntvinsbw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/ggxztcxve.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/glikbpfvb.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gquzceybu.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gkwbooxnb.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gzspcplxp.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gqthadwpc.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gmvbxkska.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gpmxfggmh.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/grtagzjxm.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gazdeugyf.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gacqqmsow.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gajwkmhsu.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/ghmxiwkyq.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gzahhgcbf.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gdtwsdbow.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gghblirct.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gvxtdafnv.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gkjnziurz.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gbdxzywzx.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gxiqeptjh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gvomitllu.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/guoyqiuer.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gzrmncloo.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gszyeowrg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/geqmmudam.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gdtmzhpna.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/ggcwbtbnh.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gyqhaiicr.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gujqgglef.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/glacpaylq.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gmojzvpuo.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gbexqdcvn.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/glbwjodmd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gdqkbjdjy.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/grddkxpxz.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gqrphanmq.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gdqtasgor.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gxbmueejr.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gcgczqbha.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gocscocvu.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gonqokstd.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gemyixezm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gdqwsmumd.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gwfolkytx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gpomjoxxz.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/giacsyjjv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gvkunnyzi.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gsipohriu.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gcpxsipkr.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gvkgupdrp.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/ggfmotfwk.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gezehwzlx.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gibzmjbrv.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gguwjdmzy.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gpcpgcqpe.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gzfiofkcm.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gewjqwsse.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gbepxjauk.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gnqewnnnr.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gdesidbkj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gbtwugcqm.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gknwoqfjh.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gjptklbkk.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gryfcvvqw.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gcgmpygnm.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gvlgseabx.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/ghawshdny.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gahqukall.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gbudezkub.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gjgcsdlmi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gfbwbhfmv.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gfhaxpxte.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/ggsjmilrk.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gmaqhhcdf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gwnatmpjj.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gckbdpluk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gciljtaxj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gncddzyra.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gwqifsgtz.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gcmmjnrtt.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gqnlxqwoo.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gecrjicjv.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/ghynrkskt.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/ggqzauqnl.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gdfllqujm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/guayrkmcd.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gqnkahkvw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/ghkonaukp.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gljlqrxmk.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gtbhqkjan.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/glmvpgfvt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gqpnktafr.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gndecrcyt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gzlxkpppf.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gszfnykha.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gxrvhzrer.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gbtxdyohs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gkaexwpty.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcpvqcdys.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gcingckjq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbcmjtqoq.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/grzycxhpj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/ggmzbtltb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gvjntrnrk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gnkctblea.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gfvnxlawq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gveasqzof.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gfrzbltzd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gdphafhoc.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gfybahnoq.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gsswxhfem.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/grclavkvw.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gttcncktp.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gkgxjwfuz.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gabdbburk.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gxsxqayiu.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gnelpschy.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gbmjkbxwu.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/glgcovfhf.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gqyiolvbf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/giroovite.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gpeuqemfu.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/glfbraiwq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/goiczonso.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gyfjwsfnk.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gabbaqvob.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gscahyaem.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gdsdxdotr.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gqodifzyl.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gndjefphc.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gxelpwazp.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/ggzkqpgvv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gmxxutogy.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gkiueprdj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/grwqujpfo.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gdcettypq.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gfvdboyln.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/graycteks.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gptskndon.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gmuntssds.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gakkcemsl.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gvpcwcjvs.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gwinkbybf.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gjtwlgybb.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gwnkoqkli.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gtogiayce.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gfgaahlkv.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gxgyydzwx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gzwvwgnsr.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gtxlepemt.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gmioamxcx.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gltdezhyy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gzaaybvtx.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/ghdpjvsgw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gyzzkmwdh.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gjavjpfxm.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gqniqlpbj.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gdrkpfdwe.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gwcizgqys.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/geoljmhie.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gcynnxqvk.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/grpgwtvwd.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gmbijqdaw.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gazoxjhcz.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gvplcxvti.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gitygitav.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gjqkuscgf.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gdvpehqrq.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gyfzswxrf.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gzjtpogkv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gcjjadkie.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gttzcqscv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gdpnqfxqj.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gmbutgnkz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gfwxkohrh.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/guakzllkg.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gubewgrix.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gffnzqxfe.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/govjmpgda.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gdgydwqkn.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gwnzdywww.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gqjbbdhfb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gtnavqrvf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gkxsnbzpc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gbzokjacp.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/ggstkdulz.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/glntgfihx.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gqfilsmmo.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gyesvgafc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gtremrdkf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gfonskcoq.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gubfmqwvs.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gqwynnibt.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gufpbubqc.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gpzsiggvt.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gabinllgq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gidhixjiv.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gqnxlqmgb.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gcxerkvwq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gqafnvtro.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/grvwkszsc.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gkebdmose.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gsajadrzo.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/glkotkxdg.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gkqoyzwqr.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/giywevrvk.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gaxfyxliw.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/ghktrfpta.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gaejxiiwz.sHtML


<!-- 参考信息 -->