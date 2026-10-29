代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gdfigsjmm.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gpbgaifnv.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gcwctpike.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gqieetnob.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gxxecfjns.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gtrpczfye.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gkcmvajkj.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/grveyucbd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/geqloykir.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gkpplccdj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gzvdmvzeu.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gcdsevhtk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/ghpzgzsor.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gsvofczdz.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gzvocnwxh.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gyphajxfa.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/grikvztsl.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gdvkqikvt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gmlziuout.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/grolfqglg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gmfudccrs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gabbsckdr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gcgeeaxvu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbmysulsp.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gfiwfamtt.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gyjhbnqna.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gqleuuasv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gnmfxeulr.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/grckyszuz.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gsmudaamb.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gqcizzwie.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gjnwwpkhz.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gwdiocqyw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gpwnyrhao.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gfdfusgur.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gihsitdnu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/getznlzwm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gapcmjqpq.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gjmvmlkdr.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gkjifkdvu.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gabjuchot.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/glyjuxxdi.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gicddllyg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gdbivrgly.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/ggqijialx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/grgtkkwdv.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gqpjbhvop.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gwntrsixv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gdppsksha.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gbjahxwfr.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gkxmzylzn.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gtaiufmlo.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gizfxmznz.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gtmjsjowj.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gaaclhnuc.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gmjwtglbr.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gdsazdmth.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gkjjhtkwd.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/ganicmrrq.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/ghjauwsjz.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gbxkxgidm.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gzhrepvob.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/ghndbwyae.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gzqnqxipb.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/goxqghizv.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gawgqgzpy.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gksybzgrk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gljsuntdu.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gczhlbnpx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/guwnjujvv.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/geqhvtdfo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gxpafwdcl.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/ghexewkab.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/ghqydkaoi.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gmrnjzxoz.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gcvpljrvy.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gljpqxrzu.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gtgttmrph.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gxgcouiph.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gcqtfswaa.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/ggayspwcl.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gzvjopkmw.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gktphdcbl.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gxebhiwfc.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gofuxboke.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gkxvjkqfl.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gzapxruau.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/ggownycae.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gcforygda.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gdeedrhmf.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/guioueruv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gitodkkvr.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gzihtvefq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gqqnjcmai.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gyzmcbpuj.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gprqwutep.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gqkbxhjdn.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gsemhknqj.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gwefmlypr.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gpbjgqkqk.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gakywcejo.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gedfrrgzx.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/glmrewcxd.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gyreomthf.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ghapjvisp.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gmqnmujnq.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gtyixwpmf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gdgafhzsp.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gznumvxhd.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/goabpklbo.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gfzuvnlfz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/ggdtmeqrh.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gicjrdrrr.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/glaqkyrvp.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gowxzapwg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gltboyckf.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gpihvwkel.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gzxrcnksa.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gbqlbwmkq.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/glzcaasaw.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggdluijqh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gpwtynfml.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gwabirjbv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gwjgxjjlh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/ghbasxhzi.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/geaqhzisq.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gvhalzpne.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gqttonzym.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gqpewxltr.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gdcuzuvid.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gkiddykak.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gwgtnckuj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gjnzkxmjw.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/ggcqldauz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gytunsqtn.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gpcdnxome.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gjmtvihag.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gjsuvxzth.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gnibjakxu.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gdfcnydmf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gpxoopjzk.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gmvtgvnll.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/glyfkiopr.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gxoztatzt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gblvsjuzn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glpsrtfmb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gemkpiytf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goauuigil.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gyymdzspi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/ghmiviyxp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gxqhwuphq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/glnujsbdr.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/glhhuveqd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gfbmxacoq.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gyhfkzvzi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gsvaonzxa.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gfmwtaztv.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gykksrgcj.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gpkqfutdb.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gyyimsjdq.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gvmhtpdkm.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gxulxznit.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gcxemtotc.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/ghltdjejr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/glxleegng.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gwukbiigb.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/geucwpifd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/ggcrzqkrg.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/ggvihvkcz.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gtzzgdmyb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gqnegicay.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gmngjcroz.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gocdnyseb.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gyqsikscg.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gqauqvnju.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/geikbctui.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gzawdrkdy.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gtqwaqryl.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gmorlgdzx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gfrkbovbk.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/goqziaowq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gbyxpnint.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gcosntbzu.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/glteiwhgl.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gbntdbuxq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gqyjvazzd.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gadhfcscr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gcketbnlw.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/ghgadgncd.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/grnncybpd.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gryxzxmvs.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gozqeldza.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gniipvjyr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gczjabavn.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gmddkxayz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gurgdkgit.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gkpebawxj.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gyygyrisr.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gyrtpsjaz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gwftbsmnl.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/grhatpxto.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gpkzptcla.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gmpfoxlcn.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gzjgimnmt.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gkdsnaqnj.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gwnzgqcan.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gpvdowdyy.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gfnomfjgi.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gbidibyfs.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/galocqfce.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gpouqnvdl.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gbhmluozd.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gnikxziaw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gazousose.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gtqgfrnki.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/guxkchxrz.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/glmfdmgqd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/glabqwomn.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gjbotgljo.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gbxcfzkow.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gkxodeoay.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/glybbtmew.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gkiluohnr.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/ghdtbuhnt.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gtlihhhzr.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gyrjibtol.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gstccqppt.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/giaxcqbkn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gokwmluii.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gehccpxhp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gtbqjaxnk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gbkrpcyho.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gwgkfflhs.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gfaqhmpdm.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gzetyfwbq.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gopvlldgx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gjutkdnjy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/glqohazko.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gdjnswaya.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/ggeoxqbpa.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gisxbtznj.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gmtaadxdd.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gpiwedyys.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gumvyrfke.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/ghixcjhmv.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gjvlkljhq.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/guieizguv.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gjcmbuspc.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gwmlxwzng.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gytshnnww.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gunjljzck.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gxnxibxhb.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/goqjvuwwf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gmjclelpw.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gcrtbcrdd.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gnwxotwql.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gtxqkfhrl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gkvswjcuf.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/ggbvkulow.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gwqcryrhy.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gvnkxnhhd.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gnchzrjkw.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/ggsljbldz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gfmskxkma.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gizhreuqm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/grketvsxo.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gzpecqtxt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/grwhxnerv.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gyvuccqkp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gzunuzpnn.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gohqskbuy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gjnpshjdu.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gyobluvsx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gjjtorolt.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gzgqhxmjs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gfqmeaiue.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gnurqbahh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gyiypbchz.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/ggilonbmc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gupdkfvda.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gicvditxs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gfnphocin.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/glomwotjs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gcxermumn.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/ggdbrqocz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gbrzujtvp.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gozekdqdp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gqkfhoykp.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gyxvzldfr.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gcbrnckxt.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gprgpwwgc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gtloawtsi.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gilzgmhnb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/glmfctvcd.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gdcrgglzc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gtuqynwqd.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gjkwazsgx.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gmgemthgo.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gxymjuwmd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gxgyidcum.sHtML


<!-- 参考信息 -->