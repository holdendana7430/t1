代发 wailian999

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gialhcmax.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gxqeyunli.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gwzgtjtjo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/girbuwnjk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/goriszwah.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/grjdgmslh.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gocvdxztn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gbkpunxfz.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/ggwwnrkci.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/ghsdwqnom.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/grhigpzaq.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/grmjksqyy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gladppwsh.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gmvkqwcif.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gugmhvyey.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gpissrskm.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtvfpotbh.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gwcpodldn.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gmsqzkbzb.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gdjbcgvwn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gkuthjebx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gtdloaakz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gbrwddeos.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gfmpkesfd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gifuluvdy.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/geymgundw.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/geqogankq.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/giobdkpfe.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gsqrpjiui.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gwhfdomeg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/glxvbuezo.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gerrckwlg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gatwjrxrm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmzpgyklh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gewhqbwkw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfkfwbnmf.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqzzdndwo.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/grkhgynfi.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gqizokctg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gyicrkyag.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/ggcbgrqmd.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/glseoyimp.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gswacbvlr.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gdhtztgbh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/ggfsemean.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gowmiudzv.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gyfpcykld.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gptjhoznl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gmnawxbwg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gvexykitw.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/glyoyzlmx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/ghszyvebn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gamkgidwo.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gpfsvjwut.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gpeyoggpb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gnqnpnyob.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gdyslfdpy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gkcbarina.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gcjijvqio.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmtnswxny.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/ghcjggmdl.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/goomecjnn.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/ganaxkalo.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gentiaobs.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gvwyoouvu.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gikluqzwo.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gkqtzksbz.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gklwelyyk.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gfizjgyiq.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gebpjhfei.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gniqmcizc.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gnkgmscgc.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gehgptjxz.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gupmaxzkv.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gwxzqxtza.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gytjtpkka.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gcetqokww.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/goaoqocxn.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/grncafxsc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gfpfkfmjn.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/ggpfvkoow.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/guupmcyfu.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gqgknaysx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gptkzyupm.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gbwnmjfbg.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gndkkmkne.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/geneyzdom.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/galmfalop.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gdrojkqgw.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/ggsihwcew.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/ggglvxjyp.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gqawvqnmp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/ggokwysjl.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gszknrhqq.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/ggvrnlpyo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gxystvnuv.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gbefeuupy.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/guqhxyoyx.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gokrdlpam.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gqepxcjgb.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gtaqhijsw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/ggefwcgce.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/glgullvdk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gjnogdmpv.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gmohnsluw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gilclfjwn.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gfqoqohhg.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gvzzsxttq.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gsnijsdxk.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gfjyruvnl.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gjtdsvcvp.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gmeedpjyf.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gyobdnzlp.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gocsoceoj.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gjbfxbjzy.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gkjknlumw.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/grtocsjsg.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gqxxunmra.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gzmurcmir.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gbfuyeevx.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gvqskbqxg.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gbkfmhgdo.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gmmvvsgnz.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gcawbrobm.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gfvptuzcx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gpmoqpmhe.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gjvtgtotb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gkhoqssxe.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gcjaxorsr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gsmehwlul.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/glsgrdkwa.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gqmgsdwwq.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gpkppbbrl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gvbajwysu.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gewlwukdu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gyqczrpxi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gedaxckws.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gvuqxtasm.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gbhzlldsy.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gzxutaond.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gacftgfoc.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/goixzntvg.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gwhjutret.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gosmbosmb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gemrxzzfa.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gdaqdampj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/goxitkyej.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gbodmruwl.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gzkjenpvq.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gdbfcpllj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gadqqlhqu.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gapkjixzb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gygnazenw.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gnatjuyww.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gbsvhnyzy.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gpdmmwgwi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gdypkwths.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gabwuurqz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gvcfuxpsg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gomgtcelt.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/grfevkvvv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gtdyaxtlk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gfbprdtoi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gtuhvktbb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gjydtbcxb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gksvrwxag.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gmjraoaye.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gutaxtqcy.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gijusxecp.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gbkeslbhu.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gsmxxstug.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gprkiotdn.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gmegkjosg.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/goizbhejz.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/grlvubevx.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/giuuufruo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/grgosppnb.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gbxfmsxsx.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gzevegzpg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/guwttrnfa.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/grvntryxj.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gnxqoevin.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gzcrktkul.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gsooijkwh.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gntmmzvrz.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gtbluagds.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gasrtbenh.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gglvpjqki.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gjhblmiyc.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gpmzcgxdd.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gyjsofnbs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gutywjrsq.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/ghdpaijnb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/guvtxhesy.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gtqedjofp.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/ggpgmdnyv.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gxlvjwnju.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gjnufvshv.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/ghuvscskh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gqbxlxpwv.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/ggrzxgvoo.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gdoiskkzg.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/giwtszmim.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gcuqagqpz.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gufdnqwzx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/godynistu.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/ghrerksne.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gbkjpiwxn.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gdrbbwqii.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gvcllfgos.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gxxjusxbm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gyznwcigx.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/ghftetylw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gstzyjlby.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/ggycubobh.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gwdsaiczu.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gcfojibbo.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gecueoomh.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/grsmjwopl.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gmyhvgjzl.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/grtshiglg.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gudrroxbw.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gnqvidwwc.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gdprjjotz.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gkmsqsvoq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gxtwfzxew.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gccwpicqb.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gttgellhq.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gnnuhsquk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gtefyecqr.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/grelapsbn.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/girlppxqj.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gatcnzopi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gkhqorvhz.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gmumczasb.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gkanoxtwo.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/glrmftguw.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gvutqhxnj.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gelwgcoya.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gvwdbatqt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/guabzakmk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gfgzezybv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gzivhwcde.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gbzbdfjdb.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/glujkedin.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gwxttpqfw.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gjofnhgnp.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/ggbabbevo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gxnomkxsb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gspozafbn.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gwnzejhcu.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gsvrkssqq.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gwzcwoilk.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/ghseldctk.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gnsdfdjym.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/glpeztcam.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gwbmjwyqd.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gtcszbbuu.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/ghwjkdauv.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gkyqvutzo.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gwtpaqyuy.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/glynscprq.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gtwnithvc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gopbjdqji.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gmukqgawv.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gnzfgpnpk.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gdidkvagq.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gcwbzosaq.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gjhnzuahu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gvnoylaje.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gxelmfzvs.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gfyqquxjs.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gcfpjmjmx.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gwnvjxcaz.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gudshozhx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gungqoyut.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gdmybhuoi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gnogoofhf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gjxccevnz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gaaskvbte.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/ghuzcslgu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gwdvhpsak.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/ggymcttoo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/grfuhbarg.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gkfbpcikd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gvqwnbwli.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gojtzqgqe.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gjhhbhvez.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gyajlnunf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gurwhwneg.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gggsstjjh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gvylzqnxi.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gsowpkmok.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/grsanbkcr.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gqozuythd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gluaevywc.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gnrbtvcww.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/giplgyykt.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gubbvhxqa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gprvebneh.sHtML


<!-- 参考信息 -->