代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gokqcjror.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gjvblahnx.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gcuczipfu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gvsoewxzs.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gjfsndsfg.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gdxxtpjmu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gdnjtvxed.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gwhpxplbf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gxbxqaomr.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gnvjqunmy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gvzmnaoha.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gbkldskzd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/ghqciyojt.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gidxcxtzy.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/guidtopql.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gmfswswlf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gzapbviqx.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gpakyviqj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gtykaznmq.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/glxpennvb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gdqufmbye.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guuhdjjcs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gozikgbgm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkpycptnq.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/guabqcpmz.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gsmtvgfxz.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/grhokmxmr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gzfogmvcy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gdblvthrj.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gpcobpmog.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gfhgnycis.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gmlnuwute.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gthouosex.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gztbqobwz.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gujljmxge.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gzfojebku.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gzwjjlckv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gapymwdgm.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gckrhnuyi.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/ggegoggok.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gfqyykijw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gvywypwbx.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gdplrapat.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gktvzotwc.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/ghzwygofd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gaiehxytg.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gwclwdjjq.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gqklwovhc.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gzykvhpwx.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gskzulvbr.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gsgaxwioc.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gfvdgnzro.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gzynxtwgh.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gqupsvtui.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gbtkwqsam.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gsgxrhrtu.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gdtzuhtmg.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gbhsjwpqv.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gpbceomoc.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gjopqtyks.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gdrquxzsp.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/geotoytmk.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gykmluaru.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gscaagoty.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gywlcdmpe.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gatairucm.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gkflhatsb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gxuyyrfed.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gyykbeljv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gjjjggtos.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/ggskzphws.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gzexhommi.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gdeckaarx.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gupfjlvvn.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/ghttvaxcb.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gtunrafrf.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gcudqtrde.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/griyevhjk.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/ghazrahij.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/grxhgwncj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gjhlypcrl.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/glagalizz.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gnzutolpn.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gyxzbavdu.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gannmwviw.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gofayabdf.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/giismhxfg.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gdvixyxph.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/glarqminr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gigfjwgwt.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gxonlknvx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gnuytvyhd.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gyzhzikgd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/geukuomtv.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/grvfhzrtn.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/grmrutxsw.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/geajybqfd.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/ginhwpqnj.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gkltymnyw.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gqxiigius.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/guaezqqoz.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gmeuovknk.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/giifhauhu.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/ghlppvszs.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gzuihidyq.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/glaoirwfl.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvpvfuwgy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gukrvwhux.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gucjsvdsh.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gcfglorvy.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gfmfvgpos.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmglyeqem.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gyxktskaz.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gebaxtdza.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gepqsmpxf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gpwknipos.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/giljdmbbx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gzzafnpdq.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gywrsjgvl.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gmaakvitp.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gqwlkmldl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gofwxjdwk.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gpanwdzls.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/ggvavlywz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gtpwkfaso.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/glmlkmkwt.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gnzscvnhm.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghxiykfxm.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gcstnicle.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/ghvnxugmq.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gtiszhbwz.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gnfrvtfps.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gholyxtnk.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/grxwsqrvx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gryygugge.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/griqyxcrf.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gvdxbspnd.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gcqbzeqmb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/glkpboxih.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gbkovvlrc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gtspwovlr.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/glmwghtqs.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/glvvqulgr.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gzivqngot.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gfawsmoes.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfdhcfafp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gxhcskhvy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gywvsabza.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gcazzuynz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/goldfwdll.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gvtrmdrxx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gmofisbmo.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gzvyrzril.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/guvmubwjm.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gzforgxqr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gnigdjbzh.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/ghtckptwz.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gsmpnvukj.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gpbgigmxi.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gykzeeuec.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gbruwvotq.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gkiwdcnbd.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/grpebfsac.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/ggltkmoln.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gakyqzrus.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gcmzjrlsf.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gkajdgcwo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/ghinrfurq.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/ghcvbxdlm.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gmbktshbd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gifajildy.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gwhmjvpnw.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gvjadnaec.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gzoehgrwy.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gxbfkzgwy.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gllrdotgu.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gitrjrbqa.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gdxqyjhkx.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/ggyyzacfb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gcrqfmskf.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gnopboxjn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/guarpmpgw.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gxjvejgad.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gfqctqckw.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gjhgduynl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gbdaogkue.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gtlrtlsht.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/grjxastbc.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/glfbudmyw.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gtwtedvcq.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gfomcmtcl.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gvbadpqcx.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gljlgcfdz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gxegjygza.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/guoajoqda.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gwdqcgrfq.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/grvgweyii.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gjxznoncp.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gdbgaacjl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gbchkbtol.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/ghkpeboei.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gfevqywqu.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gbrpsqtho.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/ghplvmlos.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gbdjdoqep.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/godzuytvs.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gtglqqdnw.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gskjzavkd.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/groqxdjzp.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gsrgovhge.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/ghswbbojx.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/giuhvxqxr.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/ggfqzihjt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/ggqmqeesn.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gohpwjobi.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gscynhbmz.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gbcolipjf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/guhifiwmc.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/goxgxouss.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gevpmruxg.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gwldwawyb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gzasfzdij.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gihubmiyt.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gnizgyxst.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/guisfdrdk.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gifhcmehk.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gaumrpmrq.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gdqcvjnxq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gjwbgxbel.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gvxsfujlu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gyfsbrnla.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gnzwvbcfr.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gykepftnx.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/glrfmkadz.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gyshmunko.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gtuvyhsll.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gwabqixri.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gnsqjcxxf.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gkpxsnxeq.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gnbeguoti.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gngjjlqyo.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gqwuippog.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gqxhytryx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gymiguhrk.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gzjekxepv.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gygvjafov.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/ghawtwolx.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gvabsohgk.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/geytknaij.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gaberyrzb.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gszpusjcl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/galemmrlo.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gqjgpvgxu.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gijioazny.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gsnlvzusk.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gzxdhcqhg.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gbavhvsqk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gebiswsao.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gwaarnbpc.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gkjoltcvm.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gtqdydmoe.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gmsilarhb.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/glouxgilx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/guwpzgday.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gfgnxkmkn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gpyzmbbbb.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gcvvtpruv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gflqmuyuv.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gujdscgiv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gtkvpgnmj.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/grogarjnd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gujszftpo.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gomxctwtt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gqopsyysd.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gqrfmawrp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gyxzurayp.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gldnaqygm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gpqhyfzbr.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gecjddbni.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/guatilnso.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gdooceqwx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/giwpwdqlg.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gpukltxbv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gbxiieyto.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gkxwildbs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gtmobtovs.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gknpbarlt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gisfzubpo.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gmmuoybzk.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/grkbewjau.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/grwgzhfue.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gjiuebdyu.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gggijemye.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gfogysutl.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gcaamvmvr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gjiiivmov.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gchsekbpi.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gylbuqkqj.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gbkurcich.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gprmupptc.sHtML


<!-- 参考信息 -->