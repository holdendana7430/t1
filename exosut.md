代发 wailian999

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3aizvyghi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnyttxcc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3hxvnckap.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ulgzqsuh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qyajmgct.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gkimwzrm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zviygafu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3sqhraukk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ttxjozot.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jooxzveh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lfhczlcm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zlcxwahl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3qkoybrpq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qiukdjhl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vowjbsne.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mohkvbta.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3rshezzqb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3roelgste.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ybhomgod.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ceeezlay.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ycmlsluz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3wnavnnlp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ukjqscph.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3vxfzdtzl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3jybagjjj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3nkublxae.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3lftjqwnn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dobjgxzl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vzkojsfm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3vtwmtwhq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3bjtbkdxa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjknfbnm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ryxgyrlk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwrtxdou.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cgsbkvqi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xdcvdwix.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tmgjbmbb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3bubpsmwg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3wshdfals.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dhawcnyr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ivfjfxxm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nqumpphn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wosuegwt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ddyldqwg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3atppbstl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3cfmlxtxl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qbrmbrwg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3cqfykjir.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lcpsuhbb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3mmmwptbp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sdefqaaj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3cntrruiw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3rljsqqwx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3uahutuyq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3epvymqio.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3jmxsermj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3smsvcyrj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3rollrfip.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lrxdlbub.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3arfwymxx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nlnnuhti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nutnogck.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3rqnowdla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqonqxvj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kdhbdoik.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wmpbdapm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zmbfutvi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3jimappwd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3pcfumctx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qslplzhq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3mxhvtswv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3meubchvh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rlzrdzcd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ficljfya.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3yfbvxolo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3janciooc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vpytgtbv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ccdppeah.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3mrakcbao.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dgqdgpsy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmaotjzg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ufslhyji.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3texhvxhr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3yqkiwtud.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3jgsvkxzp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ofmxrzqy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3nhofsnym.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ijfhbnga.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3exhkshii.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rrhlclhh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3frlzmkzo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ryeifnnr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3yhpatxfd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ghjkgsmf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3prqauclm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mzqylzuw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3tybjqbfo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jlqxsthh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3azfgyppw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3sxschihs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3drrgitxx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zmrsrhdr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ebebcuon.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tcqvtiru.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3thdvgrfc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3dyjsczfy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3bkorgddd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xpjinmgh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3yuaatkvd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ouvcmvko.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xxoekaji.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bcxnvqtu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3nsppnmug.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nqtaukll.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3qaujazmu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3urzmpjcc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ugrulpur.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qrkopiqz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3jqpwabcb.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3gfksrxwa.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mgosgilu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ayupykek.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hqundwmf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gqdqpzru.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iqsfetxr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dstdgroa.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3eqlabvfz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qxumrjsr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3zzfsntnr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ncvnwjra.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3wptiryhg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3dvqrwwac.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zvtqntba.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zpysfirf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ezvlppmj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xpgxjlzi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3cnmsnyvt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3dowgchhi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3lvvudqpt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mqmvevoc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eyuafjkl.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qojxcmnx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3zchaezgk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fopiiidl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3skkxjjov.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rrsycjoe.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bogyiulm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ysqqsrzv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ttpiygvd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3akdzyhlm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xhqlibrh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyiftqup.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dgmlezta.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vidvhslb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3bpwtjzsp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvwjdywq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ovrnfpnq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3gsgljliv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3dnanpcyl.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xgrgvyat.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zilcozjd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3siecnkkm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nombtugx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3rvmwpvvz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkasgmwy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zncfkzsj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jbyknprv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hamdtdld.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sifzgtan.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qjgewnze.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pmbatltk.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sgoxdjbh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ouvlvvaz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qcdwsplk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ecisojif.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wsdpkihq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3apbgeocl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vogmwnvx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ixlpynci.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3eudylasy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3fresyhmq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3duvukona.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wtkhjepm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ypnoovkr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3mjvtnmmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhpkxehf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fmsktkev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubzfltgb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qhjpfcjb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ssmoqkgj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ganhselx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3dnmakwoh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3huvkfgut.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ggjndrdc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3tvoyzpub.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3okiwpcju.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vsymubsa.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3idnpvgsd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ueffdquj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3wmxtmept.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ywkxnyxm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ymbnpere.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3bzjvcbgs.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3zzbxsbac.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ahflwfxx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3frmckecv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vfwewurw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3cdfankbh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3uzydmpaz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nynkjisf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3jkrfvvka.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3awsiqjml.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3wcrdttxw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3dhnnnwot.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3iavwhgqo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3qfrotthi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ubbdrzzl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ozghkhab.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jlgffpbw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3bfmiqqmb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3mbnerjfp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3aiqytqmx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3wxgjqqow.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hqoezomk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3hnzfvciv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3fsiywnuu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3krhvabcp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3yfnntlcw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hnaduzmo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3qetuskys.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3isvgiefr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3bccuvoue.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3gqjgjvdy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3fijufpvi.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3yttkcxer.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gfwgdcrv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3msfcmutz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3lczvmjdh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3avcepiik.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tkxpkosd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3yfzmxazt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3kgwpzqhk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ioayagxw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3cummjagw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3npdftqgw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3hrqweuov.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3suxnatlx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3zuvxtojh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ocmdvvav.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3itpoldfr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fnvztykr.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3mkjrdphg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3fnvfhnkv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3onlfxuph.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3xvgamxmy.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3qgsrpdmi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3hsyekebp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3avqkmwwy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3wqdeymzj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3hqpwrjyq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3cfhedhya.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3erskccfm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3glbkrcmn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ufpcklzs.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3umfxubtv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3dphddtok.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3nrygjvsq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3raulsaib.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3shsusgqi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3edkgxcdf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3aexykige.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3itmumsfd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3uizxulko.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3yrkstzes.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3lryiusps.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3unkozvox.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3pgctshch.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bnflmfno.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3fnnarfpa.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3xbticjfp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3bsyragbo.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3xoprwenm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3kuzvstje.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3amnfwmkq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3fbquhhne.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3cnalywwa.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3huventzm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eklinemz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3frbqrqnv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3srzhnnzs.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3glkcaruc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ssepwgsc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3dxiwhxub.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3wigandrg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jhdtmikn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3tvgpwcic.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oqisphcv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3waiuaknz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3aimuyrnk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3codummvl.html


<!-- 参考信息 -->