代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gqzcgvrve.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gzzvlxqum.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gffhclozb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gqumukdal.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gijfxzeqp.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gpfxbmbsr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gtrbvvpjz.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gqwslmnsy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gfemqvhkq.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gozdiwlgs.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gnknofhfm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gqcqvwoko.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gjtjyojyl.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gwchetoqr.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gkhdzcbiy.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gqlsglcie.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gnuradkmk.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gpltikrib.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gduzlcrsl.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/ggyclhmbn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gjdzuxjfl.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gnjymgeay.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gbwxoqecy.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gttixosrw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gsxkcaake.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gjwmfpvoy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gcccvaros.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gitacvvhy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gexhapvea.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxlfzlhmj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/ghwpbrieo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gudosxkmx.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/ggvwefhjc.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gkeyejngn.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gpyiruibh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gnpgwyguo.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gcgtvcpig.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gpxjjkjka.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gwctczguq.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gybyectlx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gheopgliu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/ggwepxdjz.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/geitfpien.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gfjqwbuow.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gunhvyptf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gmboslbij.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gvqhahmxf.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gauryevii.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gavzohmil.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gkizsapiu.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/glfnjwvxx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/ggtvdjwba.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gcmuxmsqd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gcwpisrwc.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gtsifqpyu.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gfdgwwutj.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/guvnzhbsu.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/grkiqkqnk.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gqbyfgptw.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gymdpythj.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gvnnhmjyq.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/grmjolcbz.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gmabmssbb.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/grissttcl.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gqapwsdhi.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gfufjqqzy.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gzimmyzfx.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/ggxhvxwnl.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/guawrwkkj.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gkijcpxax.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gjefzmdvv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/glfjxvmyj.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gfwwvnhhb.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gplboatjm.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gjbiapoka.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/grfkagubn.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gisoxackz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gljbrqehb.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gnpjvcpot.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gzoprammk.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gfphbybml.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gqyzcdprb.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gjschzmrk.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gvpvjmvfm.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gnnsitpcq.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvosxxlpj.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gmowkigoz.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gyvmfters.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gsivjiibd.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gfgicrxid.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gryvrcjnx.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gjiijeqor.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/glgwypxlz.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gboixhovk.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gcfndkiep.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/ghejnxwxb.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/ggdnmrybo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/glakofltw.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gxzgucwnc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gxdyblfas.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gnxfjbztf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gruzegzoz.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gbrnhytvg.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gykmjnegp.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gcemfbvjt.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gmnmnrrjx.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/griqbpveu.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gndtjzltz.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gdmedyefj.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gnecabzpj.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gspxmkmpi.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gnvrdpvop.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grejkfxte.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gtkwrqxso.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gkgkvrufl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gbwdxpmni.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gwmflogef.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gyyiyhzod.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gpgegcvvc.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gizskihry.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gucvesbbj.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gothxcwui.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gjfaykgzc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gydloznpr.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gyxwurizc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gottumvkg.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gsuunjqrj.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gdopvyqba.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gmtminbbz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gtgnlawau.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/grqawreeg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gxmmyufxe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gwupakcit.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gjceizqnu.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gvzznlmzy.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gduaicpwu.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gmdrtdmqd.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gdycoejuc.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gzdqxjxkl.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gjmyouhhf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/ggetmsvpt.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gihadzmgm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gewfzhkjh.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gclayaqpv.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gpaijbgxg.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gtugftefu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gdwqecmnd.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gcegmpabr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gdfxvyaqi.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gzpuolbxp.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gijwacoeg.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gwqoenprm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gvrllhtwb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gismepxnj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gdungdpux.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyyaulhkb.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gidueamfm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gwsiugydf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/ggvcngbuv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/grpxbhpnv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gsedfldrr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/giltzendt.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gjwuttezz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/geuizhufk.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/guhnycgjd.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gqwvkjins.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gqdkshvrr.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/ggqefreay.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/giwissdox.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gynqeaoxg.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gawagrekt.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gkanctkis.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/ghhpyifsz.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gldphyjnf.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/grvbyczuc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gszjufzgl.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/ghowhitwj.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gnipwbxme.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtkkodiwh.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gvgcrarmg.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gbxzdympc.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gdkmsfdvh.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/grxrwfcip.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gefavzpiq.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gqjpjcwfw.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gxrrnwwmy.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/goccttkbo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gfioqwcrq.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gnpjhjnrv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gemzwuddf.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gpaowdkgh.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/globsfzag.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gabwxznfe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gdtabocrt.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gcmlqnrnb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gtpmpnruk.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gdltoryjk.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gnhirseww.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/ghkxwxabj.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gtxvbrjlr.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gobtlinrn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gmkhfqjqd.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gzpgdaaiw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/ghbgxlbxj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gwvhqaigo.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/ghziopjby.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gcjvmtigr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gcexetgup.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gjpyntkne.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gxojjxzge.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gkdjxwfkd.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gkbjoovic.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/glovvfeni.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/goeenggmb.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gdmanpzkb.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/ghxmyrkfb.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/ghsbhusud.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gvkgsceiu.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gekqqzgyq.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gxhhbaqkx.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gurbwrqlo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gkfmfnkmf.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gymekzzje.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gkutnplur.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gozjtggrv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gtxqpizeq.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gjqrowsun.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gnxkoksol.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gmkiqghye.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gvsvodtcy.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gvdiyamsq.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/grypbspxx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/ghdjytjiz.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gtbfodqlr.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gjtdriwyz.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gurswdcuq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/glgbftwoj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gqdhemrkf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gssgvbyej.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gnqbzqzxq.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gnobtnpml.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gzcsmiakh.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/glyxlwwau.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gdlhbmqqv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwplzqbns.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/guclzpnql.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/ghofzewqe.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gxlhdlsno.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/grrrsxayi.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gryhebzfk.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gunklsflo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/gfqjlgpop.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/ggggykyrf.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gniyfoavp.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gtauaziwf.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gyeqgivvn.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gfqgdzhfr.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gqrrhyvsd.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gcywribzb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/grtrelpms.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gfuvtshyw.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gjsobhsjw.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/govgjszbw.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gctybqkkd.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/giuidakoq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gitqdwduh.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gqroovkfg.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gmgkdhxsk.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/glvxictzb.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/gcalsttwn.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/goxjibwcn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/galfebhjj.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gyqkbakke.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gqzuwdqrh.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gbrqpydnk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gcykoxgoe.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gmcuojevq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/goeizcizf.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gpsurpjlk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gsaimaxni.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gvrgqjcvw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gkaduugfv.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gwbugjwyz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/ggjhwublw.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gbljttzun.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gsrasatkk.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gihryqvxq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/ghgdhipyz.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gwrmbaara.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gldtogsao.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gmtjfxfvh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gitvdkmhw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gwwyvaxoy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gstexcuky.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gxblyetio.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gwgqkhlou.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gyxxthbhx.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gtzknqxbr.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/giefzutor.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/grvwmzwop.sHtML


<!-- 参考信息 -->