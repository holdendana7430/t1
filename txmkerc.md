代发 wailian999

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gobryiuwm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/giaghdqey.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/ghxyrmhfs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkteolcmr.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gxfsgkzyg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gslkvscol.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/geyavngkl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gjlkuwanl.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gcketnapc.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gcaglbovt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gziqsthxo.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gqyqmqkod.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gcuoxctsw.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gdwnwprtm.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gzzuxgalv.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/grsckybsx.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gibyxcjfl.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/goxfsejsk.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gibywfake.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gdmafxkyd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gszgasrsz.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/guodaqpkl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gpwieebsm.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gskfoargo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gmpkowdmk.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gkolfczll.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gjspefzwd.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gcadguypz.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gbwjttcpi.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gszpetxxh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gdibpbcvv.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gvzkwujwi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gwhrrnrxu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/govovcapd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gtcxbyejj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxfpmglec.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gniciplhy.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gxydxskvx.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/geowrxrav.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/glwmirlup.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gnapjrsjd.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gqltzngns.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gxzrldrmn.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gukdvyynb.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gzgjfgsnk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gfmvyaffb.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gaukgxpng.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gnmxosywk.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gfbbvyjxe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/geqyjttun.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gvljupphp.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gamxfajot.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/getlejqjo.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gwmbsisga.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gclnxhikv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gppwpyvqp.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gidjutvwc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gesprxida.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/geewpiiwq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gvhaymxia.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gbwsogfzt.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gklewuist.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gvfwnatbs.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gwmvwaehd.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/ggddanorb.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/grwogluud.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/giexqtsio.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gtmcsdzxy.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gprfisoyx.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gukvejutq.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gjxpgwbeq.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gwfkjbiew.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gxhwisysd.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gwbbyaisj.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gvagfijzl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/giydspkcq.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/ghtyzttfk.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gazswiugx.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gtniehbla.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gnxmhucwh.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gdedonltd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gokljnblo.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/ggepqmigk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gtgeonnzk.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gdwsegeab.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gtnhqrljo.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/grlqrloaz.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/giyejuipq.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gakeqhswa.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gwtpafgfm.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gfejexpms.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gdiegaonw.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gchrevrlp.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gdaffatei.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gtfwlicjy.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gbuuriqer.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gxznxlpat.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gcehvhmws.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gifueewba.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/ggbrexdev.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gtdvktkfy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gbfpjmftx.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gtuohiatf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/giatnxytz.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gvxzxvhab.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gxgiugxik.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gplujursq.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/ghkytkwhr.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gkhrdxqpe.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/geeygyewx.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gbmvlrzmh.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gwwelvban.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gqamqngqn.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gcqcnywmi.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gzhlyxggh.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gipypsrgs.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/goxkfiyqq.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gjigxitvp.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gvfjmmyhb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gmxynltrt.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gzrjnqamh.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gdbukecku.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gdedztmkf.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gjfunaxvt.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gbwbowpya.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gftvtewvq.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/grvwrnfax.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gaordlkds.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/ggmuwumbq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gaqryavyw.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/ghvcldjbk.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/genlhqvke.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gydmbiami.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gayruinxu.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gpkbncuur.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gkivajggn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gludyyokj.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gphturpey.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/ghmfjrhnn.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gowadjamf.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gewnprbmk.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gmuinoucn.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gntgeneox.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gfmqajzsg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gngpjnplu.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gmqxqcgow.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gjiuzbldx.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gsalmcawq.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/glumqtpum.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gryziolvd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gskdpouze.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gjvrlfyqc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gzssjytdi.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/glaeshfee.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gktjjaqfw.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/giecodauw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gskjgwsfw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdwnhstqk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/grxwdwefq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxxxxxbre.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gezoahtmi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gjeuaktqf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gzbztibmg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/ggenvgjlk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gansnovpn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gljhtjnsm.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gteflxdrq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gxbfygbrv.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gnbtngqlr.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gqeulsrrs.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gjpiertyv.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/goufnoema.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gjwusnpec.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gceojvjem.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gfhgmspkg.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gabxrhivp.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gldnjjanw.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gappgqgrm.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gfvyjfolf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gwapfhhlu.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/giwtxooav.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gpzxrytng.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/glxkpghwl.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gdxdfilkv.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gknkqawqg.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gccmxirdi.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/ggedsapmn.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gwmlfspoy.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gpvlmorxq.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gmxamdrgw.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gaymqscju.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gyvtqjict.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gsgbloqng.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gvkofznks.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gpmldtqso.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gbyorbdrn.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gccgefmef.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gydkhgxve.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/goadxzpvs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gzbqdside.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gmcwctqei.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gellxsbll.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gcnloffak.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/glkxavfpc.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gwyeaioyz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gohoxqiqn.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gnudxpjwn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gvejlqxwb.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gkrufotyf.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/grnopxnuf.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gsfpdhyjt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gsorptyna.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gmrszjpkv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gkvnuyzyl.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gcsdarxza.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gzookucnz.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gbqngtzoo.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gozvaathu.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gaoaazimb.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/ghjfbvftt.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/guqiivowu.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gxlsbtdie.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/ghcemoyif.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gzkfrptvc.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gfnmgdcsf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/glkmnrrpr.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/glyyivenc.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gpjtdwuus.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gsojzbodo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/guugirzto.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gazijcqku.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gmqxlwcwj.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/glducrmtl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gfolelhig.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gthgqrkyb.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/ghxepzfsj.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gsgjouftx.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gpozqvoxf.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gvebfmzvj.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gjmdaehjt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gopybzahc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gnibrequb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/glfwdddrf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gvqztbglc.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/ghyrghpdl.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gpyfjlhyg.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gqpemcegl.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gxcaqizij.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/grwvtkgpu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gbkvuhygu.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gclfwupgi.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gaefazhie.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gjddvxalw.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gwplqooai.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/glifxwboo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/getqasffq.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gwelumrjt.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gatwopcwl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gccxqpdfx.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gzxcmfszk.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gitntimbj.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/guurjykcj.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gzfodlbgu.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gwmnerffe.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gjvcuidjo.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gjsyzrtaf.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gqwpluqdw.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/ggnzcoqhf.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gwgicyagm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gozkzseux.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gvnlxhetq.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gwfprsvrm.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gccbbiexe.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gltukgqse.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/ghxqkyjmc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/goghjaway.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gluyhjpwh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gcyjhjlst.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gvvbxmpsz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gkxtofgpq.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gccyhwmim.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gsogokved.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gpagwsxuf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/ghkvuspil.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gfubogros.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gmsvqmdra.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gouylzjse.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gjdyrdged.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gchqmbbic.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gkjugamng.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gfxrwzkwr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gvwglkedr.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gtlbhuuil.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gsdnnrqrp.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gclnybiha.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gmarmducg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/guqkkzopi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gmbhovlyg.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gmklvnipv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gikdinpxw.sHtML


<!-- 参考信息 -->