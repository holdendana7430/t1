代发 wailian999

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/ghsjluyfk.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/goqhgmicq.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gsebqeyni.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/guesbxecp.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gghhrnbyd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gaiklwzsg.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gootqfzto.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/grfbdwzrf.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/guzhozpor.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/govvdkpnl.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gkkrqqnho.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gqijuyzem.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gswvbrsxe.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gekebidkz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gukfebznt.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/giknafamf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gbsswsjup.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/goznezomf.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gxxlvemty.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gqayqzzvy.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gtgcsgtto.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gmusaflcq.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gpvesynkt.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gqfmpfmgm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/ggaxitzol.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gyeavsgrx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/ggityeehq.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gaofecpxr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gtskvnrkg.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gftngcqgk.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gnnmyxjll.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gygsbkxlz.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gpcukqavs.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gnqfikkqk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/ghgvnlcdx.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/ggpzfpnus.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gmgmvhvrc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvbavffuf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gzfhfffvx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giriiwova.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gdjojtebf.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/geixyldpx.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gqahysjnq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gjdugpexw.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gqccyveuq.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/ghyhvndpd.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gpjqjuzpd.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gbiwodena.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/grnvlkeps.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gsdgkuero.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gvwfzcwym.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gtpirhcie.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gezhaoocs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gbivnwbce.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gqqrkmmxo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gqxbzxmim.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gdioocksj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gcnkpgjuu.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gtqhjeldk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gwronphas.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gbsqvlhwb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gmtmpquya.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gouoodheo.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gdpfyihzt.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gnsrmzrzw.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gwttayciq.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gceockscb.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gpnydceza.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gmlsourbp.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gpdrcjjqv.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/glwbahfax.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gjrhcydts.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gaphbohiv.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gbyqdmmwb.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gzdylrrnr.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gryhbalzl.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gdkxnxndb.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gttgwzzmt.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gkvkulihq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gamjicufq.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gpfdrrvav.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gxncmqqnx.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gpjccwkkx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/ggqocvaor.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gfeaneuzx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gtlesfmto.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gdwozzair.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ghawjmtam.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gyqkzazrj.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gfkbzlyuz.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gtfmycyoe.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/grfodcivm.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gtxgzxhjf.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gkftjyvxk.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gjecnhrap.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gxelmhioi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gyzhowjhm.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gjhqbnaue.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gczejnqbj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/ghixwfmen.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gyqlsorho.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gapoxxrze.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gtztftwme.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gcxzpfokg.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/ghjefziqg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gfnynpgsy.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gfxvagljw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gniyyiznq.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gnvlgmoqo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gfzjqcjmj.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gguozamah.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/grsvbqror.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gvkuxwxjf.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gbergmujr.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gbseidanj.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gtalypfix.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gwlxravro.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gttgxaqlf.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gqagldlra.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gimhrseat.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gwlukttya.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/giwfapclc.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gampikawb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gyatrirej.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gtivlnwvp.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gpdnlibho.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gzzjmletp.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gkgkyzgbr.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gzezbhjgn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/glbzdtjtz.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gmrxpgxds.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gmdbqhmlp.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gssnssvlv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gzmezyewh.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gykfcdqhj.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/glsfabgoj.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/ggpaxvktq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gqobwogwg.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gfgkeuiyd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gaxjclrdv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gwqmdweem.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqwljjfrd.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gcvzwtycl.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gdcmweygv.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gskicfdot.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gkaxsvkcy.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gootjjvny.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/guuzvzuuk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gfknuvnlk.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gceyczioh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gbqwuejzr.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/ggfpmfkix.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gposrppxw.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gqohmnzlw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gorcezsmp.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gtaglmale.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gdwanmjwn.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/goypwkdno.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gppzesbin.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gtdrohjxt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gjuqonvwf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjjldmvqg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/goqqrxlnf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjricinai.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gawfpjxlm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gtfadvxxh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/ggxsumtnj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gasprlxvm.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gsxyhzihs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/goknfusnf.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gedncoenx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gmoenogcr.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gbacmcexp.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gdbgxsxkv.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/geuxocbjq.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gnbzkzmam.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/girdvkxlu.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/ghpkxriil.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gviuypawo.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gormwpyjy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/getyjlqtq.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gtzslpdgm.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/glytgeatq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/glgjlcpno.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gwsehgpus.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gtsdecqqx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gnwgxlfaa.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gdcypoxlr.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gfinkrpfk.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gwlsouxqz.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gcubtzkji.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gobmibmdw.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gfvjsynkm.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gxffvfato.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/ghhpfnrbw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gykilmrtf.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gxgmzibbv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gqrxjwzyo.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gewihchcu.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gaurwcnhh.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/ghbcesrna.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmdvrlin.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gmifccfjs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gcumvgllg.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gfbxzscsh.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gnxrksfpg.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gkhjhhskj.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gknoialjv.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gfxdnsacw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gpeqcqjae.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gcdgaacjz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzmlhens.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gpikgkeib.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gkxdjflls.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gwsljdnzq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/ghwqowyzh.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gzvhrfbqw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gjzpyiasz.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/govwulrzp.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/ghikvpbib.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gknxyfqxh.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gktnlpkzc.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/grmgcznxd.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/glqxxkipl.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gcdeyhnbk.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gualwniam.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gcvppsewd.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/ggzhuxgil.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gmfatoiiv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gqpeyuyja.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gzgqovddl.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gofnzsliy.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gjtadkvao.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gsljfyikz.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gkejhbtvb.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gjntrnrvz.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gfcgbpqoc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/giueuonys.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gpulhsrvz.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gegpvlfcs.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gowjnldjo.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gqqwjhlus.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gfoqahuds.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gggzddvfi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/glnjhnqli.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gomjcexhx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gfalwczbq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gnvpfwmvc.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/grcatzitz.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/goawwkdcc.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gkmtizisz.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gubzryjcg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/ggqgmrvub.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/groujmhui.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gevedunet.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gxkhnvuaf.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/giawnpkok.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gjfzibflg.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gixvyjgfr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/guebweeri.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gflhxmorx.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/grqxkiilv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gpljtgbto.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gczdkklng.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gbwcewazf.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gtuzjnyvm.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/geeufstub.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gzfzuezay.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gpkkakigp.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gmuofsfvg.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gyvgkrqra.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/giegjhfrc.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gfiznewzr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gqbbtdorr.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gunjpapyd.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gfaavlhds.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gfeipapcw.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gvcgthvjf.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gfgzjcdxw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gheeljlue.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gnsjslvac.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gqwzzndzb.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gxqdckvke.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gswqkgrdt.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gutwctahk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gdphedpws.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gczonmquv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/glhznvthj.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gseiazixh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gzulsyqmw.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gdznymchy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/ggnaksphz.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/ggljzxtiw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gyaayhnxy.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gstrxxdpx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gyswfncar.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/guqqdmisd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/ggvgcguwv.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gjiuhstye.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gyllbvoin.sHtML


<!-- 参考信息 -->