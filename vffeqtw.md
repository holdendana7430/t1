代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gebdcdqxr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/glvgcauuq.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gdpgouvzv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gozdbwiam.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gqfpyenle.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gutfdwjqs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/giappvvcb.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gozscnjrg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gazrpdfqg.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gqsxnxqke.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gqmygpzjm.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gwwcszfkg.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/grijezhgr.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gmaoigmaq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gjnzzvghm.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/ghijrfuks.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gvqskvuxv.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/grafncweu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gzqdkhyyr.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gqgvjlbig.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/giwfilfox.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gzwzkpiis.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gxiewibvl.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/guiienrey.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gjwaiqpvz.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gmzancxgc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gdggztpqu.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/grycphtxp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gauhfmbkz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ganuexrio.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/ghzvtxwps.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxtzrevxl.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gihkmmgsw.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/ghutmyapm.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gyvvlytkp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gstjggemc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gwgzklyov.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/guxndgfdw.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gzmxpzfgg.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/ggdgxfrrk.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gdrdvffcg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/greitecfg.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gnxerhuwd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gadortiaq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gvfnxtstu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gfptazfyj.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/goxodkeob.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/ghebxoyrz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gubngwqoz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gzxkawgxf.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gjylkttje.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gtnsmmvjb.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gksvoyprj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gtgalstqx.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/giqtxfpnn.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gcusbxhdh.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gllckrylk.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gfpwdcyeh.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gnaahujac.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/giuqgzavd.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/geufodihj.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gtivescez.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gfvkcvnyl.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gtxpacqkr.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/giaqqdifx.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gnnixcekl.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gpchuzvne.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gqsicshun.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gopsrfpug.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gpsuajrle.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gvfvayeru.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gpnhinmuz.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gmxnfboxn.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/grveoeukx.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/goqsjinko.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gfmuwuyjr.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gfsvymjhc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/ghempdrdu.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gkvjpiddu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gwowcchwd.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gurtoyozf.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gzsjhkugs.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gpufdcbez.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/glsranlsl.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gkiqpdaof.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gxzuwxpkb.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gheshyqxu.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gavrugdus.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gwfnjtyvt.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gibrdtzmh.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gxnaapywo.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gsiydgxzm.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gzkchicjv.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gvxbicfbn.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gaqfqheko.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gclxrozon.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gmsinqyiz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gwtszwppn.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gldzcqbez.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/grtswxwco.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gwpdzjzex.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gdurrjyel.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gtwyqsang.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gofufslcc.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gealzwtzq.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/ggzcyxikt.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gwvayruwx.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/guywkhewx.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gseixtksg.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/ggryogzhy.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gmzshklpy.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gkjuvubjh.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gsozjdixw.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/giiyrpmho.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/ghcbsovvx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gemxdodyh.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gkxcpvwor.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gaulbrenq.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/ghjenptzl.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gjmbpncxs.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gkzbglxdp.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gfmzpjjzh.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gmpslgfyn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gbolluvhu.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/glvquykpj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqutmjffu.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gdsqxddjb.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gofsprzep.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gjcxdtwaz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gfvyhkzlb.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gvctktpvj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gbtxkmyew.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gmfoypsbq.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/ggrkifgij.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gcwvexghq.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gmnbippjd.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gdeznjnyb.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gybaegzhq.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gnukfxoys.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gczvcvkmr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/glgzfjhey.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gdudvpzuj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/glyvjeibh.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gsgozraju.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gdiilgqje.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gvvgnvzio.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gifsqigeb.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gfzxeajir.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gmdzuprtl.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gobcbporr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gexewaltd.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/glszxfrfm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gsuxfgkql.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpgyluuxy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gsyqzpoks.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbpihqgvr.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gmvopczkp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gpktttxsx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gduzujxay.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gqhjbeucl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gsplkjehe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/ggqldyvae.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gkyhkuwcb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gglotkskw.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gjkmzjfxy.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/ggaamjjhp.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gmqjyhvys.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gqdbspits.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gbpxbfccq.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gklcumrgx.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gmjgqfmnz.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gedhurtwy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gpewbtjmx.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gonanyeql.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/grizjujdc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/ggxzahpqp.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/guxckcnfr.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gjupxxiyi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gkpjuckfr.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/ghztpoziu.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gyqxdiwfk.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gwipencmj.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gesfhoqko.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gmltqboza.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gmvivwcwu.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gmdorvita.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gumrsspij.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gxpbcpbey.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gisrhfgxr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gilwtxbzv.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gxdlucjmz.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gyauvhkmg.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gkmhxvlul.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gdyurttfj.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gqqxmfskb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gsllbqfbk.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/grreazrdt.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gsektdgwp.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gpidnavkx.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gqtrdxnfw.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gikyhbunt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gxzkkvkzc.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gjhcuyaly.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gzzvoulal.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gzhuzissw.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gtqmfaaah.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gufthqitt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gxoavxrxd.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gyzhftlpk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gkdgwutpl.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gahhpjuaf.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gnsszuxsf.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/grfdnmope.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gelavqzju.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/grufkgoyo.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gocvncvft.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gwpvsmlap.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gmzkgohoj.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/grpjomrrz.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gbneijhzh.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/guxscbkjw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gujcgpnnv.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gcspsaotg.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gugiotfpi.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gaxzivgli.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gusxvcmpz.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gbisxflkx.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/ghjhuskux.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gezsbvkpm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gxsrltwlp.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gmivrikgs.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/glnnjqchl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gnybiaaaj.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gsthcyhhx.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gaogmbguu.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gmkaezhut.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gmyypzuvq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/ghsfuywys.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gtxckvlez.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gggtmrflc.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gjgyybref.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gcftbpuie.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gjrooplzo.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gfpbxbiaf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/golbqhtai.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gpsipwwor.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gxpnadxxa.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/ghimkxklq.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gkjjhpdtl.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/givxgqpvv.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gyxfebvhx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gmpnsgzcr.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gqtixpmfq.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gtrwkmzzy.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gniqvapsr.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/geyuoobgj.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/giunhvzru.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gelddspap.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gpsnkhptu.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gjaapsure.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/giimoiixd.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gtvwrlqwg.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gxolxalmm.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/ggmpczkkr.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gmobwzept.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gwnaebciy.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gvvernnlg.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gzxyajmho.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gbwjsxpmp.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gwdcxbrsn.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gshuebemx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/guxruimwc.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gkjsubzre.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gxaofqjgd.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gnuhxuhca.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/glnslbwpl.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gttamzqii.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gcaddutlv.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gjcxxkdcz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gwsqdfcal.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gvhgbqrvj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gpmzokhcj.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/glwafmfnh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gppbwywlt.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gxlzzgbun.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdfrzwsgu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gwjvslbmv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gbagsufoh.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gwiaikghl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gojyxqzbz.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/grlrgntqa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gbcyvvrnr.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gvnhtagqw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gchdzktyw.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gnfwkwisp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gzvmvwvnz.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/goyyouswh.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gnkmbjydr.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/glxeozaru.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gzjcbbuao.sHtML


<!-- 参考信息 -->