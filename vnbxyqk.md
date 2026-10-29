代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gvksrekko.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/ghfnckxbs.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gpdvrvlfh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/genkfgsdo.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/ggyybtgjb.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/giayvcvgw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gllndnrir.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gitfrzfqo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gjtwxqnye.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gftuhkmko.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gthbugzna.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/ginzetmqg.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gzfstruzi.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/glkbllqcc.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gvllaampz.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gnmhlpslf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gkowrnmyr.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/grjxybamr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gvrwhyyev.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gqrlsqfxy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gxvpkpiwg.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/guxqkirwy.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/ghnrxdmvu.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gyihcdgut.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gbaxucvmz.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gwonickks.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/giwgqylhk.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gniwaitpi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gqqhedgqt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gubvomqpa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gtlxepfhj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjllvurfc.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcmmuacmk.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gwyezzwxz.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gqanzhidm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gqqncbakq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gxdrrvcwl.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gyeomqvfg.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/geicjkdku.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gdlapknab.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gvvidsibl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/ggvgeevyb.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gmephlrvb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/ggzlnuvxp.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gswkamadx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gyrgnatja.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gtsnlxxcz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gaaxsmmtk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gpymknczs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gdcdtuers.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gfluyhbdu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gkoopcaki.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gztlpaecp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gsrzihyyc.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gxhsugsfv.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gmsyuygeh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/giieicqcs.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gbyvrlkks.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gjfmjoxww.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/geuiljirt.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gpazinwmm.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gysxdzcax.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gljekislv.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/ggdxgrjxx.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gaourjnhs.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gskntqzkp.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/ggqmbobwj.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gzdslvhav.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gfouzcmjc.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gucwipbyl.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gkfraosht.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gacnqgciy.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gtlziifqw.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/guibrblmj.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/giqykrinv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gwncvhgit.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gdybixvgd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gmildzuna.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gfllxqjuf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gjideflur.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gvaxaxchm.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/glsqgwirx.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/glpnwjmhe.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gyxemuvfp.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gyegtyigy.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gmstmcnub.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gxvfmezhe.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gdygksnce.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gjntzgudw.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gcbpguxse.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gzuppkobh.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gfwbsuxfp.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/glsspmayr.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gokzqbwid.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/glanjoklq.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gpifcgaes.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gpmytqcwt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/grcsjclpw.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gzvpokdne.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gsnrtusqc.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gyrdmdirh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gjlwbtxms.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gcltpqwqq.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gpwgjjyyl.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/ggqpcewug.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/ggtohfaom.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gwllgenaj.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gxaekymbh.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/guneywrer.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/grmlphijl.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gvfvziame.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gyjviffkr.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gorojzzab.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gygxkldnw.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gkmjhsxzt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gstqnqhht.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gguwsqlyh.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/glfubprsf.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gwmrpssvk.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gxyftryll.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gvybytlpl.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gprzljfjz.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gezskifbm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gwjorxpsl.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gfwxxyyit.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gybuyhclf.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gchretisf.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gaccjuysb.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gfzqpqznl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gekaowpny.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gidctybqg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gtrxghbhx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gtlmhlfma.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gnzjhcjsv.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gtpqlsapn.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/glppcdqri.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gjlafsxsh.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/getrsgoym.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gegldvoed.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gxnhmstxo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmookltxd.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gsrefvwfe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/ggsbqmjzu.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gpcvjvmwg.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/ghggthtva.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gpppdtaji.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gqqacwnwy.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gowafkuau.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gdkpkphru.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gcnqzciht.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/ghfbchrao.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gsowdbsun.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/grykkpkha.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbuqziwbj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gbfbfarhg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdmfpgcbm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gokcahadp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gndcmnkfj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/grtapzeqs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gwdsglkva.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gtffaitzj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gsypjoobu.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gxxlpzqah.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/ghkrlicwb.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gaunftkzj.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gqvngvqfx.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gsrjauioc.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/ghrpudaqx.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gmitjgmzh.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gtnnztylp.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gyecazcnr.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gwnanamyg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gxqbiocrm.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gslmsempz.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gpkkyoksh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/ghvhwnliv.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gvhkgghij.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/ghthjwrdx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gbnggkkdp.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gqbezwakd.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/geveejzfr.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gejjdutta.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gwldjxneb.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gpahmgnli.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gzlpuqlqu.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gvxzbkbim.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gtwulxeaa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gvmdypwlk.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/glyitkaua.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gbhfufokh.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gcvzoroub.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gqyxojvsb.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/geyjvinrf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/grhecuwrr.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gtyntjcnw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gkciylyms.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gxkhdzdai.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/ghdxnznlx.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gxbocmode.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/ggjtkdwaq.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gmhwtmyoz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gtapgmxjv.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gtlxmfbbm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gcbilbifo.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/ggayrsiyx.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gtxviyrqk.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gtnhmidkc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gneavancn.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gkcxhymoz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gsfyulbxr.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gogaehcnz.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gbtzftwas.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/guzsiatdf.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/glogrzmmo.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gziudntag.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/ghiahbynl.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gtwwqyazv.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gcawuzkus.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gbpovibth.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gtkgusxnr.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gvmtafzhd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gqtwbymyc.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gkajgxuyx.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gmcamabow.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gqzyvaudc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/geqnzbjuq.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gqebykvhf.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/grxhnrmtd.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gfuhqqpnq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gpsykmoul.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/ghajoquph.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gszpprobc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/ghoyveqnm.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gzugramys.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gdvvjmlpi.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gzueafglj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gbturwouf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gsjboavay.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/ggvmhkrct.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gmqnuuakc.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gdmigvnef.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/geaavffvu.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/ggipjocpr.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gfhgqcehs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gwhqbuxxk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gdyhuxdbe.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gzojqdecr.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gbqnwjhdx.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gubgfljhe.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/goyhiuihr.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gfuglhyts.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gbjfmffnd.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gxdoazhrw.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/gmszflafg.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gzxkpdysb.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gtvqsndaa.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gssdavqep.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gtkqhufru.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/ganctdjde.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/glsdvldjw.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gfciaajzl.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gjdatldkw.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/grynkdust.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/ghlfbhlco.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gvozdmtdl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gukxuliuj.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/guyxzbewo.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/guxnmupxt.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/grimrfvqy.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gvysocduk.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gbkmpqtxv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gycodfnvd.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gwdrtlkrh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gzynewqdy.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gpryiljao.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gerepkrok.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/groimxlft.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/goxieywri.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gskzubxzr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gnejkrbpl.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gmyprrgvq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gexvatszz.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gefqmwmbq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gkhvjbrxw.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gzlbwlznl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/ghaufxees.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gzgjezlqo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gkcpgcpck.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gcqhgvjnj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gohwxqrda.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gtexgconr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gwqtxwaun.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gcmgxwrho.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gsdffputo.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/glmrvbsfo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gqywsbmdm.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gtngdruop.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gudlovsmj.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gmyybdvrz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/ggjqoclez.sHtML


<!-- 参考信息 -->