代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dznedtpj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3rdqrjlbu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3mhxawtcd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jxjplyyr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3glowfvls.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3eqplvxkm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nozqrovo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3bzdrtpdk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cldooxaa.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qdbzaqcs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ixdfrfqi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3wakijrge.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mkfpqnqt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zdtfhpuy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3apxkdmem.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zapjzhmj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3mqaljfyo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkrisihg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3manpxqsm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3abslbgdl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3awtyxvkh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ujgishgh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3sezdfwuh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrmmbssp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xlczalsu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pglylbfs.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3nixjmmjx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xqunhszd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hwxyzteu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3pdibekhr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3rmvlhqbs.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3boxpojwd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3sllcuogj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qrimjyie.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ooqohwnr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pliychak.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3brrwozdv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zyxfnwdw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3enubtnmy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3afzmpvgw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3iqosjiti.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wzirjrub.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3irdccmpg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrjwqdln.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vvynjwik.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3yfffswof.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3kznfkxgb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dawejtnf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ooeftkly.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dsgpcfbm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3myqknxzj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ylzqjiub.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ebbplibs.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zsoxvaiq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3nxytfakq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3drkfqgmr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rqybaknb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mctlsjfl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dufsbuto.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3rlanhdei.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3eotamwck.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3kesdeuqa.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mqfxnunp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3zwoyqunu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ptwswtpt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3qblruyln.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3utqvrxbo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3bncjbxyq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3yayegjuu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3zxnlnyiw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wdkrbomw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mtesvfpm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3faqwslbo.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3pervddrz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3dwnnjcbb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3blqxttbv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3obdcthuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dcqydfho.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3frxunkwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrzfpqix.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yqhdzyuj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qzbgvaar.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ivdhwztf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3frwcblmo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mhjkzzry.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3eciredpg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3kjjhrrsb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ulnfiewu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3yhbctycx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3verinmxm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ehwnamja.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xgceummo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ptingspd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3gucdnror.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hnfmefzt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3zqlggfqf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3notqtufi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jowtqalx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3shvcwzbr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ozowuvts.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3mbbsheyt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hfsbisjt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3stdeubyj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pcnruzqi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qhqweqiv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3oneczrxs.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3kgfxerhi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ubaiaqew.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3plimmjxi.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kjhryaub.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xhtzrgxf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3apctfaxf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3wggvicvr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3drshbzfd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kkchzulz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rlxeusee.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jsgywwbc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3vqabknvi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3kwxxepgg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3fjrpnkdw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3mnmtqcfr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ytehamvc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rcbkrrpo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ebjmrerr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xybmojxj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3exrdnwug.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3uqynjcei.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cczvebam.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3nhuwgngo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ucrrnfij.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3cexqwkos.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3fkxentvs.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3oqayifxv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ywpiizgb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dqfowwwg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3usfgusgd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3votgdlzw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3sllipupt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3anmviumq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3dopmjnxq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tmytuemu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3klnypuxe.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lyvjqaar.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rrkvilhj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bhejxgqu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3dkizpzmq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3elcwgxno.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3tgdippzd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3asnmakfo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pucwtmeo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3azyqeban.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3vwvkcdqf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kgibfefg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3nihmrezw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hlcusjjh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qhhbrjio.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bbskwlym.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tnduimhn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3deuujolw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ryethnal.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yxvapkgs.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3gpagjqlm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kpjwgrdn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cpkycomo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gilniyxd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3uaftgegg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xsjhwdnu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3eyclghto.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3npbvmdzz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3fukpmwvi.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3adnpjcwy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ckswmqff.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tdirmubn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmanwfus.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ggzsucev.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yqcwdscl.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zxubrxtf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bztvlruh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3etnredue.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3oqshldbi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3auaomkyd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pejfbhez.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3afvhlrav.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3zcavbkvn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ddnpqimg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kddjyooy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3stjzzcbr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tzdsonza.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gcjzvgwx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3thvqpukh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kfcnkjya.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3cufczery.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3patgbjqs.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ufcfxyju.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tkvnapkz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3wluslfpk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3udmatknx.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3whlmueli.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3haxmldbu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3qtokazql.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3dctvbaaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejtvihpq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qhkwrdvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihcurwsb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3fmaocvsb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3hmaagovs.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3zubhtplm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3olyqzexr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3dmnflzrw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3pxkllhjb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3kioyzukd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3qxfksxkk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3cznvwedr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hdrisjza.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3oytntxgx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3kohooucm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ufiogfif.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3tjgtdklg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3nztrzjmp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3mnllyitk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3sjhndrpe.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3whoggodk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3hhadwmxu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3uznaaxrk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xlxdchfq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xcatbnax.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3zadbjhbr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xsmnohkf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3erxuclcf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3tztlgkaz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3xbcmbsmt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fowxmnpy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3vflbmsgo.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3egcwpgzl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jbmjrhfe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rcavkkqo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ajtbeabi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3gzcqfsgi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3obafcafk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zmlzwgfk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xdakammx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gbjwuigx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pmrirfqw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ndaurloi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3yvtvvxro.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3mnvejcdi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3nxvocoke.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3fezvxbbj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jsuolvdi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3sbawsgov.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3yecxyncy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qpxrrxpl.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3twcahhtp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3alpswgdk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nfzxvkpv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3obcyqpaf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3svtlnuew.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3kypudxhz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3lrhwjurx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3aqodcmwg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3dvfhloje.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3mrcfrgnw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3atskbast.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qnwincko.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3lbfmokjq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3bfdeequt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3cisogayg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ehbrexfq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3pvbsbwbk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ymfeymsg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3aubjmznr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3djjvcuol.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3mftfgxqd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3hylwifce.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mimzrcvo.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3cyprpeqf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3zoauqhib.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3glcxvalq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3wnyocofk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3nxonfuqu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3daxwkqpd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3nkwuelhb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3hxwrpsxy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3yrvvznbu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wpllkvpi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3degbsxoi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3blbhfgoe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3uwvlvrev.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wozkzive.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3eicdgsro.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3wdjkbujt.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3uwkixdcu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3uyzkecfv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnqxdgjh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wgiwgquw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3azybxqmo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3qkwckxpe.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3hjqksnho.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wanrqssp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojisxfem.html


<!-- 参考信息 -->