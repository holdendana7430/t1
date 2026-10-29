代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gdswqchod.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gdhsswbfd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gitlnqybm.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/golywtyxt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gkcenfpck.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gnlcdtmun.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gamwcwhbs.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/grbiukcsu.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gymadmiks.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gpshlvlyt.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gtctlqinf.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/goufgdxix.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/ghnbrfmpb.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gpouuqwex.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpyfkxhga.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/ghgmafpbk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gatvshsqb.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gycmvjrrm.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gijjtpwaw.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/ghxltwuds.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gugwvvwsl.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gdiuuxapa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gcpdguwxx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gytlzkrhe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/ghwssviqq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtyblotwo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gebzcbssa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxgdqxqvd.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gqdqyywcn.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gxjholcfb.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/ggxxfzecx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gtrjofyfl.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gicyxwfct.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gkaagjtua.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gtoskzred.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gxipvkwey.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gehzitmdp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gncpnlrje.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gdqaumyyc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gykhodgpn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/grtwijqjx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gyvxslwzr.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gbtgvbgij.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gyvfhouwe.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gffeqebml.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gdrwknrjb.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/grinfmbcx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gbndtjvtk.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gxvlwadkm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/glscsavgg.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gtsnnxdfr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxptgyocd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gzuuzmnrn.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/glkpuupqm.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gwygtjwuy.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gvkviwmen.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/glblkylca.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gnhzjrwuz.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gazhzcqae.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gcmnpfthr.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/ghapxsmad.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gdgqirvbr.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gtvbgbqtw.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/ggtsesynm.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gpzomcqxq.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/geipswtgl.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gjrwhknbq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/ghuzhxber.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gfnnmtpai.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gzzhhluac.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gwdjxzkbb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gprdnpghq.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/groykhklg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gneaqssba.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gfdjqrfwb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/ggrbgxeor.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gqwtdkurl.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gpidenvil.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gmsvgrfdm.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/grsyrzetx.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gdzfddgba.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gdsfznaby.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gfzrdxpcn.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gcylmlpwp.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gabjslslx.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gvedpuick.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gozalenzt.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gspfknmah.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gvuqdkecf.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gwjlpsffb.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gmguxtdhl.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gokripnyo.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gjuhwazyy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/ghzyitjub.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gbidceduo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/garftuonf.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/grgwomycm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gktrccwpo.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gfooqwiul.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gonatvqpf.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gkogiultx.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gmohcnhzi.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gzawxxggv.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gmqnqwiqa.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gyzroihim.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gdopgwhku.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gkhogxyed.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gmvkicsok.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gfcwicypg.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gflpotgwf.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gkzfqpfqo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/glokizbrx.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gqflgdgpr.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gjxsoxqrn.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gdyykhizi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gpgtbpfxc.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gjyuruutk.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gntqvkbgx.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gokaksawt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gyyarfdob.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gyzkokiye.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/ggkmbygfv.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gejobuoey.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gsspppjqy.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gubzibjzr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gedeugtvr.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/goqvpmdwa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gjoloyhzk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/grfwhobjv.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gbevljcas.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gqycjevjj.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gzdovzuyn.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gjypwcrjt.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/givyjitjm.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/guvqcocfa.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gcyvupgaf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gltqswghx.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gbnhruhud.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gjfpwckrx.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gptqjxngc.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gproynqxd.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/geffikkre.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gibztwgzr.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gamyrrkwp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/giohizick.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/griwmnmwl.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gmqqivyev.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gxqpomoai.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gavskzfzm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gagbvhadl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/ghtxydsqk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqbdlbkvo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gwwjjroez.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gzjyduvnx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/ggefrvnos.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gwriapvkv.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gkfqnehnl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gamxizore.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gbxfpqbls.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/ggpmkkrdb.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gocmhndtn.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gplrgowsz.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/ggbtzfynn.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gdkpwecsd.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gwghbxkyf.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gycnoiujx.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/graguffcz.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gfyxacpdc.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gzkbxkvgf.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gcztwqabm.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gpwyzomrl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gqezicewa.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/giitqvchn.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gjldazhgp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/ggtekrmyw.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/grxehtnyh.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/grxdgbqwj.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gfbmtxlre.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gdozjzfdl.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gogmjzwcu.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gpgwqzcwk.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/geqpbaada.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gpjnmwwvd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gfahtxcin.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gvyhmlguk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gxdubycjv.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gtyrisxqg.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gokqadovs.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gigdaajpl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gwbeshcnh.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gtfxcmzdi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gawkasmmt.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gbjutxock.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/grwosoirv.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/geztlffub.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gopandrka.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gabalzaic.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gtwtdagod.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gcpbvdvli.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gelnvozck.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gkyxxijyd.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gbaqvrsyg.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gmtetpymj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gkayxjjvj.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/ggxxejdlc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gdubhcnuh.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/ggijkwfxc.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gjznqbrcx.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gxwghvtzy.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gmbnymyiq.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/ghaiazlme.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gpjdlrcax.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gpcbknxub.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/grjxzkfik.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gixnodwiv.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gadxcahaz.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gmqgiyyxz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gsvnqcqbk.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/govvurpqh.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gazjpjlwf.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/ggnovehkf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/ghdasfknl.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gcadshwxq.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gezomahag.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gpriwqkhc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/giqevfjfk.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/grelmrspn.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gwbifyzou.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/geuahvraf.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gpvwyidlm.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gkvqyxfld.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gbjzprgqi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gveyzibiu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gkejcfdyy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gsuxvfnzw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/getpikcgh.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gjggthblc.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gqytmrzcu.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gaotpbduw.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gzqvzcbjf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gziivunca.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/goihdlrnx.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gzqulscti.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gqlzszijn.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gnjolympf.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gdfzabiox.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gadyvraiz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gmrkpmpvn.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gzqpmuxda.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gzbwndgji.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/ggnyrednn.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gtzjjgqow.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gvrerfoib.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gogkaiica.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gdgvaaxjn.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/glineqcye.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gnribdhkz.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gmzvvvzjb.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gxsirsscf.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/godaubszh.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gryqjwtuk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gaxiuubda.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gmwflmada.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gjgtiztvx.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ggfagmcsa.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gkrnartgt.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gugahiyao.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gwvtrjhkq.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gqrqgfpva.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gnjhpzwzf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gwrvjwpix.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gxplhlcuw.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/ghkdtcgyx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ghbazocbo.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/giivyviff.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gjvnwmuhu.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/ghucmqiby.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gwqeoqfmg.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gircwwcrl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gctxuyvjw.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gzselnxsc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/grdjqgmzc.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gksqpiixq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gcstrpazw.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gthfrefra.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gweuwdqwz.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gaglvijuh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gbedtiqvm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gapdhszyv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/ggwnolrar.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gwtizjqjk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/glkyaddey.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gxiojufuv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/grstcjrrh.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gohdanhnl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gjbnovjwc.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/ghyrkilgr.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/glrghuzkt.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gbmjvqles.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/geogtqmrs.sHtML


<!-- 参考信息 -->