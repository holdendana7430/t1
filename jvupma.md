代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ifrbgodz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qnxjegtl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3pgzhyqzw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3usegwhbk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vgqgrijx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hovranrw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ggmbxhan.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hqswpstr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3nmpvisag.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rmjppmki.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bvzrizao.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3prinurgj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbczhjxt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ofsxzwot.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fwwpvxld.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3urvtjarn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3jfechqom.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3kihlsqod.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3tomnhrrf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3febaonpr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3thbfltct.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3fpwavzwf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3rllzrrud.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3nrajhike.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3wzslxqsa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayukokyg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pkcpwwuq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3xvotnkqq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jiaqrnkn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3bvuvmcob.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rfhgxdst.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3bcsmbeqy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gmuwqpjl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3otgaudtd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3yzpgzwet.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3xlvaqnnu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3esnwkprt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3tscotgst.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3kkyheecf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wpmxootc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3uikmuyav.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3wxpkcqbz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wjahttiy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3upkfveoj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3egcposeg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3yvrztayq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vdwvamoe.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hczqqdko.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jyihfrna.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mmecofmt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3jigqipfu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3viocojdr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3chulzjre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbcsnldc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3deomztpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxsitkqw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bfsumajq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ijztgkos.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3iovwebdg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3esswewmr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3blvlvoho.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zniiticc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3datpkrtx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nupchdlg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zqrbgfcb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3dlostzsp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rwxwqoep.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oggkmbqr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nutgudwd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3eltkjlei.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3tkvhdldn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gcmbeubr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3hjuzmqvt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3lcrliuwv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ziixqmwv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3cgjbxypt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3xtemdhvh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cflsinec.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3dhdtmfdh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qivafoun.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3mkqwdeop.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jnelmonz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qvxjwhxd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gqvbbfbg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3fmnnslfb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wcifedxj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bzxfmufb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ykciwfav.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ozfjfpyg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mksayrhd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3igummlnr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3swsntava.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jzpgwkzs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3yzsukzpx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3xfrahiyo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3pheyughd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ofdkrlce.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ofynvugt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3uymrjeoz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3njdfmhvg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mfimgnsh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ewnllnos.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ezhfhtdm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3preixncu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dibexcbo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3hkvqoorm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3iyyiudzc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3iaktkktm.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zkfnsxyw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3livnjshm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3kibcxugh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3afsolbij.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3fqtsplfv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3zcdkwzsv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mfyuceoi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nzixdntg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yetjfwuc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3knuykkch.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ttszbvcs.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3slkfffsr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kjnwvkka.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ofwwohsi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3obwadksu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ejxxghgs.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3noydksxp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3atwgxrrb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3tycdxatl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3rktfrcey.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lfdlwonf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3llesgqrw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ppvvpiiy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ltxczbig.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cxiusgfz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gysqfrro.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3estzmett.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ujcmckbj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3txveoavn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eriswrdv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3jnpscbpt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3mpcyufjc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3icejtubi.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3qiederqh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3rpbcvacs.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3taymeabx.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3bhyecdqn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfkwnpfc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zxgroxhl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlqppjjm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3iedmlvda.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3rneexggh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xxjygewc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3tygjpvkx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ezedmqey.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3umrqfeor.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3txorexxe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3rspboodq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3pwuxbtnp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vwtxmlkt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3duadhqcm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nfhkhhve.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3nmisfhbq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xyrrqpny.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zkcxrubh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xnwutjnc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nvenfdej.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qyifbjra.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ppbvgllv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3amorgcjs.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bzxnbcxm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jtatbabv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fpfrdgqe.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3lhwaivad.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wxnkfwow.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3gxiubnmh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3yjosmcgb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3gzqrogxf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3nfctwwfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbxhymyj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jcxydmut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cljwdpgu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3cycomefo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3mjjdnbpv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3xuvyzezb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tqhqznrr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3wzmwyrjh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3aadfevis.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3hawejtjo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3nbfwlfpe.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ljoprdal.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ejmibjqv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3fgogkrvj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3cqkehcbs.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3nlhexodo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3uoupbxhg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3oyxdktta.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3hzfkcgzm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3cealcrpf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3xzgiojdm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3xckirstu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3sayhclbm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pzjsncsw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3qbzyeoce.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3uuxkrpmg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kdwtqayg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3fpnidmiw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3eghrfubx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3avqcefor.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3jyvtsmcf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3uamvubyg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3itgsuero.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3rezsakgw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3jxnxcbnn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3eovzciaa.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ktkdnbxq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3zguavdty.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rgxtmwee.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ptgwzbej.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3mntvblbd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3kjtqzfzr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xmpypaod.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3xzudcpyg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3vfvcoxze.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3jchlisyr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3djckpqfl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3oopbgnlh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3vkcknjgh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ykwcihgg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hlhifkbd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3didytedd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3cjuslxgh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3uicigcng.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tlbkimvu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ltbooaza.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3jlajhque.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3aluwylbn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3riljgggj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3dnhoxobt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3lxtlxklr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3bznrhsdw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3obqvwmfm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3rvvytijd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3uijedvwl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3jjkjikjj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3uuoejvyu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3vjdrmcve.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3bdxjtkjr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3evbkxfuk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qkyvaniy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ulekzctu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3pmrlsepv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3osunkbce.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3fzsitoja.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3gmjnpchf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3boelxfxp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rsysbtjg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3dksbmcjs.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3lmpqnmls.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3prdsbeai.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tfzglmji.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3iiuccfnd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3cnstfaxh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3quqiqlgs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3lisjgffc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3euakofzh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3flwfhtnb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3gxxkvwab.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zltmennm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ksoviajm.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3nktclvum.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3onndjaer.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3sswgvkka.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3xqchpxsw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3cgtahksr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ikzqocxm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3livlmiop.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3slwnaspq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3pwjrcnwg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3orncwbgl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3lvbtdimo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmjibpqn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3mtooavfs.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3hfyfnmnv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3thgdhmbl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3msswzxpj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ypjspdid.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3rplzxqbh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3jlazqrbm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3vialfftq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3iveafuph.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3aypbuqlb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3drypdwwu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cjmzkoiu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pzfamycp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3grtrrdhh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3qxmqgckd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wdazbxga.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3pltaycaw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mwrxupan.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3poduijjt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3atsarmpv.html


<!-- 参考信息 -->