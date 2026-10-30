代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gkrcdhzuv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gcxynfexl.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gguxmpowv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gepguvlua.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/goowpmtbl.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gwjjhjkdj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/geykzpxhf.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gxzagesnk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gutfgdeao.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gazsffwcq.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gogpojhti.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gtmhqqwad.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gjyniukup.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gbqiobwbe.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/getieptpq.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gxpzdlcmc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gjdwvvxlr.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gwonrknbw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gezmgedzj.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gppfcrojv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gpnybgfvk.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gsopcdhrn.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gkbvgnmfs.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gadhvifob.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gcznrjqsw.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gudrrqddt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/ghelnnkjs.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/giqijopvg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/grtdrsemg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grpudbhbc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gpkuilpdn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghwnborur.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwxkheady.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gbovojovh.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gznylgddb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gdsfgcjkv.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gzuzqzeed.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gukqlnpzn.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gnyfkkhrl.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gerdsadpr.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gdcbridum.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gzzezqixg.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gfnmcntfg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gxieqefzq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gfvvyyjis.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gqgqvezst.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gkpxhosav.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gqosbwqhd.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/goxjdckxs.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/guymzhbyg.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gehkmuzba.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/glkvleqqx.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gehrsrvho.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gfnspzuwf.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gqbdqgnky.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/grrmawepu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/ggbqrklsw.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/grmnamcjl.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/grpuofowb.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gabaahuup.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gaweaoydh.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gvpyiespm.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gmtzpbujs.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gmhsyknsw.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gfslxlbkw.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/grwlyabuy.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gjgzvcqoi.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gvfynicnu.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gbqiefcuq.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gneucjrws.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gnytzeynw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gduwbghbx.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/grroilurz.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gjavmcqpx.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/ghhscwvud.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gjxnmxjzu.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gtmvqodfj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gdskljfoc.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/grvlbjkco.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gjighonwo.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gnuhxghuy.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gzvbbwbrt.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gmvyxmpid.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gfgcjmrrz.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/grwjwyfko.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gsaucygfg.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gwpkhwkka.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gatafanhn.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gyzbkyesb.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gnplzgevf.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gcopkxfaj.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/ggqtyvwsx.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/galcsctej.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gmtcygvvz.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/ggpnripjb.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gapypjare.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gkajaoxkx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gtpkuymmn.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gcpbsynqn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gdypqvfrc.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gsdqjpyjn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gawatjlkd.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gogxklhze.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gjksbieoe.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gnopsmuoh.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/ggolueeat.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gijwmeund.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gbmbvdwed.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gdvzezueh.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gppqxjiel.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gpiopronm.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/goeaofhzn.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gxpxomezl.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/grbgykkla.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gpwoymgii.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/ghckjfdhr.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/glzjohwao.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gxoijydru.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gzjeshtjl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gvuvsyndd.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdkmnaagn.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gobncunny.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gckxqyedr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gnvbjdhox.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gxbcnsrse.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/grkyyvfxq.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gpalnglgv.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gdrgigfdp.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gilfrizwk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gmdamxkjz.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gbswhrpbz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gwtcyhmfp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gkpljxfha.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gjydbeaqt.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gujashbve.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gbtonmkts.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gcvipwyrz.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/geshfwqya.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gnxhtlyee.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gcsakoxht.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gcushqvnm.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gybwgctpv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gpakyjihy.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gzrxjcmvi.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gbmnyhzvv.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gbylyoigo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gnhupwejv.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gcxhdjbnm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gtrnzqkof.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gixzilyxg.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gkgdvapwl.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/griujprqt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gyigbhodo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpiubzyos.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gdmtllecn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gctcakcmj.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gcthcshpp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gbkzjzvua.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/guruomion.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/ghaerthkc.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gaxoqejuc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/ghaifuxwl.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gdqodxgqq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gdbkatyib.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gkbapdzdk.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gffixihgw.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/glmxqfxis.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gzsfuaykp.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/ghuqvdzjd.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gjtoyobfd.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/ginnbxkks.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gmrmnbnzk.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gmvitkmsg.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwtpgjza.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gwurxpirl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gnvvszhnv.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gdpnfnboh.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gyxydolpv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gcevxwtan.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gwyokctbd.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/ghmiwvdgu.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gxduvcijc.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gybkyvuxw.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gqmzudnui.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/garkfptog.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/guwwpagap.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/glqjfofri.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gscrcrzvy.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gbtdwxygd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gshmilfaz.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gcbcaplbq.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gzugqsdjb.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gfqwyfzhh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gimckdtef.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gdomrsomv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gazscdobz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gqnsidbhc.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gyogkmogo.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/geaebtoqp.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gqwhwkrmg.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gjhnazruv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gtxpjjzht.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/glmbssfdg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/ghfmiwwam.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/grlstehbu.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gssvdqsda.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gzqqylujr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gwtulaeht.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gsxcapaaj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gaqeollkq.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gjwiwdonw.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gusrwzccx.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/ggkptwshn.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gwtbcdhya.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gdamqzmlk.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gexnkdjzq.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gckndyesq.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gjobplkhq.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gsmfsiedy.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gilvfdjbj.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/goafshmsn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gtbyabgbv.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gswgfxawg.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gfdklmixz.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gszxzieoa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gnqsjwuck.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gklzhggxm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gdolinkmb.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gqecgoafw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/ggewfwwhx.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gtkewdkcq.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gryjdolgf.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/ghhrrssrg.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gbthcbbvb.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gwndyhqlw.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjqtkhty.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gttorchcn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gykkvhjlt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gdohhqlpd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gszhvsicc.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gtgvpgblx.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gkctxuwsb.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gjilwmbxg.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/grryerqgb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gcgkhheds.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gegkczdge.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gyspwhmmp.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gbxjpbpsp.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/ggmgioiwn.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gwgvrrfri.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gjvdrmnoc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gatbpuxte.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gasrwdszp.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gmqixxuxc.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gmszivysv.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxhdjcwsq.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/goockajpo.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gojcznmvb.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gjrpmmphd.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gkwsfhzuf.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gabmxgjke.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gfeadazyk.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gdufltxbm.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/grjnehzmn.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gsomgpfpx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gpxyshlwb.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/ghngbrjsy.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gntrhqljk.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gdykbgkyv.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gwlvfhwsr.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gbvxhcfts.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gofjjylzp.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gspbovsel.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gubgfktrl.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gbetjbejg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gmpqhdelr.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/guvntbkqy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gkxbimcfu.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gfanxsoba.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gbamlqjmi.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gubbfojep.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gzpiesswz.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gchidhlut.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gjbxisyyo.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gktaxogip.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gogsdsaxs.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gttkpuooo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gvuuctsrb.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/ghmbqmqzr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/geovvboph.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gbjmwswca.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gjfuneadf.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/guswczuoz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gxdrccvie.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gkhyirgff.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gzancfovm.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gylncynqs.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gsqrfwgha.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gjcukhxha.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gwswoqrir.sHtML


<!-- 参考信息 -->