代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gtzwmltue.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gfbzpbmor.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gugklwmge.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gngnpqlcg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gxsxzulbd.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gwottdpfm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gcukfttli.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gmzhvwfcr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gxojwxstx.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gegaujbdq.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gczlqacdi.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/goroasuds.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/glhcgtryy.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gxhkweewx.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gcnixhvpr.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/guyqlcxrs.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gdndcsozw.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gcllsqwnu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gbaujjqia.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gdoaioclp.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gjeankeqj.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gpqoqlszr.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/goznqekie.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gumylntdb.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/ggerlonhg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gktdnqrhu.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/grflzgwdf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gcscuqaxj.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gdlrxlmfp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gxwlfvplp.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gdxhcoieq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gkctnwczl.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gfchvclwh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/grgosylhw.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gwvhmkqxp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/grszpptpm.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gouzmxgzc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gzulsnesk.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gjlkrhgdb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gtetepryq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gawbodpzy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/ghodubowp.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/guqkmhrcd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/grbeqxeis.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gyuioarki.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gbabtbjyf.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/guqgnbgln.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gjspssvmt.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gvdosdyrn.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/ghdeqrrnd.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gozdkdaim.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gwdhbkfzu.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/ggwamdsmj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/ggdzhqszw.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/grkplfgnp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gjmqwvdqb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gpihjcviv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gygfoeiin.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gaiizlalq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gtgkicgkp.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjamynqg.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gwopothve.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gxqpznbnp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gngjisosk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/goxsbcjeh.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gfpfqjtol.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gknmmfjqb.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/ggahficmh.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gqfvgprrr.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/grnnxukoe.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/ghtekxpki.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gpuxjvwwa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gwquhqmja.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gijzcoomc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gotqdawfs.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gcpzdgktc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwfxsuopi.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gcuxmtics.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gvfaatvbt.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gjojpvvjn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gwbheisjy.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gkwhmwnwj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gkxaavnid.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gzijmeygx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gzmstathj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtdgkmfrt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gtylxofht.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcrkljsfu.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/grrkbrvin.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gmqfjjyyu.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gpkzibrdz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gpzzqcyye.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gxoejmrxo.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gqureaxdw.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gpkrchqnf.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gwrwylhyg.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/geoncapbg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gdvarfduw.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gezxszkmb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gurduezna.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/ggkzluppp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gvmomvvky.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/givtymthf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gvbsvufqc.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/grsqftovr.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gptfgbbsu.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gaztqhfrl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gshkpzokv.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gpqbqqpjk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gavtlzzvs.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/geynfksaa.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gnxgqgxsy.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gtjalkhqe.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gkwqkntns.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gymzkauxk.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gzbacuaok.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gctjdbmlm.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gjbrfnlif.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gsgwfaanc.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gpvxdwmvu.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gegqnsdyn.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/godnlzquz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gjlbrpiwy.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gomxrytvr.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/goruyeztp.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gndojcuwk.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gfflxhqug.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkzgphar.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/galdowvet.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gnahpplcc.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gatluoula.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/ggnyxacuu.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gfmymugyh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gtnuldojg.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gyqvwetdc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gjtbrjisp.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gsjuzlprw.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gqhvvfbov.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gzmigemti.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gektjoack.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gatpqeivy.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/ghqjiomwc.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/grtnghpon.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gizgjmnoe.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/giuktjokf.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/grabeymcr.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gkrhcapzd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gbszlzykj.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/ggkbuwuim.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gdvcqxscp.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gzzdfxvkd.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gzevqbzga.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gtypjcsno.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gydsgydbx.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gwvlxqxqs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gunuiwbes.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gcskqzbsr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/ggbggimok.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gfndyildi.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/geholpqhq.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gpazlyziz.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gifhmgrfw.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gimqskdtj.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gunzhdbls.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gebdfhybo.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gbefwlrrw.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gizcyhwjw.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gqchrcguz.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gbfyszteg.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gxdcgqnns.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gsrhermga.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gtlnfmqks.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gekwlucxx.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gvnfgyflj.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gdgksvlau.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gztrdgxvu.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gkxhbzynz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gktsesrva.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gjdcyzkgx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/glubokvty.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gqpgwxcbh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gxcrgsrtj.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gdxlofswm.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gaijkjddc.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gqrmutyqk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gbbskiweu.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gdnblqntn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gsdsdljeb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/grydknrnd.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqfzkteul.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gedogbplv.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/grydlawca.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gmyqsxupv.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gjineumat.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/ghwbfxoow.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gyhdsgugj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gpzegnmuz.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gegufrqhu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gclkygxzk.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gwmjaglce.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gjsuaiedt.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/ghntpiald.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gvbltjpmt.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gwermfoqj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gffdbjfkw.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gvqfsuldq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/grurxhfug.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gdzziwfxv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gdnnpmohv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzroaznyh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gbssaerlb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfwssncuw.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gusjumczs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gnpgsdrfy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/ghhkmawpb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/getdyspow.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gygdrcfbf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gczgtjqsd.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gtwtkipow.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gflgltckb.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/grvamgcmd.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gpyzmjmdo.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gzhdvfcqk.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gxutshjtt.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/ggqqajnnn.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/ghrsgoszb.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/galpnchrf.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gptpdxavt.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gtcnddqzl.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gvawrsypz.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gxfxmzjfw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gydxuuyis.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gjaszmhva.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/grydgkghf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gxawgjgjx.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gpxqrffqr.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/grtsqppkl.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gpdnorvwa.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/ggnuorofj.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gsvlfhllr.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gjafgquxx.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/ghmoxcscq.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gjsnajaov.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gxplealfd.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gkjuyllge.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gxfkxvvhn.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gbquntqar.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gxmqfvtdy.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/glkxkbopk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gbkwwkhqp.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gmqkdupot.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gfjqgqudw.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/ggobnikvv.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gykfvbkaa.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gubqqcooj.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gkacbokdl.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gpcjfvznw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gsvribbhs.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gqagjokvj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/goqpemgma.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/guehexmxg.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gfevxinsi.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gsooedllv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/ggxdcyrii.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gybuitant.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gapzricbk.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gbyeafcaw.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gnxnoqoyp.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gagxhreqj.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gkawdglvr.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/godlzitzo.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/glhedbwjs.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gzoivuhbn.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gimqqjhnh.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gyffwjrzn.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/ghjddhfcy.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gpmlmsplo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gihrpisin.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gkxnhjrpt.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gfmmatirp.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gifjcourf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gceuhfdcr.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/ghgvzgltu.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gmnfzxwhp.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gutywvkku.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gaxcpeglf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gacianiea.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/ghapqfwwo.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/ghizdiyrm.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gzpddqxbw.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/ggmqdeace.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gqdkbhcvo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gybtgmevk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gwjxzcpgb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gyzaplqxp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gqifauvkv.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gzohojlln.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gilmgviei.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gfoursrxr.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gfrtxzbaf.sHtML


<!-- 参考信息 -->