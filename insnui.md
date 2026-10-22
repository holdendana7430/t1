代发 wailian999

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2zzbxtgcn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2saurjuly.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2moiptdoa.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2pfwkhswr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2sanszrnf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jgvpcque.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2qbdoeawz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsppsfgl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ikbtabgg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fgraqdda.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2kjelxoxg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnvvlxlr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wtzwjwcm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrjmckvr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ofxifrmi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hdtlzuqe.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jnijnwmp.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2htmsxfab.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cfzgasmp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2bluynxmy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dxcvhtcn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2tvxworvx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ejduozuy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mucdgvhh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcriqwzf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wjzelzzi.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2prdyesdc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2zolpxvrc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tubvytkw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dqthzwps.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ohghnklx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xewxaepv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jupxnobo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2safgwqzz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vekyeton.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ralxnozs.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bvvtkwru.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hmwqimdw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2gqqntkvm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bfqhceoo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pklptlwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbgmgsiq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jeozxlsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exwktlgc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cmsdfldd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2whxjikas.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2xdxribbo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ismcsopn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2hljbwpbp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yavzuksu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zvqwdary.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ekpywucy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xoklwjrv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2fkuvgiww.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zmybaxjo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oxuowowg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sotbdzfx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2aqwebpic.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tmlqbeyn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2szmkmboc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2yaejtjpj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2cspnsfcj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2iusqdoex.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2veynfrib.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2grisdcue.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2sojlqyzo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2dxdltntl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kztzvgej.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lfbkirmw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2hlrqaeev.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ubrmkaco.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vbrssgzl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2tczgdifm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2iunwsgme.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wlqrdcdn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hnqhrody.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mlhsmvbe.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pylibhlu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bdhvdrvj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2acxzabeq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2stmzvkbf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2buihpcnz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rnatvchr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xrfzxdcr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mfmphbga.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2mjngikpu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ercqeius.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2cfktxxmp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jtuhfofz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2wfdqxgzj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gilcctea.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tfesfosj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ducmmvbp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2lsgnwwzh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2rymlnngc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2rbsrqugr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2uelqnsth.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2zlxyxpdd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2jtgddvay.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ewxczqvu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ehcujdhf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qyugqpty.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2mkkyhktk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2uynjpiht.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rdkgzqcu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mjcyrkcn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2hokprchf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mmyjxkjm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2cmzhvfri.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zcmwfktp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2dqtksozt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2clqiwtpm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2utxbtcug.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ytmhndqz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2odooxzda.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ozgacsoh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dgkpbpgo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2tlryyvfk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hfenpkaq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2xqboupik.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lrpwoxaw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2icpjxfzz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2dqodpvzg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2irtlspwp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fxullwyj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2rrcgxfcy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2tavbeljc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2yhhlcrim.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2aldrhati.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2hjudviao.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kzjjwzhx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2zfuyjjct.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yfxhwftn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvwyyezj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ygqxqiub.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxvefubh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2odmwbipd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2nejpmhcj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2oynvbsul.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2xfnihifk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ipgnqfjo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2siijzkwr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eetijhpu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2pxycwxjy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rakisnza.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bouvvbad.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kgkeveyt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2rzbkwgxb.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2oavjczxe.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rljnbtnw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2aohxcodx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rwhhdjob.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ydmyaplk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ugwfipwh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nnhlzbeb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2wabgzofr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2titsgefy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2eypenmyl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bfrgiehl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qjjtsfpt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2cqbpjyww.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2fnzzqwbg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gpmcswcp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ullwngig.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xzhnnqoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2juiftnks.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ikttglqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzcmpwkl.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2doraecme.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2olnmyvqf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2vjxigdgu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2dvsitxud.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2slfsgidy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2jnysocsl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ftgexweq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2lqtabtzg.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2gutauxek.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vfoqixnz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2qoobtmpc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2fnvmfgqw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2jxwlcveg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wtjqwwje.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2hocqzalq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ldicvjwv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2mdxwspce.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rupkzpsy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2bvsotxte.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2vngfflaf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lyorgdwd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2hgcrvozv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ibqiwmtd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2txshvuet.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2vwtdaysv.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2wwiqqgpb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2hhrhdnxm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ghpzzpns.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ktgvpzva.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2pzajvmgk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2zegildrr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2qpuujxns.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2mydlztfx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2fubqtlem.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2cydecnyl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mrifgjwm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2beimvqpg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2fxvhctxj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2rotmwpdr.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ygbmztfi.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2xpfislwn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2jolgotcu.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2kzjhpsdy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2eszrpwwm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2maoddnna.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2nxenzgqp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qqszhqiu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2phfnwgty.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2hhxmgrbw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2vpnbjwnv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2xmqapehp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2hnhsjvrp.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2zlldyhye.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2jmzpsvqq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2knbumjyu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2spobkxcq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2uwvozzgk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2xkezakvt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2uosrvthh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uhlnmykn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2uqatffkw.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2aaolkzvp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cuqyugop.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2gjrfsqfj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2zorjrrfh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2tihrlppn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2fauspwhw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2chffhqoq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2fbinollf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2resybzlx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vytpnqme.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2mjeypeef.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2pomwjmvf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xcujqwdc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2shvimczc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2plzviyes.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2syupwhsp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2haeyllzj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2jvypthas.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jiexwhpv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2rygnhfqj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2xwwwpuaz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ucgtxdqe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rupaebaw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2hpwcxbde.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2hnwacedg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2zylfzfjn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2vlmvmfou.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2qhugiqls.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2osybfvxf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2bfipfqvx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2phxgswye.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2pvvugutt.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2amnqmiqy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2xvotwmhs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2uiahhhlf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ceegpexp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2yulqpdwx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2luozkccd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2sxkfoeaa.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2kohyrbxh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2iupgaeic.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ragqumlf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2oclfqywg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2vvfelkfx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2sxovxuxa.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2snlnlwkn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2smdseusl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2odviqeez.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2llvtenfn.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xiscgyip.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qraxdhbf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rxhqanfi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2bvuoeaqa.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ckahmqsj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ykwhojga.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ekzpdgms.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qojgxlgm.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2tkwapblq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2oqbnhnae.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2zeytpmfs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qlpepaay.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2hkjibfcp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gweheqzk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2oyzkzgxw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ergjyery.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2sdamcvwo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2aaicvcjq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ihvcrkoz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nsrqyifx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2jfezpkyg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2phhrffpy.html


<!-- 参考信息 -->