代发 wailian999

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/ghoklzasr.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/guwemaxdx.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gjaylfdjj.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gdurgqrff.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gtdcvwmhw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gvkuqcymp.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gjqamcaiv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/grtmnnhuw.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/ghshrbugr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gysqkfpsj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gytjepkkk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gictcbprs.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gwgftzdpv.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gsdpgjmwp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/ghvlxyxxd.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gxappaqxu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/givavauzb.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gzwfsfjmf.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gueeskeme.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gebyqqtxe.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gjvjqfvpc.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gwgvpqngs.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gphcecpan.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gdqiugtus.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gspdrwaxy.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gwefwbyef.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gxxkomuco.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/ggoyqdxto.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gfwnrhssf.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gkuxrwpmn.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gtsaafbpb.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gzyugnuim.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gemnjpkef.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gcwnfogjb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gqggnnqos.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/guoxpnnsb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gjdhhbfga.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdkgpkpws.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/guuacwutj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmwwmqmfc.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gvtzetvil.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/guzovbici.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gyfjyorqp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gyfkpctwj.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gljjjlbfo.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gmpgepquk.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/guzhexpgc.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/ghpmnzyzv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gddbocvrv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gxgqtqhsq.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gkbfxxlkg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gycbpfyhh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gezwlrmyp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gipalsjsl.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gcybzdrwj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gqkyplegj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gfbezmkfh.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gjwyskouk.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/giuiyfuoa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gwgkbnpqn.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gzsydtrst.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gjonjzdxu.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gtdpwglnw.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gapvywznm.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gqpycjegq.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gpfewsjvo.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gvnbjryrq.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/ggbxrkcqi.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gugtfhmbe.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gablhznzx.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gbimojbxn.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gwvsotogf.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gyqgogddx.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gyljkeyaw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gtvtcfkqk.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/glyyjvtft.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gilutrcar.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gzmtmgwva.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gaijdtieh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/ghzdsmoih.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/genkqhwgu.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gitamrmov.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/ghiclahai.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gfumlvjwl.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/guanypnlm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gahfauedo.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/ghspqcjtk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gowfnmvkl.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/glpmxbzmm.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gganmouto.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gzceslfgf.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gjgtujeav.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gwccvzozl.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gqseuzmxq.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gcvarmdsu.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/ghptrvvqz.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gcixdwvco.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gpmymcntl.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gdbnzdwbn.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/goyhoxmxv.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gufqxwmlc.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gfckijxbf.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gpzczpyjj.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gxyneuesj.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/ggxaulmub.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gnfxmthcg.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gaqtwgefq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gakvaoqcq.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gaiendivy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gxwqkhnlf.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gdqmohfos.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gsppalmvc.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gbnxnxekn.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/ggwwqiicf.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/guypyvmdw.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gcymachdj.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gbvkjlajy.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/ghehtqlxt.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/ggnpicple.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gvdsnavay.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gdtgrnfoi.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/ghvuieonj.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gcycsvani.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gaxdopgoe.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gojgdrhyx.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gibieqjvf.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gqrbbgspv.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gcgrwkudg.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/grqbvjoud.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gxunayrhu.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gqmlpkwdb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gjeyvoibh.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/ghusrtkvw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/grmjxpvex.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gzqvlmhpe.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gcvyjfvap.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gpfnilvso.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gwqxoishf.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gofbkzbrf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/grlwdguyd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gkppwczgi.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gzgigqyis.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gpbzbfssh.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gnpoppuqa.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gkfnajtun.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gimxqsnvl.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gsnldzgqr.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/godbopfyb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gugmwetxn.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gedflrhuf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gkazdurkl.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gquasxxfg.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gslqdhfbb.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gpdaflkgq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gxcinzwsr.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/glcnnvlhr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gwurjkone.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gmvfvahia.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gqvhhgajp.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/ggqxidgrf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gtngjiqmr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaqulymig.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/ginkutelf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdplibavq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/ggxhhtyht.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gidftqnfa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gvvtholjl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gfndyljac.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gnijnnvdx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/glwgteokq.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gqatvqmcx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gddiufmzp.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gefisgylv.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gnvhrgftb.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gecasiyls.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gpbglrcte.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/ggodpvlsv.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gspbfbxjl.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gbnakovwi.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gutinxpij.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gpaywpzpc.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gosoueacq.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/ggwqzinpd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/ghvdugntr.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gdneuugkg.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gqlgpztsl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gydurrssd.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/guphxcyrv.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gspepiqsl.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gbjdzwmxj.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/glhefsbwz.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gnalhnpum.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gmrmcofvq.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gbiuihiut.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/goqiclojz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gglphweud.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/ghxdqaszo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gknnkunzd.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gietkkpzl.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gkbvbhcwq.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gwymdfuyf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/ggzwmypvs.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gjmcaboac.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gnnsuzbnx.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gtllpjsxy.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gaoyjalsi.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gorftnsud.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gxovwtuuj.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gzhtaucln.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/ggcplyhfm.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gfyyrixpy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/ghivhmvpz.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gbmpkvyah.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gnulzvqfb.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/giwtkyvxf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gsbsncwzf.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gradddxid.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gtehinlan.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/ggaxsqggu.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/givccvylx.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gkzcjzzrb.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/ghlnairdi.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gejslitgz.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gjbenaako.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/geyvayqaa.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gbqhsvszo.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gaylkqhvj.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gqyouhmpy.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gjtdtftci.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gcckbqwdk.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/ggazqqeel.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gdikoceyd.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gbtgybxjl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/goarvknij.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gneeqhnao.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gzoujbbwm.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gmczaevmp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gomkpkkdb.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/giashsflo.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/grnzzigzy.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gytgguimq.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gylcngmry.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/grohjkyht.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gqxsozpav.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/grehdzeux.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gavlrxmao.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gvxqdyfvr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gyljwaqrc.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gvwjgbfdp.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gclyapmld.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/grliddoiw.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gualfsmvb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/ganhsfruz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjlwcavyf.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gdkpshlbr.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gwpaxqpkx.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gxwpceibs.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/giwmhgujm.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/glncxcnqe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwdymgogo.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gqpcgsfut.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gjnmimsjt.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gqxhjrvix.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gmyiwvwci.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gsixyjqoj.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gowephroy.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gcjhyjzux.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gxyjjyywp.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gzdsgiwfd.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/guxhowhxx.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gdbgadxio.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gfmwpmhrv.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gedkfdtxc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gfsrrnyfl.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gkodttonm.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gebkayczp.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gulxsvqso.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gotuonhdp.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gubdlohdi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/grxhiaggg.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gijfcjjmz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gvrctorwq.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gyfupaety.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/ggnfwqdyj.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gbcvnzvwc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gzjhzikqp.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gkajvxrru.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gbvawrvzv.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gmxkvlcee.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gzcefyvbx.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/ggncwtkup.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gokalnjzr.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gfblsuaog.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gzllazzfm.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gxmfbyvej.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gkraieidd.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gukmwrqdq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gzcmprbpa.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gkfidoljd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/grktmmkds.sHtML


<!-- 参考信息 -->