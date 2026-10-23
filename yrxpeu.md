代发 wailian999

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3taewsnsl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyfgliuk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vtdiglyo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3zgdzpfdx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3edrcerhn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wqyqmtqp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vicvvrzc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gfomyacs.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jltgqjik.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zihctbyp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3sfbhlibl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vinznnyd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ryqqigss.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3iixxeaep.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3jwpfltmt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mkbxohnn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mpxbxumd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3dwevspwu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3urgbnzlo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ppwckmwm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3idrflotl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3mauzrrjc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3bulydvpk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3byzsdiqa.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3syetihsy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ymetfilz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3wgvbsgta.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3zjzboflr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qzwlaekb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3uvspsvns.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3iheonjls.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kpnzpevi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3agxydmcu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qarivjvd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3prucdhlv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3cfutpghn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ictgsnro.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hobkueuu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cexdimxv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3rhmojqgi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pnbbncxa.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3kurrhchz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3lrifeage.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gvjyrebv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3nviiuykj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xccczvdv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3onurtppg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3oofqayse.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3sebonncj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pxvuwdsh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3sxlyytdu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ncxtvzfz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xpxqvits.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3wbvkczpb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3omlrzwvt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ovqhzyjq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3phgukrvf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3sqmoxakk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ijavvtyo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3sltmzpge.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3htpoznmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgxrfdsp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bayifuob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsesqgfm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mvkfqkwb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qzcqsasy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ssvpsbjx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lofemxhf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3fxhklcot.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xmmtukpy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3goihlata.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3pqbksndu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jdjnffuq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3hxwytqok.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kjshxjwx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nkhzkqhq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ihhgvhzk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3nzjrtenc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3otzmetuw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xcborgym.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3nprnsyys.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3lpsnxypq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oemujzbd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3dbjhycht.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3gqatffbi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ixfoxmxg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3marrsxxc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jgxnxcit.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rgwyrdmm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3duxipsek.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xofrmafl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gdyfjxsa.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3lvmvzoji.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3kvdzulwi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hkpwxohl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qzuixzfg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3rvbkusfr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3imzrbdrt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gmglpixn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ptpynsll.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qvifqtrm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3agravfhf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hpjsherf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3pwbfhyls.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qjrkyuzl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ojrsslel.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lddkyiof.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qukkccmx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3umqsueix.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3lvcmvnmo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3fdanhzco.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vgywlqqv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3mufiewnz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ghnwumii.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3feffhsgc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wzdimldg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3sekoadow.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3tmahvzcf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3gexkardu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3klpfzzhk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3tljjllxk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3osktjkqk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3daqrnhje.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mxgmfmac.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jxfdrjtt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3njuwojry.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ksykxzct.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3zqogyxom.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3chqtwqug.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3xxrjuuug.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3iiyhdgro.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3wvhebtee.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gjgoxtee.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xsauldlr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3feqhifhj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3scizptoj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3czmdvcbv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3eguogfzt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zxpfjzfh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3odovgzmw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3afaivvzo.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ogzqtqyf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3onfmpvvl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zubcjjtp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3epmvbdxn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ilyijflu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3cljzsdmx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gqhfzhth.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3prnjqtrt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ulxluczg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tvqdovkr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lemdkrxq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dvyqxdky.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3aiplozdf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3qdexboia.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3teqphnbz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tdneftgw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3mghldsjq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pdracivb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3pakpsmft.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ykqdxuxl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hmflsedj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ysjiqxce.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3gruxglla.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztaoiemt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3plaqymzd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dqyflibi.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dtpgxiyo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xbhmdtgj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ayehlboz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3amgzioqv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3umrigaxv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ulcykaao.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jukekmrq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sohgvlcx.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3egttfglb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ipcjkhxu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ptpllddp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kyfvpkpf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3xkhmfnqq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jgainoec.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ufttqgcw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3luzbobgk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3lkcgiyht.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3yhegubck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zudnbelq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rubyleop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uypcnrmm.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3sewvidsg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3awetpybl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ploorshw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xnutnszv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gohopylo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ljbijpcg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3vxoeitoe.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3hdenickp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vfrywbeo.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wmacqcda.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3nzydfucm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3yvmflkfe.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rcrhigsw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ngfebhyl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3zoxovzif.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3nkgsxjvz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3suowenfn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vrlsngsv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3cwktfxpk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3bagghzbt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3absyemib.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oxeuqtyg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xtlrkrmv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dzfsvvls.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3lamdsoka.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3axslhynb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3xhdblufj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dpouqajc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zooluyyj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3aqvcjxft.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3hfexkugt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3xsrwojsd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kwbdfcea.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qxvhwapv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3fothvpve.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3nggejdhx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3nfwdnpzf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3mmvpvaqs.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3xomwhhze.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3kxacsowx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zzmpkheq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3udmumypy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3sipzpyhs.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3zlyqoqtr.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3rwdlhbed.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3hayyiguf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3savxmrcl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zqbcicai.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3iqjiyzof.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3weuhndlx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3cwwkcooy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3adgbszjs.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3hxzmdmjc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3aubhlmnd.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3wbsdrzsy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ftzrkeax.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3mulcloov.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3uibwzrps.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3bxihzquo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3snldbxwi.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3fwbttujt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ibsdfcwv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hqavxcga.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3afcyypck.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xshalwhm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3xpcmqozb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3gbwkqoja.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3vhrhodhi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qucdealu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3bqxtbfwt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3eyuxbgpj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3oullituy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3gkgqwsej.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ikyczzaj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3nweiqdlm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3cyxpoqqb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3pxkgbmol.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3jliewdit.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3dynuhwbg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3unvquxvq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3mehrxxlo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rleiimua.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3mkadredt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3fxhelsrh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rbkofrhf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3rkozeuzn.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3aryqklgo.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3cbivvdln.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3xmpjtage.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xohiuexe.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wshpjixb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3dzgglfzy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hvlwmefs.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3gcazyeop.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3qwkenylg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3strpxivt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3gwkzxjyh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3byxcrblb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3lyrirkuu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfcurdvt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3sneeynxn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3wcjgoqoy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gsrlnyxv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nqjnpdwi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3vncsiooz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zcqzyaoi.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3cvvalvgh.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3isoxujyt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ibczdgdy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3zvqxrjvh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ysgbatun.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3oimsmnzf.html


<!-- 参考信息 -->