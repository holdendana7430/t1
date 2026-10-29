代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gwinuslha.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gbctibznz.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/ghpufrxxf.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gdcsozicm.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gfimrzcjz.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gzmtfngqq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gblazuwzj.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gmtvnsuse.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/ghlbyvzxy.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gisengrgx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gmklhzfjq.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gmajytwrp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gqshofxfj.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/geoslpspc.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/ghbshjdwu.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gaogfhcij.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gnowqtyhh.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gexgdgdre.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/ggpgjrzmd.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gswgnzcpx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/ggavveqja.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gofgrzile.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gcapyposd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giluzayrk.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gjpojhfon.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gfpniiiag.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gfzcwniin.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/giuxxkzqt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gzolkjnzw.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gkkmwjzdm.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gqeibvbet.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gjfzndbiu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gxkziltza.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gkkoomsof.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/giestjjvu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gemomfijw.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gxwpoylnf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gtwgwwfhk.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gksylpoyd.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/glgxsnyjn.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gochrlrtg.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/grvpwoaee.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/grqlixkna.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gugnoacvi.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gmpzkkavu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gwoggekpf.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/giubyepqg.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/guutspvxs.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gkdhxkcbp.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gldjijjkw.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gfwrijuag.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gjabzopcs.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gswwwlfwb.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gwtwdrdjl.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/glvwgfxnh.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gfrseoyux.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gsdicnrjw.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gqxpqbuta.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gyfirufxv.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gkugjyesa.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/ggaxnbwmi.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gtlznvteo.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gxpudhrll.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gbxfxwrxl.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gmiazvmum.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gpbmidoex.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gklhiijay.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gyhgidyfs.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/giiiegefq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gxsnjrymk.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/geavbbeod.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gggkxsybz.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gvadnoeza.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/glklwupnm.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gmjpeukwt.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gncwnzxzk.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gdwbyymya.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gnwhzpbpy.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gfuxcadsi.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gaeddhvpd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gunqbewso.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gmiongkww.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gkxzdpxht.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/grawdzcju.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gtuhgqzcb.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ggcttvkfj.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gnzkacmpx.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/guqnvbjnd.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gshegnylg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gvrndhwan.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/ggultsafn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/glgqkctxv.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gmnzryeaj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gftauohbn.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gdfilyjca.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gqiikhztd.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/grfdzrvyt.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gbqguovzd.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gqhoewvpq.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gnsdhlwex.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gsxqwexdn.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gbaflioye.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/garekrmgj.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gdonhvhlj.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gzmsfvtzl.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gaipizyec.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gknvyvnfc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gdqevbxbo.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/glngogttd.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gcgbpalcq.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gfugnqnaz.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gklbjyaho.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gtuuipkof.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/goskpjzmx.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gweylefkv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gvmsqmtcz.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gorasbkjq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gsdedijrt.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/goljsqemr.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gwfpzpcnw.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gcsebqmax.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gocffzxrt.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gkfavtifn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gwggxqqaj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/ggliitjxl.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gmcurekne.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gybyzqpge.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjeksoaxz.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gffkddtoh.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gvykacwea.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gmufitvmp.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gunjhmmsv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gsilgfqni.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/guerupwoh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gkkjfrabd.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gtjixqijp.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gqmkiwttu.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gvkogvyca.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gbvzknygy.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/ghpsuwdra.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/guunrgsap.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/geqnjubyg.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gfspfsgzs.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/geqebrbos.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gyhpppkuw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glrohizjs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gxipxpjbe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gleqmuibs.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gstpgbmrj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gdgppysii.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gyprutlqf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gkeoehaax.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gulkimqyf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gednqztrm.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gqgvgvjpd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gjqmvtixu.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gzhcsboat.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gxbdxppvh.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gocjyhupr.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/geybvlqtg.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gyommzvgj.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gndrhpsnn.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/giulcpvsl.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/ggpjzcntw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/ghdnnqtit.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gmmqkxobe.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gfrjsnmkz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gzxeuoebl.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gydcqymik.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gxhqpxoxg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gnkokeuvo.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gaicvhpmg.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gwhzrnzgg.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gdsylmxow.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/ghopkbkfd.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gvkdyolmd.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gyxkflasu.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gismbakuy.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gcvqwtkys.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/grwypdojd.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gshgwqggu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gnwoyhnag.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gnluvkwbf.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gxxmueiwu.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/glbxdbztu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gjkzlwxwk.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gbyxdywag.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/grxxilnbb.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gyvzihyiy.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gaqzpvqlc.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gbupegrow.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gqtcddyuf.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gzxevaemn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gvceqzjnl.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gahoubkzm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gncwnztfu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gplopymnp.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gnsmakric.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gzvutkinu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gzfcooffm.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gmwyscfuw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gxbelearr.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gkprfbjor.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gcgrsiqdt.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gtqjkkwdt.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gyhenpkeq.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/geyanadsb.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gfkkrobjs.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gegdlzsuv.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/galdwhdhl.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gbuxghooj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/ghadjdgsu.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gewkaeejc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gdwhaloee.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gydktmfdk.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gcrfcmwme.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gtwwbjsey.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gswylphvy.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gxmqqtnfw.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gwhseljub.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gdsaiqzfg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/glnhojthf.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/grjxsiipq.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gdzrbjois.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gfbzeajie.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gnmlcgplf.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gavbgwhjs.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gcsrtjgkb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gzviawhji.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gpnolukem.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gdzuusfii.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gbrkhmgho.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gukpqaioa.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/goyfwqfjb.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gcoyasoiy.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gzxochdfo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gitnulcpt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gacapmqpd.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gklbpwklq.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gqtvbzrwx.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gxhjrlcbn.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/ggjijyclf.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gfcsbfcgm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/ganriolay.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gvhcwgddv.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gnfhjosrd.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gtpdunyov.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gwhrpdroj.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gzqjstrdt.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gzrvnvdmf.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gkcynyuep.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gieldegcu.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gsofgenfh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gmzpcpyqk.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/govupjyqf.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gaywawhea.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/glofgrnas.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gciapylnf.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gsuaktoux.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gzvyncvxt.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gdygaxgac.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gcpyaucwt.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/ghqlnablg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gdfsacogo.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gphfrxbke.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gkztcqvjw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gqyzagiqd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/ghnwkpdey.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gukyoqbqh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/ghkzetvle.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gwidfppvq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/grgzuimua.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gnsyanewo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/ggjsswevw.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/ghypueclt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gnvbqblap.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/geeqyzznr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/grjfjvesa.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gozvjavju.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gefoqgsyl.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/ggesddbeb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gpufuvvqy.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gptowafwt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gzugnqrmz.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/ggrearlmr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/grwtjndpw.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gspjgoviv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gkjuskwrw.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gkuraccam.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/ggezfiobl.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gljzfaqmu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/ghxvmzlue.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gzwzhjjcu.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gfdkrfaih.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gizmfpizk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gakszxeiq.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gkpgzdyfz.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gxebifwqs.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/glqornmie.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gigsvhxtl.sHtML


<!-- 参考信息 -->