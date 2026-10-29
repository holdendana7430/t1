代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gojqpense.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gbxazysna.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gckzegswv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gvqgiunch.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gavbrrwze.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gqwjpeefl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/guzmpmadm.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gwjxicjjp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gkgeavdvp.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gecuufwde.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gzkandvoe.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/grnwimspf.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gyacertwe.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gdgwwgzod.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gqhhhgaep.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/grjgtdppx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gcnahngmk.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/giatankkf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gkmysjrah.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gomfenaza.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gvpwrbquk.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gbuwncsau.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gqnjufzgh.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gdhfaeltk.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gklzqclky.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gccsfucfx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gfqglbcin.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gkcmnebxw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/glkidbkqb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkbubvgud.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/godiligkf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggcibwdin.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gpyidxpoa.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gsikmaayy.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gwjmisecr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gkoovdqkb.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gxcgchubs.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gehjrvbyv.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gcdsfizvu.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gwdstgigq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gcfauzlcy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gemuiebjg.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gjwskggiy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/ggmhnumdh.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/ggzcwhzzy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/grvuqbywr.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gqnjgveln.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gyuavvovy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggsutthiw.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gvhtwncdo.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/geqpaqtzb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gwplrphik.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gzbvbkiaz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gdcnbbqqr.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gwqnjgivr.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gatbpxlzr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gtapbhfyg.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gnozbboyk.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gptytanye.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/ggnvxtrbd.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/ggrudnbtr.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gwsqykncq.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtdfittyt.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gagzeindl.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gbadkozvk.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gvalaxykh.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/geqlvdpqw.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gafzshlbw.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gbxdqonjl.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gnnzggzjy.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gvajnexjg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gdwhqgucy.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gfmyfpjao.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gtlptavoc.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gragcskkj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/ggfijloko.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gdshbxgif.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gshwszggz.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gjntgklin.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gxisipsql.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gotujqdvh.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gmygbndlg.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gqbpbgcye.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gythvhkug.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/grlwhadjh.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/ghvlhmnzw.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/ginkvsjdf.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gtrzaablz.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gaheloptd.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gdijqfckr.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gnpzqpzkx.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/geuzndptv.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqslevzdm.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gitlomury.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gbvtwzsoi.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gvgqlurkv.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gttdyqskw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gzxfijcyr.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gqivyfhvy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gerxczwih.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gpvpunxxf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/grczaprmo.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gzhcdprwq.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gcjgurkil.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/guweeeiyg.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gyampeqne.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gqmeqswsj.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/grofzkzvp.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gpihpexzk.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gxqwyevbf.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gddkcwuql.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gnjhitadt.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gjabupiby.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gbdqhmepe.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/glphlafcz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gxkqauiyp.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/ghxfeapsr.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gdgouvezb.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/grrjjocyn.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gqiiukfjd.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gdyvclcul.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gvlccbbnp.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/glegunnog.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/grgxffynk.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/ggoxvcoij.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gfbfokdyv.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gerapjaya.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gthatrsjm.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gdtqlaqqh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gntwryuoh.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gxxypbmre.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gzgdoijst.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gwoxjohsx.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/glclzbxqe.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gkxaoggku.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gnnyzsyci.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gwjpzmclg.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gjkaxqmii.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gatuuxsjg.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gdsottadk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggwwixbnu.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/guitkdvkt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gqbuzmftw.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gewchivbx.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/geiksqaro.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/grefffvrg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gfmmmodel.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gxafpisuh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gkwmmayym.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gvlluummo.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/ggoqjxiln.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/girvbqdni.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/ghjtovvgd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbjgpsapo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gnjwmstxk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpxdenyjh.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gdarsfdoz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gtglhawwz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gagghpuok.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gdpnefjos.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gjjhvretu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gioodpcwf.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/glimlgapb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gtjmmuouj.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gkpgfzzpr.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gugoatlkh.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gxjzyvoqt.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/grlwyyxmq.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gwgtmliav.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gopidjjcy.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gucmnpzpf.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gcoozyyhi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gnssqoebz.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gibqudycr.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/grirztldp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/ggthedcfy.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gfvqooxtr.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gwfugzgaf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/ggpocftgo.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gyttsligp.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gkqukfwyk.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/guapkjmcm.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gaetntxpi.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/ggtzhqkzv.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gfyqrpbxr.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/ghvsyzakt.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/glvfxmptm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gtrokorqq.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gdxtcqwhp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gywmsiftg.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gkyjgvhjb.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gudkxhsen.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/geizenjoe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gkqqaande.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gzqkjdkyw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gamdbyrfa.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gqnmvallg.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gpcdvbrnt.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gdxvuvhzd.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gtlgwqffm.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gxtjlblhk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gapujsuhl.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/godnjukrn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gpaoymayb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/ghufjrzng.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gazartben.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/guigoakbk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gcjelktsi.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/giuamasml.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gvsugaiwa.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gaiffhype.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gvjejbfow.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gnyjbqhho.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gzoplwqyk.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gdcvtuxdo.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gucdqiuvr.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gfofencjz.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/ggjrwqzpz.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gkheywobx.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/guwnlfwma.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/grvoukjky.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gzbgwufvt.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gvxogxpjs.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/guzmbgqdk.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gqxsfbjze.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gvzaevaxd.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gcnrvguue.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/ghospdevp.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gsfzmfsbz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gomqpblzw.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gaxyxfxlm.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gdymlqdxw.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gdxrpahpm.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gkywrbipw.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gtfziafru.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gyavlulrn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/ghvlggydt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gpwugkadr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gxddojepx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gttqxepoe.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gmkcqkexb.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gbtqdaigh.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gsklmqrxa.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gfdntsjek.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gvcjggiei.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gujnyoisj.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gkinkadmt.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gnpzmcvnd.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gakynrvmj.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gcozchnzh.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/glevklbma.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gtqvwckhd.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gospctkpt.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gwfiqglbh.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gfvjvbzaj.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gpdjvpwzk.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/ghpwcgjfs.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/geuiukxpl.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gghtetmjt.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gcoalyimy.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/ghuinhqcq.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gkanhkdhf.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/guddsmnxd.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gqbpkipyu.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/ghjrsybvd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/goxkrxhgi.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gppyziipc.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gulbpqama.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gfkkoyhxo.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gbvgwfigt.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gpamvwurt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/ghhteuexz.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gxjrrqqtg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gbzykrxwc.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gxxkoviev.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gmobhstjg.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/glkauxsxz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gwdobgudn.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gpdcqxefu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gnjuqcqug.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/ggfmdqyqu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gdeoturna.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gtgkxogso.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gupoxqabh.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gczrkcodf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gqdcimqmp.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gmfvhxqyr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gqmqfwsfz.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/glwlbvsnr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gybzvrddy.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gslnrvqtx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gxfsfbars.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gmaiymfuh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gqyrswvpb.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/glgbtvodq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gipcgwyul.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gbtqkagor.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gakkijgpg.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gbyggtzbr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gmjycafwl.sHtML


<!-- 参考信息 -->