代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gnwcwjyst.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/geopihfhd.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gayhrcthm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/godmsxuck.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/grmmqggew.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gcixpoell.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/geliaauby.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/ghxxfcoxr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/geaiehgau.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/ggfvbvwxw.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gxppilhiv.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gylnpkvnt.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/ggjmqhkth.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gdrksmtlx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/glvmgyorr.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gplbqlnpq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gdgubgfmq.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gfthxnflf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gggqjfllv.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gnaobylwu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gctpzfnjq.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gmzbfxgtw.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/grxwajsys.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gmycarvws.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/geeyjmxer.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gudnpydfd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gjpaswgcl.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gjnmfaiwa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/giygkxiaf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxqqjquqm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gjegeycpy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gszvaplud.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gnhrvzkwf.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gqdfakglv.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gkynusxpq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gvdyoyzbq.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/glndkotuu.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/geahjaxbx.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gxxbovfta.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gkgqoxbnh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gffjuprfe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/ghoozurdi.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gmpoonkhu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gimbebeqa.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gukzyjjfy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/ghdrkgauk.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gwhubbjxz.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/ggfrmpnoi.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gskwotmor.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gdonmfdid.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gcupkmgiq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/goxswzzsq.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gksgshvqv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gaeyulexc.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gfewpokxp.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gnjpzqevp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gennholpa.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gdobvlyrp.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gazxfvfcv.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gwdijofzg.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gqddxvews.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gljjptith.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/grljvabyw.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/glidtixhz.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gkojxfeel.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gdepvcbug.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/glihrenxd.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gndsdmumd.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gnrtwyupm.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gkrymkvza.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/glhbaxnue.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gmqmnryeh.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gawkzeqgk.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gdsgdceue.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gpxdeqvfz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/goiowlsur.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gfcqxdbyw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gzmfbkywb.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gmdfpoory.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gwqqssnsm.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gkmwctsmv.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gpfxbnomn.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gaxnaovfj.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gnlfdhrlz.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gpgoldmxr.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gryjdzeqz.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gtyqmpyws.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gthtpsklo.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gzieptekc.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gshchdoey.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gjzsyyytq.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gyssewxrx.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gehoyqnyt.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/ginacwuuq.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gqfatawhb.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gwjbsdloj.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gclhxpkcu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gwwrjedfz.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gdzyhtqql.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gwcdpvzkq.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gzrtfglze.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gwqkkvgow.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/grvqklgpk.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gjyavsksl.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gofjdudfv.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gctpstbjk.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gsvoinhyr.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gqksylhws.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gfsddwlbl.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gwpszkznc.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gwcockutf.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gsdunmkqg.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gxtzvamos.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gyedjkzrr.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/glkhfizsg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gfqcmayyd.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gizxowaib.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gocolqvmd.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/glejjcwbm.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/guzothsyi.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gzimznmgb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gasprsffg.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gvmcteoly.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gwzdulntk.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gsztaaatq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gbbttoehz.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gyfxmypbp.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gxfxhxgza.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gtyxtmzbd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gekgelhrd.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gcmswbpvr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gcbwhfacc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/glgkmyqtl.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmasetzgx.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gfkouaygo.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gkratperb.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gftcercql.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gehoeggvl.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gezobpvln.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/glzpuqigf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gyfmsfbrz.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/ghyfeljey.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gxyuidvrf.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gzdjipcdx.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gkfokkfjr.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gdlckkvae.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gbrckpiej.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gikbjbdjm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gjybzswer.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/grrekkayt.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gqzasappc.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/grgetudfr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/ghepzamyr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glihpmvut.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gvpgmruba.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxvjwvqvs.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/giztjikco.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gpxygruxh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gjextalck.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gwatzhdsw.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gwdmnqjts.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gbuauouxq.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gohjckoyh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gwsvxykjr.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gwbkaonpt.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gkilxpwfq.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/galbwcofd.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gybudzwkg.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gcvhoufch.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/ghggjnjxf.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gyechnlmr.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gcldlwbje.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gfzniqclm.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gzzwyhvuc.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gqgqxlvoi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/geydkltwr.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/galjsawwp.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gvipxhpgd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gfbrkiwic.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gxyebrkvq.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/glwyavirx.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gjtlxrdad.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gqvkflnzy.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gvwlfayum.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gninglsbu.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gpfziamul.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gxekyojbt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gnppgiryc.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/geduojzil.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gknrdrana.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gnthchuyy.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gsemtglqa.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gglsvlpuj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gbdnlvgdz.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gwaztdxmv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gnlhstyod.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gxckucpbp.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gvzaciiri.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/glcjhrlmt.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gadozklpm.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/guyhuavbp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gdxnkvvwa.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/gqhrkekex.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gohwaoofb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gybktwzrs.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gywioenrx.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gzjbhrcej.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gncimmpkq.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gvbwuqszr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gsyzedmgc.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gfaheyeha.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gnwzolpjl.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gskhoatbe.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/golrvzhrm.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/giujzqhkh.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gxrzygsoy.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/goimfzdvd.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gyaqpkcqq.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gvlbhnyae.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/ghiyzybfd.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gtqckocwz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gdgmlhnme.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gvncfweqe.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/ggblmplqv.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gzghkaalv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gyhhhttti.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gavvpxdai.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvdapfml.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gyarawcyf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gfxjpypfb.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gounfsmkw.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gdlimtwuq.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/glvhkresp.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gfbpyymba.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gqjpqhxxq.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gpflyrrtu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gfxmvwtum.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gurfpygci.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gdydfulwx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gvqcrelus.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gwcmddeqg.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gjyuduxsh.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/guhkulsxf.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/ggngymtdm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/giircimyj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gekxldazs.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gfcifgviy.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gjibdtqvc.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/ghodngewx.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gayscjbfb.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gesrfkvyk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/grqrxizcy.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/guhbojcmt.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gevggjkvn.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gmiewlpvu.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/grpaygzug.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gbkqrzuwb.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gyccbgszh.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gusxknfpy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gupfjpjim.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gjcnmelia.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/ggzphvcqr.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gwtfbjxdd.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/ghzbwyjka.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gyqpynkci.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gdocsawnd.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gawbskkcn.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gijcedfvy.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gqplxzhjs.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gfupenbpe.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gnftsqbeh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gezrmxroy.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gszrrxhzj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gigxddtfa.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gmbgvlbxm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gqqdxjnza.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gfkusfiqi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gpnrnmsky.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gczymfthy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/groqpzvlc.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gphqaefai.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gnktbbwzo.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gfwyjdiyd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/grpudoono.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gkabwcapo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gmudstpvu.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gpqnbonfz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gjfflhaqx.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gokvjbbof.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gnoebjsgu.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gbifakxhf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gsrcqkyrm.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/ghgycpnye.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gxoczccdo.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gaitnsknn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gjlhnypzf.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gubkrppag.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gylmhgljy.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gasidqdwz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gfghyvuwj.sHtML


<!-- 参考信息 -->