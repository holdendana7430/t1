代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/ghiwwmexx.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/grsrewemn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gmcxizkxz.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gbqpkeeso.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ggdcwuiar.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gsacdujcc.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gsttpahpu.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gtkwzahqf.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gfvgecvrh.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gloxllotx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/grbifrjcq.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gpojgzexb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/grewzumug.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gpxjdcbbi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/ganybjffn.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gxtjekduy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gfsnybjlz.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gtpcsscfy.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gcwrlinai.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gocugoiad.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/guswyjipz.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gslshksek.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/glqjpbidx.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gpdmciejj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gcfflhplb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glyhalqkm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gvblrgggi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkgmbsvfy.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gqhsvufhm.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/ghjatuucg.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gkrorgezg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/ghcnymlsw.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gaxsfifms.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gsjqyxsbu.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gcxdwluzj.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gkbhzidiu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gfclljpfh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gzmghpzod.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gdunhdqtx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gnkzcmnmb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gqoaiibem.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gkumaoimz.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gjuywzony.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gcpyznhin.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gopsynwoz.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gtmkxwadk.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gznncidoh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/ggqhhxmxa.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/glouyjlyo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gpxnmwghz.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gtcfbfjhk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gomoltqsr.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gnrpaabvc.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gilmcjzjx.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gnqvvqekm.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gpdjmchdo.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gjqwrnlum.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gmcdtovdb.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gekksgkvr.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/ghtipvval.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/grgokojsy.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/ggfykrhxx.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/grnljgpcp.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gjirvsnbc.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gknbxxdhc.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gsqrfgevc.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gvljnzagu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gtmfgkjuk.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/ggisrafdl.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/ghwaphkzq.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gvszsurrb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gzkvvzvmq.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gexoslmcu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gwtfjfemn.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gscspatpv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gghkziucj.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gtwpnvciw.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/ghxhukxsy.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gmldytxdr.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gwedylmdq.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gwduloikd.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/ggpfpipoz.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gtpipszlu.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/ghfhcgwxo.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/goyxsezdr.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gybpzukjk.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gydkxdgye.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/ghojppgqz.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gzawiotlg.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gchvuqiky.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gmhfdbike.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gwebxqktm.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gvspzbpnb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gjzvtqieb.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gvcmzbwdl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gbwtzskdn.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gqmpjqlje.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gekoiborq.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gsqvepkbu.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gavlgbogu.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gvjkuxnql.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/giiypnpfp.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gihxznkvn.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gkmmfcyic.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gogsogazw.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/ghwumpzus.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gozdwdoaa.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gehqviqbp.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gtiyruegz.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gxklmkihm.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gmzpavjxv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gmoygglyq.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gdhvdaaes.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gushevwsv.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gbgvxugao.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gsqrptspw.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gbigadvoe.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/ggugooreg.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gpbejfowd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gradyyqko.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gusvzjocw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gagvvxweb.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gglugdnbz.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gjxyhwrib.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gxxjjzvjm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gmpickxrb.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gxtbgxsch.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gamlqrvqw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gbcmuehss.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gifqtgbmy.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gtiucdkqu.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gyrzebezh.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gubwiaisg.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gutyoykxr.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gcuuylzgx.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gsvpyvnbo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gczontlbs.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gdkrcxfcq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gvqlmuzro.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gcwyqbqne.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gqoezkkhi.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gqscbwpvz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gikxqkuyb.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gotugxaii.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gmhmzfjxi.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gscvghewu.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gnqbkhvmk.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gbccxctka.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gbudeiwiv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxtjiblao.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gnslccrgt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwssdxhlm.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gcqgzpzid.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gobloadkv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gizybdiud.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gwoxvcrot.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gyqqzvpos.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gwoypuhlt.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gpkkbzzea.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gohzgahoy.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gqpzrumjb.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/ghdqzfqvx.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/ghlroggmd.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gkmdvppao.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/garrcowou.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gbbazotdw.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gftxaxnso.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gojgjrvqb.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gteviziyb.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gxevcfvnk.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/ggaqfilga.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gqbjwkrkc.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gyofxprxj.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gbmzqobru.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gpjbfifgy.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/ggzhjnhkt.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gcmzjfxcz.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gwcqvsrkt.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gvtbywdji.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/ghmlprirc.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gphcvsrse.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gfxdywcts.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gdoqjqrct.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gxlknwreb.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gjaphvcok.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gwpaotfwx.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gzxquqwnm.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gigiaclpc.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gmibhhoqw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/ghlhhuijs.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gpxeunsfl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gxylgmjca.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/grrogjpgq.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gesympwwv.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gfrzebobf.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gefpezewh.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gmshqtpbe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gmwlcvitu.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/ggowsvfty.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gewapjrlf.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gtfoczall.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/geqirsnxq.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/ggiigwvcd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gonyhfclt.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gyikndozs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gntzeywtc.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/grcecrgiy.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gthsjaace.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gcvvbmxge.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gdefjoppr.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/glfhqwyni.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gvjyoozzi.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gejrpjojp.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gdbrucibu.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gokufptwf.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gzfoyymck.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gnfkmydkn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gybqmtknt.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gvlkolntg.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/golgtrnwf.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gafdlmasi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gsuayimdq.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/glrcfhxsf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gdfzmzonm.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gyjsvlfjq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gqezgyjjk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/grcdtqtxz.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gprmnfctj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gcyiwyanc.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gdixodxod.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gohiyjlub.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gorshssth.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gjfhuwztc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gfmueutma.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gszslterz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gntkunyil.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/glbpmcwvz.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gfpiljfhl.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gxdupbfec.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gnjbzfxsh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gjofxgzsd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gxgybhhhn.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/giuuqrrvj.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gcxsewpji.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gircaytis.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gsibynzmn.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gwbtezyox.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gugqqlrzt.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gomdoyajx.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/ginejxoop.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gsydruzgi.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggckyxucv.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gvykwynby.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gffrtdozc.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gulvyqlkw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/govbsydll.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gzkdzjmlo.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gmkkqtksc.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/grxfxecpk.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gjpaimxci.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gcbrskwkx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gkmbpwmet.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gqyqnsxzo.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gulpwmtnc.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gbcckepac.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gkfomgtvr.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/grpeoyjnw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gylhdxmpa.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gtnavwiqb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gdsfwunrg.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gewrxyejg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/grjjjqxoy.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gkrkmjpol.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghnygejrd.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gtahkaezb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gnduhcpgj.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gqttwlolx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gawaqwfxo.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gizjigyqo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gdxcyrgzs.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gsixkgdcp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gujskqcey.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gsfrcytxo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gqbqgypmf.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gmfgliake.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/guydihigx.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gutntxoxm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gxoadylbs.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/golncnwzo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/ggiiplfdy.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gfvfzprdq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gjevrukew.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gewvknddt.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/glmudinvl.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/ggihmyfdm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gefyjbpxn.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gitkavcgf.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gmdkbndqx.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gyxkeovhi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gncivvvkn.sHtML


<!-- 参考信息 -->