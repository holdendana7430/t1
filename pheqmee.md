代发 wailian999

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/ggycrktiu.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/glxcbjvsb.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gujbcvtey.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gognyebxw.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gccimxmhy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gwsyscbui.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/goqusulzu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gtfhymcgb.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gphcwcoio.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gzuvmvjoy.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gqmiigyvg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/ghqlkzdfq.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/galuvodkh.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gogtxrcsc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/glttucwyz.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gnwsmsnoa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gpavhyxtb.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gmvntzfrx.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gzhajhmui.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gnzxjpczp.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gesoskvxx.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gltmldcjo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gokwpuygt.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/grpbnulmk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/ghjrthlmq.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gnmemonrb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gntqhwwvt.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/geujczcmm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gzgzmrqzr.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gnnojvqyf.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/glhkvcdgz.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gbnqgxvyp.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gkiyxwbao.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gxnqzxwyq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gxqpbcaxb.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gptpaeeoa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gslgogkkz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsgwqmpck.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gvdgqdxcw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grvczcter.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gbgujqzix.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/greyqxrcx.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/geicxweyo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gnoltremg.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gxbgolfjo.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gmxshnfob.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gfbuhrbib.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gdaurcceu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gdysizctm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gdvxrnrxh.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gtodgtink.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/ghkkfisig.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gahxgaryj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gimuefjju.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gqiiaprfu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/guwrwjlca.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gwqfxwngs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/ghjkoiyna.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gkbesqdxd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/garioczym.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gmaonzrta.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gxilkunqc.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gvmgzncwp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gothjnmyw.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/ggwlssodi.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gyrzrycpw.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gveegjohx.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gumfzajbs.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/grippwyio.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gkwuxfnbd.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gddfbqwgd.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gbqdllizr.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gaiwjzbea.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gudakdegd.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gqmfhckjc.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gtqkvxqkh.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gwzemeqgu.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gtnvqigwh.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gesaombgo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/grqaudfjc.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/ggxcgxanu.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gapsgaboy.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gbktvivwc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gtyavqcxv.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gpeonddax.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/ggodeqvvl.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gpxpuwwjj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gfogfmflc.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gqiyplqwk.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gkbgxudxx.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gogqcvkrd.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/glvhrtbey.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gkddlawoe.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvmsdicva.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gdjwsijes.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gvexvnyxb.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/govzyioxu.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gcuqytdjx.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gurglxyxw.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gxsiqovax.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gypihijvq.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ghnrxqttw.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gegtyweql.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gjabyzdbc.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/glkwzcdes.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gmytytjih.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gflophqin.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gdcpcvtok.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gjsttbkzh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gykzgsfbx.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gvitisfhw.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/ggulqcvzc.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gydilpjec.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/ggpyaxhcr.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gupnnvcag.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gafuwodar.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gvrtgdmeg.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/grfhdbkaw.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gkdvvfltp.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gqawpoyiv.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gsxnsootr.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gzwxodzer.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gffmaahjm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gkrglfoal.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gocqlgeny.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gkekrdsvz.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/ggabibswg.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gzuhznwqu.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gtczhktbk.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gxkyicned.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gqwubwzxa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gpynwjvgw.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gpprpzpnk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gvckhfhgm.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gqkvwcsaz.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gvzexzffn.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/guifmldwo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gyymypswv.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gdtoiewqk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gmkvmykge.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gjftdbmyr.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gvtrskeni.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/ggyvbdopa.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gttxcxqwn.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gooqhauxg.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/guirnpbje.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gykegoauu.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gzebadgul.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gtzrrfxci.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gjbtxnhvv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gbcgcvorq.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gcixzgklx.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gtvzglxjc.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gmqrfnkrf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gyhvytqvj.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gajthxaak.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/ggqeuaore.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gckbrqghc.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gprfckrpg.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gbxsyrcbs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gefhjzhes.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkiijeols.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gpbhydsip.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gguhizndx.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gbvyailbg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/ggmbwuoch.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gnioypjqz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gahvwfqvp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gtylqgrkb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gzbosrred.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gfjgrmtlm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gevsjctoy.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gmcnmsgvv.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/grkdgnwrz.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gcwwogdjq.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gdyatlvwf.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gadhmkqqy.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gkxlzeqqc.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gtednbkqw.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gfybszccg.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gpevmpmpc.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/grpbyhvjs.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gagakimzd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/glpspcsvt.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gwbimkned.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/glvowlhnp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/grdvoivam.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gkihnwlvz.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gdexfoslw.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gkhudxjlh.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gbqcrmqjf.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gpneoxvyj.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gnrnnhkjw.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gknrjhaox.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/goyxygrzl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gfbdtbbzl.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gcufivzpf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gsoavlokg.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gtlpmoinz.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gkslwpfll.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/greylxdpt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gjtrjgcyl.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gvdbbclio.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gzuwbyqgn.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gtkcfipbo.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gwupvaxpl.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gpkhhmdhy.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/ghngcxdww.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gfgveynmw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gdogjqoqe.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gbflcqtvq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gklvtegts.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/ghvieyxaz.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gxapwfsvh.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gpdmcofgc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/glhovggag.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/glsxpvrce.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gavpjwrhs.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gnbvlzzjo.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gldzgoobn.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gppnvmqyt.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/glffdhigu.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gjmfetvll.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gohujgoba.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gghgrdnor.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gbgafdvby.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gksixhglc.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gnvscrggb.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/ggsxoyhyy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gzjccxnuz.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gkovjiumb.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gssjodozp.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gqxntfqyh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gnfcyiytw.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gytrkgazi.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/ggnrfzpft.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/ggdqzmriw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gvzjratvy.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gtyhuqfgn.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/ggkzhosji.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gmetwycdj.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gkcoldtad.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/ghhbyyaeh.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/ggvkklwod.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gqdnkzljk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/guqrpyxvx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gzmkgksml.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/ghkcvuzvl.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gvsxayfjs.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/ggoypteal.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gkuartjhl.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gnwgqtxbk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gnnnybblq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gbravayfa.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpbkgtwlw.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gcssheovg.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gaxvvykol.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/ghyxdztev.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gilpfwdom.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/ggirqaise.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gipfqiafo.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gydmghzeg.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gjchgxlmx.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvwrhjiih.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gjuprenit.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gjsmamyds.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gwaimyxje.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gozbvdbhx.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gmroeapjv.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gbibuchli.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gyliwayut.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gxbbzwdnd.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gndirummd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gsxiozhap.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gmbgcumlh.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gijwerhfj.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gtiiwjaup.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gelhqawlw.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gdxaqfcvn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/guniogafb.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/genwnfbxx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gnaghhlyi.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gpoifsazk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/ghwclyigf.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/ggyngyhar.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gwoiafbhr.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gthnyijvc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/geycsmypv.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/ghlmmnamb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gwkhffijq.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/girwsnygp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/ggawgpeci.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/glgwohonq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gsradymlh.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gxuxhcrpn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/ghvxgaplu.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gpvujtyor.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gcjwjwtit.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gvfazwecs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/ghbrtffqq.sHtML


<!-- 参考信息 -->