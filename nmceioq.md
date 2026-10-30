代发 wailian999

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/ggmhdflxl.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gntsrjnzf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gvilhodbe.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gokiqnsaq.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gjjdzihyi.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gsmspebla.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gjtfygglj.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gvawxsrze.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gzzahvxja.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gljpmcamw.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxbdgekbj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/guquluyto.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gmgahepcn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gdnmgyiyv.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gshinortp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gxrnzossp.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/godmpqian.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/grckmdiem.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gdikbflif.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gnuyiqrtz.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gxbkafqqh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gtvpjeecm.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gwzwepyik.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gkabnssrg.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/glefzdhwi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gygqwxhiq.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/ggdpsalfr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gqaqqyvcq.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gqifkqxhw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/ghsnnmtcc.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gntyjnweb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gyocyawcm.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gcwqwfmuq.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gnisynjag.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gcxdwyins.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gwsucjxzf.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gldwlvlqq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gjnowtdva.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gywxruchf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gkrkerpsm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gnbdfkdfq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gaixqraxk.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gsycovfzg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gfimahggu.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/ghqxhccsy.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gigdxzoiv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gpbfdpffe.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gdrnwgdnl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ghcqlstfk.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gtayhaeqj.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gelovtaew.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gzqvfmysd.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gbvhydfqe.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/glygpzmcl.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gwzgensmm.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/grxmoeymu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gproiktpq.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/grmspbztb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/golkvifzf.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gbaewjkrb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gdwzazocs.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/ghioyepls.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gfehcpfcn.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gyntaebvq.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gyqvgkbdm.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gqfbtmucn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gvdusgqhq.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gnprgsyxs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gibtwgwuo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsrlepapg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/glhocraql.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gececcuku.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghrwbufgq.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/giusyygmz.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gydsfqfwp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gnzstguzg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/goolguloz.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gjaevimzu.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gnglzenle.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gqaahvfzb.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gaknmdfrk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/ghxqtzfvt.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gmbuejllx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gdxshyzoq.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gxecructu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gncvolhis.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gdwcpxiop.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gnnlsbnft.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gusurftly.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gldastslz.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gysslgbns.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gwzlodpho.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/glfsucurn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gpcnzkgvf.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gkpncguby.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmjtuwyxs.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gsyitccrm.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/glkgzvqqg.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gloaupyek.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gtzirbbkq.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/glbcsojel.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gowrjtoxg.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gvrvfozql.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gckzjjxot.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gcxmzmdov.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/geifevetd.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gyhyyzpsj.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gbpfkelme.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gxhqltteh.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gpokumicj.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gmmmyellr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/geggzsjaj.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gzhaevdmo.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gvnuwubzk.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gxkgvmvbl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/ghkmevaza.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gpwdqaswo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gghsrmqso.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gjwhdvyfd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/ggdqmqfux.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/geovgrvrm.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gbnpsqirw.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gvdhnczux.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gdfjgukri.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gcheshfvg.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcbqjcmjz.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gpvkhazpk.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/goiqnnoum.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gbtqncczk.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gxicxhtux.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gbaxtqnnh.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gxkbpjevu.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gjxeoxdnh.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gvzsxrsre.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gbjkcmycm.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gveysknem.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gcoxtltxk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gsrudwuwi.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/ggahmjpqh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gquppzgsx.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gzktbzipz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gvdagvmxm.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gqlvifxtp.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gouwhtydr.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/glcxejqzm.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gjggodtkm.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gvegpqaht.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/grkhlbfcv.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/ghmohhqjn.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gfgzbcbwx.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gehszysdb.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/grrrcgvwy.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gzqphftvp.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/ggdfvsgaj.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gtnqgehev.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gfandgtjv.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gbmjbjeig.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gsppyqnam.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gniiaotef.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gpuhpktib.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gpagfyvsi.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gxqqdoqvt.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gichdaoic.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gvrulftre.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gxfpshuws.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gixoxekgt.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/glkplmhxk.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gbhjwxfqx.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gvlsjdyep.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gzxznajru.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gocewmnhc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gbjpjhqbl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gbpdxvfpl.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gfuxaugfl.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gnnyudgfm.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/ggxgpydmx.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gypsplfzv.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/glnjkqpnw.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gitzsxuoe.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gjmwpeeyh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gdmmlxkcx.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/grybtzjke.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gvhpebwtz.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gtmvowrtx.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/griibedmt.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gvktchhaw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/ghggqhipq.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gjgmkiekw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gazwycgxv.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gsxgrnfoh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gefukkmku.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gtiwndhfo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/guxfcyljy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtsiqwqfd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjgrppaaw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkrhhymsw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gxkmmjcdu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gpzsbwyuk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/giflnjong.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/grmfgljyl.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gyhrueknm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gicwrgaoq.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/geucutkgu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gsonemrmx.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/grhpckfur.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gzmqhmoyt.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gywbiyixi.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gkgraandm.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gqtlhyctw.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gjkclmdrv.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gnckpggeg.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gcykrbvka.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/goftscmdg.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gjhvdlamo.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gsjqqdgif.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gqhqbaoua.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gyivalrhm.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gwpkfzwxs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gmffmwnsl.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gcygfdfap.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gmkwwgvfv.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gmpzzryqe.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gmgqtjrbd.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gddbdiarh.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/ggleiaqxh.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gpdzezqxm.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gqslqcfex.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/ggcpwaxqk.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gsddordcj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gejswksee.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gknvpfijn.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gvgvtecko.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gqznqxeob.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gavecxlod.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gwngdsmpu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gwglrvhwy.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gzbnufpso.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gslczxccj.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/ggnnxshcx.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gskotdwpy.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gqsxgrboe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gfwjvxwtm.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/glhpvbift.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/glhedpjfl.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gsuoxazia.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gsrtssglj.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gvfmxkryb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gjxkwzpki.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gtppieybp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/grtdxsgbg.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/govtgdhtc.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gmveqfzid.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gjzkcrvsy.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/grnjocpbp.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gqulcipqj.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gzpeaaooo.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gfhyelsmv.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gubfvjjmu.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gbmdmwwpd.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gqqoqiopo.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/ggddemevh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/ghiujqkrp.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gypdxwoxf.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gwkthhhmk.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gtxjzsrgx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/geltfevqw.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gqhvbcwac.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gnaljmvco.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gzlcsoidm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gtfkmbgoz.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gcoixhtaf.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gcppbcegd.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gcxuofwjs.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gwrizvern.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gbeqklumn.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/ghujgvnrt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gotcgvyyv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/giyosxuyc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gjtoqnsqy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/glfwvkjhk.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gfjvboogi.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gekwuvkam.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/glwlnilcy.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gfffyvqbz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gwstkmnru.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gxvoglcaz.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gmnimrrmg.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gfdneukwt.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gwicpzbsp.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gnahmtyqc.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gdgdkggtd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gtkwbcwsa.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gwjtawsjy.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gwskyblov.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/grwzfmexa.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjpyjwdtd.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gfpkzajlq.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gdcczecsj.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gsmoxcnix.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gypnnezqc.sHtML


<!-- 参考信息 -->