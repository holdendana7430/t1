代发 wailian999

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3lnxvqvgk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cjyboyyz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3qydmuazx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3iggsqthi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3olpxdtyh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vybzbhno.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3tthqcngi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgsgsggz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3fwhiedrc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zcrdtcwe.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xufnlemd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jukeemkz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3cdgnekfc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3uigvsvxv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3cdzvhsxm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xrrsymdf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3goraeehu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3uuvzoqwr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3anxlfwef.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3lsbikvkg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jbpynens.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wyupxxgg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3txkfunsr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3uaygrtqk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hypjwubh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3bierkvlb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3xbaqbsee.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dekuroaa.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3txdscpag.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3xdsyxvfb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qryrvnmx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3udmslqay.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fsurdoci.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3jibuvdau.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3frrsaqbq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3blqlxrfc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3lclccsft.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3nsruxxhy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3bblmmkaz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3eqdrpdvv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xwyvizrb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3cmewcueh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bfacgoqv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3adkqqukb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyqqtzsb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3viguihwa.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3tfyqakcd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3emjufqop.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bejmxjjr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vxompjpj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ggdxexop.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3aiuwdgaw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3nwolbbla.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gdainale.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3tkwcplsy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3mzwrudkq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mwfyulwp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3coxsgcaz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3rjhmuvat.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3yokpacgr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nxuwvdbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cutejcvu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qcgsisjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyajkbfi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gbkxtpiv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ykqiwgwn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3jpqqhumo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wrqoyxuy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3hyotqkbf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rcxqhrgw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rjqmwiqk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ndhsklme.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jmugppsz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3vpfswwmd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vcnktryb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dafgeciq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pfvrujjk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3lorehujz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3npypfhaa.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xjyrwryg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zoocnwyz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3nzeswsds.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gbqkdety.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3hxytfoov.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3rtsuwvam.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ezdmbrcf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ebeprjls.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3befkeabq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dqxkcrmu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmkmylwl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wuzmxzpe.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3foaclxqy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ivnqgppf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ffrnqspx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3onitiyqz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ytdtzmgq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xefleajj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3dvfflsey.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eqmyugto.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3qgbpevsm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xxeijxvj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qlatlfvp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ymyqzsvx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qpauwvpw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mrachvbz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lfbftfjs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ytuxnuwl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xgtcylar.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3femuijtv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pdvdhphc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ktevhysg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hrgzxchh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3outnswrg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3mxckifue.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3komrrqqz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3uzlhngqf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ayxihuec.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ugrmxpig.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bkvpipai.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3jbirsxyv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3djptpyoo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3egjmlvab.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3xswviduk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3amzrvovo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xltvtjam.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qbqveoll.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3eahbndap.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3hmjbgeyo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3jggzjhes.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3zkxoysre.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3eaarkown.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3eqgaiwcg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3rlnwuvue.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lshpkjew.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3fphbenma.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ydvryxgc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qktmtlcf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rcixpwfl.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ahyfyozv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ixnesuwa.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gvfqtmus.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ogmspvsh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xuentzzn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3auyjewlo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ydyomsan.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3infgrygo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3bvqenery.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3lvxvqrds.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xksjqubd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3afkixfek.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3iwknouaz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcgasslv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mgebdwrb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3drpzelkl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3kzlesgms.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbeeaoou.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3eghpfldd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3miobdpyx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3agodysxw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xulvokla.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zdeoxlhq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkbzemii.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cdqklkbn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3uokdubqc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3mhwkarkm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3djasgvvr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3orhktpsi.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3mniszjjf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3yqduqtph.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xvzeqvdb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tkmspsxg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jnqtwzzh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3fjxwwqso.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zgbdrvck.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3haxgxumj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vieapeux.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ebrrhojn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tizzkeqy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lnehjbme.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3xkpqwnwx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zwpyrbrw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3stcnphmx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3upagwyoz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3nqbgluoi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3krfddjvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jylrolfe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qjqxyiio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzlwujcl.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3yuymrhhk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3hulwtmyc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ujwqidfk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3piatpzwr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mokdtspo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3fxwjbiqw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wsrlnhhq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3swcuriaj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vetverwg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yeuvztfl.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3vkmnhexb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mauvurpl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3oqmpmnje.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3twxqhrbt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3jyxrlaey.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3utewmafc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jmjozxxo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3flztrnnx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3gcuslgao.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3wpqstozm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dofeeeza.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3fkqklnzq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3tqudunsu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xdlkrcwy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3nszcoqub.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3rthrfxtn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3yjbsnses.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mzqjvgjq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3hrefuadh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ahcwhlqt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3cnanwfvw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hdsncqby.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3geiajphh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3brcuaqka.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3zsshmksd.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kafmklhb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3cfgxslsm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3fjlqewtt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3sxxtxaai.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3pwihyntn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3bbdnqcim.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qbdfzjzy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ywmjvlow.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3zjqhhnaz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3grttrblp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wvcrzrqm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3kawhhkej.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vrlhzwvz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ilvizzht.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qvwrzscs.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nhbmqeno.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3tgffnlvm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3hnaiospv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3kuqwedih.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3oymdakms.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3tipwjzxz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3iuadodxr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3glrqjdcf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ciwwefxh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ugrwegzk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ucyusmod.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3cwscfykk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3bhcqfcbm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3mghfxncf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3jxuppuxq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3xnrlhuzp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ffqflqts.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3zctpqqfb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3wucbkvms.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3aipqdaal.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3pmgcxjor.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3idhohwpo.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3thtvixyd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3jyjentvp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3mzfsjztd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3eeynhyxl.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3stiwpryk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3fhbzujoq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3uwdgjyoz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3waxlpakr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3mbabfxyl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dlleimgo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3jgsbqhti.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ehtwxlfc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3issdoeam.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3mzgsibtn.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3kwmxphjx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3wptfajbs.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ilnbzhht.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jbroqipm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3savxgwfb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3piutkjyi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3rsaninbl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ltsqfemt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3uigdfohd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3dxqyuyae.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3xqswakpb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3xyezouys.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3imaumneb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsvrtzxu.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3sqbyprpr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3soselmgd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cspawpfr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3peopyonl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3lihgrsog.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3jbprqqiw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3kixusowu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3sfgqlynk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3wnwpyflx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kzvoygxm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3rkfqcekq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3byoxkckj.html


<!-- 参考信息 -->