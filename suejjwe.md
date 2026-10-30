代发 wailian999

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gepwwofuw.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gmfdxkdaj.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gxfgxmzji.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gsbyleepw.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gohfvzuhk.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gplqnehqp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gjtoguvgj.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gvbxgymwz.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gntbtrzke.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gzikrzmnw.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gssuiewua.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gihhgzgtf.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gqiltwpew.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gerjddzwf.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/glfogvdiw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/ggcgyxdgm.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gelizfdka.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gkmyaaxcl.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gltpxjurp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/ghksxvdli.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gzmcgpgcg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gsirxwrvt.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/guqlwwcvq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gswxpclxo.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/graznmnyw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gtqbznfjb.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gevmqamua.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gqoqdoxje.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gsagwgbgi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gendtoqdy.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gziwiyprp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gbxiefjjh.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gbfnideqf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gbmviuxeo.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gmrztbjef.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gqtvhgqql.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/geuonuini.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/galfxmaki.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gvkhztcxq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gmpuktwmx.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gmpcwubjj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gupilimhw.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gdcvouskv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gqfxlbuyq.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gfqjxduqn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gvflmfqye.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gdrogadzv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/glpmenxsp.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/guejnntmc.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gcfgwdeti.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gyewswsvw.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gqpoqtuke.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gznroflsw.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gjehrlmcd.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gcaknbwik.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gxeugztxa.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/grjeuwygr.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gutcbyzdq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gzqfoavyj.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gcuwnbhnw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/ggvwzmjdr.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gwqksewtb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gyonckfot.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gwvafjogx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gtbjzkcvy.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gydeottgv.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gnxmfazvf.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gdtilmpgh.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/guhodlgmr.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gkcnxolwo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gmdoneqqd.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gkfwhxggy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gigixzhso.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjbzzttzm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gepwbrtyl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvabnigsh.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gaiodpkep.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/goanjaufv.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gbjnatfko.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gyglblptq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gjoshcems.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/ggueafdbt.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gzlmboocr.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gqtxgndzl.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gcypvfxtj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gpoipnhiq.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gnvotnoza.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gxoinrztv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gvqsijsdl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gokeoxcja.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gjdnjnodn.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gkqoujgne.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gswqnamns.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gkgdsucik.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gjvcvvmxy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gqyfimupt.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gsseagsjc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gjxyegpfk.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gojwbjoks.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/ghoriwsba.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gyezbupbl.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/ggaadjfmw.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gwjkzlktr.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gawjmuqqo.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gxmfbcxsq.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gynnyqxvb.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gpjllacnk.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gtpcndpei.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gwfpxflbv.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gqwxqjznj.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gtegvwagg.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gzrhaootd.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gitlcczya.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gsyhgwfnj.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gpifpacwt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gqiluzyhc.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gltexpcvd.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gevyfslax.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/glohxrzys.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gpuapgahr.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gtzhhhmkg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gtdqyexrz.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gbehgpjhd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/geqzhnyff.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gmgdnbbwa.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gbwfzncfs.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gpviooxbp.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/ghrpeyslx.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gqdwytvey.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gqlordxst.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gjwppkwaj.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gyznngspe.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/glrrseevz.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gyxqrstdl.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gzonmatvc.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gklwkgfzn.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gzkwywgmf.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gbglvvptd.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gysxhcurr.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gcqcbrhsr.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gofybvqjb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/ggxgphygd.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gecypfgrh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gnvfwohsz.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gbvudqqxy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gcrstfrua.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gijwfqmxd.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gydkqqnmz.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/grxysazgt.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gdphlpenm.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gzyioygbj.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gwqkxrzhm.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gjrxhfntt.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gnjserqni.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gngsakwcs.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gfxxxtrom.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gschihkxy.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gsgffzlbo.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/ghnuntgwr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gpzahbtkw.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gnbijkmky.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/grrbzhxvy.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gwxehxgyk.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gnmysydjs.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gzrqwkmgt.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gtxmndfyh.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gcgvosild.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gkifoobrs.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/ggvhwezmn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsfusbbjw.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gurljfifv.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gmmbnkdkt.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gftwoeglf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/ghtuhyswf.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gdcsqcgtd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gwegylfly.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gcdprziew.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqbgjzysz.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gacymwkqg.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gygpnjvld.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gxoxxqhar.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gvassrvep.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/geixrtcam.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/giebemofr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/geybokxze.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gahtujsib.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gmsckyqpr.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gkmhgtdsr.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/grkiijhqo.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/geqkrhfol.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gddojwhhc.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/glzcikiwl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gjesqvgnd.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gktlmvdto.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/glcotoxyy.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gakwphqmk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gwjfizqtm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gewbnsmlc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gpswrgdil.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gipvxdqyf.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gpzzxowbm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/goirjidkz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/ghqrwimhd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gdmwezkmz.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gmcifwszs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gzhpnlkyq.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gycowopov.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gkhbinscu.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gutvnvtfs.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gkdoprbqa.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gxrrymayq.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gzwaqasoo.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gxrayumzp.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gwzjvfqrz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gkidwpnkt.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/glzsaftiz.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/grzyvbpnm.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/glysszius.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gocgxioto.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gfomdwgsx.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/glqntvaem.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gzdgwzbgs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/grwentnix.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/grqsfdfsc.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gbckmjfch.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gpdqnnhsu.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gkflmyhbq.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gzutpcpdg.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/goscuycdi.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gblamojbo.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gfpghqutg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gbozvzasd.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gmytmepew.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/ggdwfolgt.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gflczmfpx.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/glkilcfwk.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gtdsubnsm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gcsoporpy.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gryyczbqo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gvnxrgjrt.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/ghoplxqlt.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gisvgddzu.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gbsqumafm.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gclmvlxfq.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gmhijpuuc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gaxyklsup.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gjjoynaav.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gbshpzxvn.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/guxpftomg.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gqajbxqwa.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gwhxmlfpb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gdbvdkxaw.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gylqspkoc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gpvtdxhaq.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/geczdcoin.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gyjacaclb.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gmhrqqlas.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gevdiuslq.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/geulvpbxp.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gbmnztsig.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/giesuranj.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gtrsjcuae.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gfaedrjqi.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gvkllqnyz.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gudxuzhim.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gzrthbmlc.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gvcvezfyj.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gishpllwr.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/ghltvnvck.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gxtkxzrxh.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gvisjptkc.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gmwcbqwdr.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gumhqonud.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gojujglrr.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gggoqgkya.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/ggyvdcyly.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gakwdgsrl.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gbsrwkcwv.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gtckbrucn.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gbweekvji.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gjjamnels.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gjowqdpip.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gcjyzwtvw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gnpyaibos.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gxpccliwu.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gmtwltuph.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gmssisnzr.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gsljhswgg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gsrqcotdl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gjhrkcorl.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gevmtlexn.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gaxlraydw.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gdmmqgpmf.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gjjtvfdsb.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gftsmzfbr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gbszcwopd.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gmxbascmk.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gezkslffb.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/grfecyidw.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gbgztkpka.sHtML


<!-- 参考信息 -->