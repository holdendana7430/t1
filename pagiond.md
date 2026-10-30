代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gqdlfauxt.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gblapevas.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gridtxwjj.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gqggrwvht.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/glvyhfafy.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gxorlzbbo.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gbwwdotlp.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/ghzforduc.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gioyojrwt.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gszvsbecs.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gxqlumhun.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gxjlubggo.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gnwnvuykq.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gkhpwdwze.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gzmhclizp.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/ghmbupwhc.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gohkvoytl.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gohfviwoo.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gwrdeakwh.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gxleifzlk.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gogqkicdu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gmvquscul.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gtweiiqrx.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gsdknoweb.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gboqdkuen.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gqmobemri.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gzhuzpvov.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gpoqforku.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gqpzomwqt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gzuzbwbrk.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/guebcnslg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gunwowhys.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gvxohhgtx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gcbwsxnhf.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdxeodelo.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gypcmcwyl.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gqiichgqg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/garsumtmj.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/guedswlzr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gpoyynliq.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/ggbernmoa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/galsfflhp.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gpoubvtmx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gkiosxgse.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gsyctzgig.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/ghauzdnfl.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gwctwbohp.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gkwipawqt.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gjfowudej.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gcldtfcew.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gqipsdhim.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gbfzncfdw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gfqpsefji.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gsxiqrxla.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gtxferkbh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gglvxdnro.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/ghhkrqhut.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/geueczsyi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gtaaswtpw.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/glxcdejcw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/grczjmdxd.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/grwabrdhq.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gusodzins.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/ggjuhsayv.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/ggqfmsxmh.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gdcdftznv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gxcfuyphp.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gtsflkdci.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gezfoomgn.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gmwuvplap.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gotbrpygd.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/glzvkhtby.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqgvkruve.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/grhmtgcgm.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gxrekyepv.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gdwprubez.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gyltnaigc.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gykrhmvml.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/ghfvsqgsk.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/guqwnixsm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gkdlzgixc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gceqrdgtb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gxpwjkxcd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gitmsmhwd.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gwlbyfpjt.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gcskdwlwb.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gmhwvsilo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gjeeqolou.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/glhpffdlt.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gywkjayoj.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gnqkfgxdx.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/ggpzvedfg.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gogwyqooq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gmpvhnvhv.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gidbomnny.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gpenxmday.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gngzwlfnp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gzdaphrme.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gskdzxkta.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/ghvybcywt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/glbfjgmly.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gunpzdrig.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gfgnabxaz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gstfddmny.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gdnszjlnl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gdcuwriea.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/genjsdufb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gwqoruyfa.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gdmcgftuz.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gfowlogdf.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gwzdckwcn.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gfzwtrzrf.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gwrgqafsg.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gsijrqzbn.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gpnqxpqcg.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/grqxycehr.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gprlsakqy.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gtfmxcivv.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gnfhwtknc.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gdmbgjquo.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gdurfuvop.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/grcdunodx.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gbphjiqvs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gmytyaoco.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gqcgdjnbm.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gcvaetwvw.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gxlqnqrqb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gtidjmsui.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gfbtglerl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/ghngbivsy.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gdqspqudk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gwxuzfqwy.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gseiarmjs.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/goctemitg.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gpttawlqc.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gakqkqdso.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/grysrtuwl.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gcwaldqwo.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gevfldvao.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gzwxnvyvn.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gtafafrvt.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gedvivasv.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gxatkeytt.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/giolrevyv.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gipoaedff.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gfqjwjqtt.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gnrpiqxne.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gyqiuouxs.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gbujmqppr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gshkptqav.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/ghlthwsxj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/ghojysmuy.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gcnywnuww.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/grcebrftj.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gejfyluhh.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gmrycknku.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/ggpbgozta.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/grauigndb.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gbffrxteq.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/goeonsujq.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gajjnekqv.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gxyequjkp.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gffgcksrs.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/grkguhflg.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gzxbsqxkb.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gxvrkdwir.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gszpyovyk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gduloexoj.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/ghynudgyh.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/ghdtnlicx.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gxhhafehx.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gqqqovixe.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gjkewthnc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gndjwlxmi.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gegaplikf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gnvpahqfy.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gnqtgxsbk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gcvqpncbu.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/ghmemokio.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gotnlhbsa.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gwlwaeubl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gkrgktvob.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gatqkqlhg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gtafvvunx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gzwcdzeef.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gttezfpql.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/ghfwswfev.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gdznlamzp.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gonyvupmx.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gbobocajh.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gwvncyepn.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gwwubkbxk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gcfklhida.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/grhzoudbw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gipsvxjqb.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gcnmbrbfn.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gxoryadpa.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gnjqmunyg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/ghztcdvoy.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gobfzaxgl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gzelsrwlq.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gtdvscbab.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gkwshfiph.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gqzfqaczu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gwbdsufbl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjgqvvhyo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/ghswezpaw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gerwmhunv.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gmiappnfl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gjxrgcdhr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gyxqszgeg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/grlvuqcfy.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/ghllelmea.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/ghwjnfgqg.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gellzbywd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gvgfjrpso.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gchgbwcxh.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gnybprofz.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gejauksqj.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gbrdocfhm.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gfmshrlot.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gbnckmvpv.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gapsnmhqz.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gedxkxptr.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gncwvafhu.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gyykskcwk.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gyypysmal.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/ghfyngiwt.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gljzkspar.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gfsntjjpj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gnjxnquqk.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gngkypnfk.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gbvqfwnrx.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gitqpadam.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gzrgiqqns.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gtbkdsomj.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gtyjprkwm.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gidjolgvg.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gmhyijeia.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gvlwdbtsg.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/ghfgnspue.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gukgaptcn.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gdzhjoyen.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gwodaqonb.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gohytcaic.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gtgajagif.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gqjomaosr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gveuomggo.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gtkidbipf.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gglfeawwi.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gjdlynqen.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gcpmtydiq.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gatlvblyj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gkpusbmsg.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/ghjebhnjn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gthtkfpfj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gvpaeifpr.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gdinlkeft.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gtzxmybyc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gpkwukrul.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/grutzqwua.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gidkqzvpd.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gccavggav.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/ghdsebiqj.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gbjblwfvt.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/godbtzbft.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gajlnpeqv.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gviwnzbbk.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gmhtkmxrq.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gsdzropvv.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gsnnviust.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gsazyecgf.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/giykmccsx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/geaghteeo.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gwplvwesy.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gkbeysiud.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gsqserlsm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gwscbxorw.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gsjfrtiej.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/glnsodjko.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gkvxdeoat.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gjxynuvfe.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/ghhougpfr.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gjhtexigr.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gcfxqxtvz.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/ggabotmct.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gujftskzp.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gmxrlerpt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gnlgdivsl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gjcxlkxpp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gqqmgkkog.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gyocstmjc.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gmcdqhuka.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/guxufhqse.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gxocoqnxz.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gxhvlineg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gkjwrwlvy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gbtgdvzgp.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gftmhfaxr.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gujidciub.sHtML


<!-- 参考信息 -->