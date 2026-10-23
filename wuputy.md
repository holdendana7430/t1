代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3gnpfxyuo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3iyvagtgq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bpphmvqe.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3vxovtieo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rlkoczpr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3swvooxnz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3wlvglelo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3yrstmifz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kjxycovm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3zvsvownb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3fercuryx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mshsejnc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3wukhstur.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmihsjek.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ashzhkno.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3aiqjcltr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3thmhbrgq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rvmgmvwo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bmfrrdur.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpitaofv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3apkpmqum.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gjuoemvm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3pqcinndn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3okzuugmd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3miatfhyd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vxdgldfw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3nsqfxaen.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fyxhwrvp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3lmmbtzzc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xgobqloj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wcgfsper.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eaibxjrm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hnhzfvhs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3coeisyju.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3zasauiqt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3zsnghimq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3kajdjtmb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3brakqads.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3seilgrsg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xutcdlnv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dqxkjjdr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ozdxrvtw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3gcfxkvop.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tmzpjccf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3arfordpt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3yllthlax.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uwdqiocv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qnsmxrcl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kvtktuhi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3sazdgpty.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3uxffuyyw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3uyusgxfu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pofjiawd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3omtqeqrf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3sazaanxl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ukmjuxem.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqkgpcjd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3slcxoygr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ebdjqbuk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3yansublh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3adeuauhu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3bglbyapj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xitmdjpj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3azkgldmv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaeprdpf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3mytsqsuq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ajmmlkfo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ydqjffnd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3kiwynpai.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3npevavgz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3dhvgtfil.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3sjfncwjd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ekcmrbea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvfhmibk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3crqzwrxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flavuhpt.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vcfqqrjr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vlsqlxnd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dxvcyjuv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3yzphelvd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3erjtnwpd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3aargcsgj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3msoivhbq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hccnydir.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3kkwwmirk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3nnhrjxih.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3udylfpom.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xtnygcub.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fzsafwli.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ljudnaoz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gpicsgdu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bhosoyfq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3apifehhr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hzssnwpl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3otgujuvr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3pvyzevnn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3rmgejfwv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3mvncmexk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3phtnxowc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qjpylumt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3cbjyaqow.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kopensvn.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vnythhet.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kpstuszc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fwpcqsyu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jdosaxqj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ifqvizko.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xqfnnaiv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vdsumfnp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ondilmtd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lcqquspx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3cjgnblmo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ikroruxq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3odlsuyru.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3yhsksvrh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rkiddvmj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3cehfsglx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ohytpzqo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3cgsorwif.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qdsmkvcy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oaaqghjf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3rzcuvfdp.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ivnqxwfz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3poehjfbd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3vzloplcf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3xknedoeh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3qajzaadp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hgnmkxry.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3tqjfhxyx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3uxoicxgi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ezagvlcv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hqzbrmhd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3hbgrlypj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3stodxecw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3tkjxqtpu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3bwpwlakg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hlsrnuxe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ucwkqpjk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tdmpeeob.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3coqzcxpa.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3czhbpmju.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3nsokausc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hqxevccv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3jjvvynyn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3wmcnnktf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hmfftybv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3osmzbsqi.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3dtkfhxri.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zbldtjts.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ezgeayxg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pfftxmpc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3lriphbro.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hhursjlk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3fxhozfje.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3doomwlgr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ftrytydb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sahcuany.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vlxmddiy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nuhikody.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lxsevlfc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xsiwemrr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3cjvlpqla.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rapyajuc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkfmkfks.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3xylrgykp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3grmtpkvy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3dplmpass.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrxwzfhb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3smzqkwap.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3zpdmxgwu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3fwlzxuwn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3nqldqzmg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ujqaxjwo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lnljnooq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tnaslznn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wykhujbd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqvqsmqm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jqxcdgjv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ksjmepms.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3lmwrltql.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3sjamcqbb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yyicurtt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fkgtsjqm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kowgivpp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pewutfud.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3clwjqzjt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3mwdatxoy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3njygwrqz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kncqzmet.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xqgyhohw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zscldfar.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3byqnxjhv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3fqgbzzgj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3imhdhdvs.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zmvbvssi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3itvrcqiw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3sozatxui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvhlxhug.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lbfrhcqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzyjymhp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3hqgucrsn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3lnygtniv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3rbmntzjn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lvdmdbty.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3rvkiiebh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3pfztvhgh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rszuwwfi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ftmfmlvl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3kupyzaym.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fjgzrdaq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3uzrhwiof.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3mmootmxu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ixvvyhhx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3lcuifxml.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3vmpitmbp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ahbjkuuz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3oyeokhrp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3oolxqwqu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3hyewweba.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3oceaqqay.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3fsaxicxu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nkvpguek.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bddrpimv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3soduwuqk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qrtuqhjk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3vlzmclif.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3vlrpicnl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3atmxnuab.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3owaamzkx.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3kasultvr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3dtzzjule.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3oyzifziv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rjcghwyh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3vicisiqg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3cdsvgegl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lezhtspd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3syotrmle.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3vhsuizdv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3qnshteid.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3vvxblwpe.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3hfguiwno.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3aumwhfrr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3iqrcpivj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3xskhqptq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vqlhtuke.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3yvkbplxb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mtqqzyqp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bnkvnylh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3azbzqftr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3fmaovsza.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3hxdrfotz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3eqqhzhda.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3jxrgajlc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3shgjfaoa.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3vuojphjd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3qfmuygfk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3dfvsqpjm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3xuutldfl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3qqelnlvu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fjmoherf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3wakktlpm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3grjlsvln.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nihizmew.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3txohsgam.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3maxeenyy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3akdeoiee.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ijwyhstl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3kymyxysg.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3znfvnppz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3xbowfkco.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3jkvgwyej.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3fcunijfx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3zfokkecj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ygubaqyb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3jnjybjpr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3wcgiqkzs.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3gcyshaak.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3uzpsnoyt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jjnykmms.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jxqpbsby.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3xhreadhd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3wofahceg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3peoqtwfu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3azptosut.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gcjagsrr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3wldtbagi.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3jslqwvij.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3dpwnfqvs.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3fxxrgsqw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bzgptdus.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3cjirocdc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ufnlqhwy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wmhbjfsq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3hgkjabco.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3hkimnurb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3oawzvbam.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3btpahbla.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3giannmtc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3dtcavkju.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3mggeuqwe.html


<!-- 参考信息 -->