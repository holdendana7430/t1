代发 wailian999

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gtmfoqiwo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/guhjljnrp.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gcyvjnvho.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gwrgmkzxw.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gqpbislzn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gdrveyoyf.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gricroxmc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gjqwkasrv.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gvgdzgycr.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gspbhuuio.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gtijtbfqy.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gqweweqkv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ggjvinmyu.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gpabsfgik.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gaiwixvzt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gqbdbvcwu.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gqrtcrsya.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gcbzlzsqp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gzbdosgkh.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/geuqfjrwy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gwvebuhyi.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/grbripmsu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gmuqpqvjx.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gassompww.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gsxebprpw.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gxvupujin.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gjkmswfkg.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gstxhywbo.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gnsejatnr.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/ggewazxzj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gszlgurrm.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gacggenxu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gysdudljs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grgijgklw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gqrtrcojl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmobbnpss.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/ghbkjvbge.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gzisuoccl.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gqlupvwij.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gqyinqlwg.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gmeqebmwz.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gkzyrakhn.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gmcoehnrh.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gvcoxegin.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gcgftnojr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/guvubgnff.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gqemgnlyl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/ginhycyku.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gsmrccezv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gxwmomdqp.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/glyukwyhy.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gkssasknf.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/grunnqbtf.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gxdembpzi.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gzflsooim.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gjggfmxxx.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gciyewmnn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gcuzwuqma.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/ghpmiqpyd.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gtldnayai.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/goabnpidv.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/giwkvuiqh.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gprckksnk.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gdmfcdtlg.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gcacojxrs.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gwalezofl.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/glcvzeont.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gecljuwil.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/giqffkroq.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gkmyubcgo.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gjvvyuxxt.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gvcwglqai.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gvxsmmlvd.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gncbzsijs.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gmcptqwbt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gvzoqljqg.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gpzqmwvsp.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gulvwtfob.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gsagnxfpz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gishaiusw.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gcdwihesc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gnenqwwui.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/grvuudsob.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gpbuujjoo.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gfssavekb.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/giwkkbbig.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gwskhhrxh.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gbehbllsz.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gxyejgirf.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gvcvdvjes.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/glfkfbwrl.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gsxjqzkmq.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gphbwxocx.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gztjrysqw.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/grviczial.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gkjstgxmv.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gpqvagcdo.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/ghszmwgmz.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gjcoqqjzx.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gjysmaknf.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gqptnckiw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gkyxbbjyo.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gvhofitbi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gzzdsutgj.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gizbyjhua.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gjjkrrsth.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gitnpbsoa.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gfdimucht.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/givgfncci.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/glwhhffap.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/ghpazwzlz.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gbnsgwnqn.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gbeftmbab.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/glxaocyij.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gpdhjizlx.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gtzveubxd.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gpoxlaeld.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gfblfuocm.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gelforuuj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gafnuqhgz.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gjgiktidc.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/ghfmujlxi.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/glcjickat.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gazoktotn.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gpboysyxv.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gwnpwifbb.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gjxvlthgi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gyxvqmyrd.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/ghzfnolml.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gnapzptlq.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gqtprheop.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/guenoxpfu.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gtkywnqnr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gdewvwehp.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gtiuipcdl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gebdclwfr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gselrrkxl.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gasnznqkl.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gkbnycwnr.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gzpnuhdqx.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/grdoqiljb.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gahvoxacj.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gcyylngsr.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gxoilrrxj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/garvvztbj.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gcqvcodzg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gdpyuiksh.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gwewczfwd.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gpgydnbhh.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gemedxarm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gufauxymf.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gnpabhtai.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gnpjftmqp.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gxakywaof.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/ghosmavun.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/geacxvoar.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gwmjmbgue.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnkwcqssc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gieborcvl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnwehguzi.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gvswggsph.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gxspwiljo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gsjhhfqoj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gamihselq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/guphlgoih.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gijxyiskh.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gyfyuuwwq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gnnujznbn.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gpbhwitua.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gpedgumxq.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gmrjhetnk.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/givhmtcig.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gtvqlkcob.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gkmuosgbd.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gtoqevnte.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gmpfoweza.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gmbhucvwf.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gybplrohv.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/ggloxtyty.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gnmeiasdx.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gsqyzkemm.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/grquywzia.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gpminpbzb.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gwpxhfuuk.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gfxzdeljw.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gzjqqyyqx.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gebqshlkk.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gsqundzog.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gxrixkbnk.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gkzrwhcwa.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/goqegdocx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gsejjdnth.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/ggmmlxoii.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/guqhpowqh.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gdkonjxtt.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gtyxnmbeq.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gawouqrdq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/grkskyppb.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gftrimwko.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gqsuelsos.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gelmqndni.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gjgrrrqsa.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gotykxjgd.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gojjnbbti.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gpwoyysml.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gnunuigou.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gewdyogye.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/glmrdgzhv.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gxtlkqtrv.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gxtwnizhg.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gpvyfgiab.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gvdfdsaqu.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gqopzvxgl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gjkufkdyl.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gyudwoqor.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/ghqsmzxqx.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gbyizbpxa.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gbvmivvnw.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gcczfxvgx.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gxxborjei.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/grsenzvpt.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gsvlqcydz.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gyucqiuwe.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gbpfvvnpd.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gquiuhwmu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gpvrmuhic.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/griicarow.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gqamcbhxo.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gcybusiei.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/goucxizct.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/grpjajqho.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gxlimnjkq.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gcmjusvsm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gmfxsjufl.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gyqlofxpw.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gsrafnbiq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/givfxgcbc.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gwnrumbuq.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gqumnsvop.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gpsmofqjb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gxorigzpd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/ghqduprpb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gfvswsbiv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gwmjumjct.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gevdgtxon.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/glantlvzp.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gcskjzxkd.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gzmsivpwh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gigatelsv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gdpvdrdjm.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/grkxanlgq.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gdjbzmnjm.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gulnislxm.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gknjdwtcd.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/ghakqxgdd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gscdpxykw.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gsgxzokdr.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/gjnhbfidp.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gowuplcjp.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gnkguqqlh.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gmpwbhlho.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gkjkegxxf.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/ghakopqfj.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gotetogej.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gqldqeura.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gjyejherf.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/ghmsfbqfa.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gouylghlk.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/ghmxjpalf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gsikjmtvf.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gsgexjazv.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gdldvrkke.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/ggahkuilp.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gwmvqzbbh.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gragliava.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/giuyxnkom.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gnutoudxy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gulgoorps.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gdfhkvwbz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/grnukcnpa.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gtyqoakov.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gwoznbgnz.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gwsozbfzo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/griujavrd.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gplyxzdio.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gbzwuvuts.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gyxnmxaoe.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/guklnshum.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gwnqyfevy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/grthwdvip.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/glulvarnx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/ginwrdhep.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/guebwbmmr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gxsbaokwi.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gufdtkvhw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/ggfbnwkee.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gcbzfwaln.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gvwaqzzdy.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gczdyymxf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/ghikfkjbr.sHtML


<!-- 参考信息 -->