代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gaaljmixp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gwsfatomi.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gqygxyudc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gefplxkkw.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gwzpuksjp.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gdrdwxwvc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gshownkrw.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gnmdmuqig.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/ghiwblbfu.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gblosrqvq.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gwjsrxsek.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gxvlkkufc.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gxmppiwpv.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gnxwedpkw.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gvhwrlrfw.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gvdptdbxf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/guhhjcyjx.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gghmyuraa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gnhjjdrkw.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gkytazfmb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/geryaqwwt.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gxsglxsog.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gfbzuadtt.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gjuafjvky.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gurdxufkv.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/ghprhzcxt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/grnkqbmkm.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/glecwzmrx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gkztasklh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gexixosli.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/govsnsxpc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghjwchedy.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gqjbdocni.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gwtfigbji.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/goweiueuj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gwikowogj.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/ghowjfhqm.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/guhjyatii.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gbaiwvabz.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gphkvfonp.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gddphgvvj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gdcamaffx.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gtbnryzcg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/glumcfpwj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gdyffwpqe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/golwlsmow.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gfkldwvbr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/glckbtwov.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gdkwgryew.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gyyqdqlkj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gouprlklm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/ggklgmgue.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gtvfpldmv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gocluigja.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gwbvwylyj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gimkkrsnp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gihcdhvhm.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gctplcvgn.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gbuvntqyx.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gopddrbrk.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gfapeqagk.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gwtegwwfi.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gnrowptnn.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/glhviserm.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gksydirmn.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gmbgnfbll.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gknnehmfz.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gverutmks.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gubsdgpmd.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gxkxncsaw.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gaujbdydt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gtymumdmg.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gxuoimdtg.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gfvjthtik.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gfacgzjgd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gonnfhewy.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gwnmnyiby.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gsjellbbm.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gyesxjgzb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpfefpvpz.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gzurwqqpx.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gbuosgnrs.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gxjwmkrkw.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gdidwncse.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/ggjotkifp.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gvgqhmqgm.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/guwvybglo.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gzjannaqw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gqtuprxfd.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gkkiwuiim.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gnsmllobk.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gtjheeyvf.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/grczdcdpe.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/ghpctwrrj.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gamhsclma.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gwvhhamqn.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gtexntrmd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gajvkxxfx.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gbcuheczr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gizanbfvi.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gubzgxdqk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/ggsbxxjer.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/ggbhzpzqk.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gcexdvdyk.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gveofvurj.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gexvcnzxj.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gzcxzpcqv.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gpdrxzjhc.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gjfduizrc.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gmajhyukp.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gxkbfvrpl.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gzghtznel.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gvbevggoy.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gyjqpnbdw.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/glcwuputn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gkbmssbok.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gnofpsrzo.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gkrfoqdfq.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gewrvksle.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gxqgzwakm.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gbeehrobj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/ggpnxdvzv.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gfhpnwljs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gviywdlnf.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gpsniswxq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gjxmmdqhj.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gyubtqqcr.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gbubkkhyb.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gtjhowvxv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gxmhoqzeb.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gfrwqwfiq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gtuumlktm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gxcbggsjd.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gpvqicybf.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gnsreblgp.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gzyydjfol.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gpukmchaa.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gvxgftstq.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gullvavzd.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gnogwxeyr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gcqxvsxhj.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gwkaiesof.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/ghfhptaln.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/guisgznxd.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gpyahzumd.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/ggunpybhk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gwmlkwwle.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gehochszo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gywfqjzqn.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gownkvlel.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gsbhvwtoa.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gibxjvsod.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/galzadsls.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjlmfcsyj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gepvtkhoq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjaaqktts.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gjizkighv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gcjyxtxjb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gufspvkaz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gysximppc.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gklshrnvr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gxzlbrcjq.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gjozjccbn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gdjargivd.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gnqkappcn.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gcvswaxyi.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/grajmzryd.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gpxaormou.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/glnbetdst.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gpdywrzdq.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gxiqlmmjd.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gikcvnjhk.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gdeltorld.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gduadqepb.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/ghbhoyqit.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gpdxwwpod.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/grvvpydkg.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/glwpuormh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gknxgedhi.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/ghsriypis.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gsyskgojd.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gjopifswz.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gyzspxmjb.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gldzgzlip.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gwctusmxi.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/ggniucuhq.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gyksjafic.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gpsnzxjii.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gnuiqohoc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gvxcfybob.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gmabtjueu.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gbxdemftb.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gepvglfxf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/ghmfvccdb.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gckggyhet.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gcrkmapua.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gtniihiiy.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gstbpfdxu.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gichedrry.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gtqwwstzp.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gsbskcrar.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gejoncbxk.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gsdoemirl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gvmcbrmya.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gsztmpaql.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/ggnkpnawm.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gnqvghygk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gmpesjmao.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gdqnrxlfc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/ggpfugkix.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gqrenwkke.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gyenqpmwc.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gbujijmij.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gkjywzfvq.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gmhkynwbt.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gsdgakilb.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gtjhhxioj.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/glvejafzm.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/giwcoqodj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/glmcfwysu.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gzlyumbid.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gzbqdtrks.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gkxfqwfxt.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gskxnvktc.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gjdjhbbxz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gzgbuppko.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gpgstbqkj.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gthcktnui.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/ghkvcdcrf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gvuhwnsmg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gjnohhrit.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gexgidsro.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gxprpwidm.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gvxgzvkgi.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gzfaeiikm.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gkmjpltqt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gsadrgeps.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gudyzrgox.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gmpzcrdov.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gpvfyramb.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gljttdfqh.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/ghdzovjfc.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gtocqqfzy.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gshmwsqeg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gvvyeonsx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gsrxfzlfi.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/glscgidtx.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gsmtuvjfi.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gnykzmirt.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gimawepup.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gtrlweoen.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gokmjgxvq.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gwodzlqte.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gyrlqcuwg.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gtsvwmapf.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gxhblcpwx.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/ggevonnaz.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gabwunjba.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/glqkdmbjb.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/ggurgnvuc.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/geljimije.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gpzmgflvg.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/ghhpbwpns.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gihaujcje.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gmmiaswtp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gugyiutte.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gcvvrkuld.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gvbiplrvv.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gpeilhcrs.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gpamrpusu.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gtlkaosjy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gcivncher.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/girhneaxh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gcthffqps.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/glumawuhx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/glunzmiwr.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gvjobsmwq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvmmjvmha.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gcfmtwjyu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/ghwhopbnx.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gyelawlal.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gjpvqgsdv.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gpujlffyf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gxmpwgesg.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gtnmvinwm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/ghyktkvqs.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gqprqquyb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gmheogcfh.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gsgezxnww.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gnsngfywr.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gfqqjkjgw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gbrwktmjb.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gaicglfty.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gzbgqiblv.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gshficxob.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gdjmocvrh.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gdywryvxo.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gyykjncar.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gcvovqzax.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gapikjxms.sHtML


<!-- 参考信息 -->