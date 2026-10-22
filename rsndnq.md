代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xlrszruf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2bbyixtur.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2fmlzzkjn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2igwsqhwv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hwomatcf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zbpyapbe.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ufuegusy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2zwgulgvx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zunujxli.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bzfshlgf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2yvrzpdhx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2xnjkkjsz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2srqaqqhf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2sqydlvgl.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2vdqiqodh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jwxaucvd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2jvqsbfqx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bipusumd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xqfmmypv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2liviuodq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2dnnoifec.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uxtffvqu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2navococz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnsmkrtz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ntcskczc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tcjdmbdq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2adofhqdb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zcrzefeq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2nekrjamw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fjrgghiw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ogwabgqf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zptlbctq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lkxsxooq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kesxlexf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2kqyjltfo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ipeuliff.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2zupkcrrl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vqzmmrfz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2wmbjysbl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2typbpbvg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2grqwtflv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kvmxkxwl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dcsysvbd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2arvlhuas.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2usdaqpdj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2eomkntnt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pdqmpyag.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2fnvzzyto.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2juzffpkp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vehgcqzg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ktvxrntw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2nadsimve.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2jpiutshj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdsyewzi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ywuxwdac.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mnwghlzw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jzvupkcr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2uhlfpdzp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jpwifatq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2npceuich.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2zemafqsu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2uwktvfcg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ylbffrwy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2svqahjjw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ydxxtqdc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2piotcnqq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2bgdvtbjb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2hmldkpms.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2yikgyahm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2xodwwkuv.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2irdsvscm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ncztlpwh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xoskucbp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2totvpgup.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2juusyofw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fcdsgacq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2glyjhrpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwarhmta.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rzgthmhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgclazuy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vrplrchg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rzjztazo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2swxluttc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2vchnjxhd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2vjbfjwer.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vuqlaqon.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2tzakizpl.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hgkddhpc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2lncxymcd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2msmkmtyw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qbxoafrk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tdizpoea.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bapapxui.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2tcxtjuea.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vbeiljmj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2alulhisv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wcggbmpw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2cnlrghzp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2uoziribi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hicdvsyo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2laozctfw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2iujhstoz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2cstproql.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2grjsxusz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2oxdwonqk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2khwupsqb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mauygtco.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gfkowium.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2trtuhmwu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rxpzyyjl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wibgzbad.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hfcrbvwo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2eajooelp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ntszwjjq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wbtxmgqf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2xqyvndfq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2eivwayjo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ieqjalpt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2tssmrpmh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xytjbgff.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xmhduooy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2gduxasux.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2vibsiodm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xhflswyp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2xjlbqphi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pysayzcb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2wwqgsxim.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2laiedvft.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2uxrjpxuf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bcxpyrtn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2uulctdns.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jgxordra.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2mcibybbl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ikmufzkj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aavvkgjg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2skfdgwqe.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rnpmftyz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2bkupqfbx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2kkibpemw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2saozjqsz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qmgsptnm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tbkgmcwz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kuvxrkrg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2fdyiiaqm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2sbgwfbne.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2pqxfumsr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2kwfultej.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2igjwgwed.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ksrvehjd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2shlrksol.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2buvebjnd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2cyvkfwem.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2pxhprekp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2sccnhiuo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2oxrypihv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2flftmvno.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rklqqmaf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vkzzqvaw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2rbjzxrvd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2tjqymere.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aoemremq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2xjtzpqpr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2mhnhfduy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ikvguepp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2okjrxjwq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2wvuyxrda.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2sslzqzzs.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xowlfzlx.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2iwysybol.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tccfmumy.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2prwuuagj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fjiyzpzl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2bsmfqpdj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2aawqbmzl.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2iwjrijhg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2zpttkosa.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dhqytocs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2itlxpulb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2csbdhfnr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ukulookx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2fxdtfovf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xlsimrva.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dfdtdevq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qixkktmx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gmcdnrpf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wsinoxza.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2djbqwsbb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2feggboog.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jwdimgvv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tnfnxset.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lsujcanh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xizcrawp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jjkqpvve.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mykhdhfh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2llexrihn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2oqakzmxm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xchmpdpx.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2hiafxtko.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zhvuvulx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2rgbmvcov.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2xwgcwjuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmwrnxnh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ogazgpls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mlcvwimm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ulumwfhy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2pixvomku.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2zetmehht.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2nydwoxmr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zuiggxhb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2egtccpgd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2lqbpmuzv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2pqepxdbm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tyfuzqgj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ypmnrtup.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2lwvsomrs.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2uzhltnzu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2fpzumtnm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2fmbvtsbv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jsyhroxu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qgustrui.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zrjafsbz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2qppzaezj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ptntpdqn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2xrztwmio.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2bnnisqbh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pjejbqet.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2lddgpnhp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2rydgxpip.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xfjwrhzz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qzhmejam.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2togxvgab.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2honjybsb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2fnsikfck.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2gaixveuy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lieulehk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2pveuhgzg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2hphezhuo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2evolzzph.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2txcvvflf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uhtvmygp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2lacueaqh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2bxkwphtu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ictxslit.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ybmfqzrx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2vjnqfojw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2wsepmmdx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2aucabwce.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2tememtdl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rmvpbdus.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2jzhiwaxk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2drmxejbi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lnvcozor.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zmclvvxu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ilfnwayz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2kogublcd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2cvxkxhya.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ksnzjbbb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2gtjtyqhp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ytgthgib.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2rcokkiyk.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2pgrhfijy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ioycjqsk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2npilxtpy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jeevgutj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2vgmevbxs.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2apohutsh.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tolsvrvo.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tnqccjrg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2pjwtakcp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2xracnhpu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2eoskhxmn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ofisgbkt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ngsuuhps.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2jxfthate.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2uibfwwrv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2qqzvtwjq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2yeqhjnyf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2tjepwfdd.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2yvttlgoj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2zrrfescw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2tizqynid.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2jshcmwzq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2gdyeghms.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2yllvhndo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2rrhgqloo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2kserkwlm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2gnhxzxsq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2jvvuubtu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hpsgtook.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2uyxpvbjc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ssdtdwij.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2hfzwacxr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2puwmdwzw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2siexlzwx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2bjqqjpuo.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2jwquztmw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2nuclkbyz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2gbrqqahs.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gbaiifeq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ltkbkhlv.html


<!-- 参考信息 -->